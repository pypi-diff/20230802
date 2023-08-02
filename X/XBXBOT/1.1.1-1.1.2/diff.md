# Comparing `tmp/XBXBOT-1.1.1-py3-none-any.whl.zip` & `tmp/XBXBOT-1.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 14115 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    68315 b- defN 23-Jul-21 18:25 XBXBOT/__init__.py
--rw-rw-rw-  2.0 fat      839 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      368 b- defN 23-Jul-21 18:34 XBXBOT-1.1.1.dist-info/RECORD
-5 files, 69621 bytes uncompressed, 13429 bytes compressed:  80.7%
+Zip file size: 14082 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    68615 b- defN 23-Aug-02 13:29 XBXBOT/__init__.py
+-rw-rw-rw-  2.0 fat      839 b- defN 23-Aug-02 13:30 XBXBOT-1.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 13:30 XBXBOT-1.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-02 13:30 XBXBOT-1.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      368 b- defN 23-Aug-02 13:30 XBXBOT-1.1.2.dist-info/RECORD
+5 files, 69921 bytes uncompressed, 13396 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: XBXBOT/__init__.py
 Comment: 
 
-Filename: XBXBOT-1.1.1.dist-info/METADATA
+Filename: XBXBOT-1.1.2.dist-info/METADATA
 Comment: 
 
-Filename: XBXBOT-1.1.1.dist-info/WHEEL
+Filename: XBXBOT-1.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: XBXBOT-1.1.1.dist-info/top_level.txt
+Filename: XBXBOT-1.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: XBXBOT-1.1.1.dist-info/RECORD
+Filename: XBXBOT-1.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## XBXBOT/__init__.py

```diff
@@ -56,15 +56,15 @@
 
     print('Packages installed, script restarted.')
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
 os.system('clear')
-print(crayons.blue("Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy."))
+print(crayons.blue("Mathyslolbots by Mathyslol & helped by Pirxcy."))
 print(crayons.magenta("Discord server: https://discord.gg/GxQQfPRHcE - For support, questions, etc."))
 
 
 sanic_app = sanic.Sanic(__name__)
 server = None
 
 cid = ""
@@ -353,18 +353,28 @@
         await asyncio.sleep(80)
  
  
 #///////////////////////////////////////////////////////////////////////////////////////////////////////////// FRIENDS/ADD ////////////////////////////////////////////////////////////////////////////////////////////////////////
     
  
  
+    async def set_and_update_member_prop(self, schema_key: str, new_value: Any) -> None:
+        prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
+
+        await self.party.me.patch(updated=prop)
+
+
+  
+
     async def set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None:
         prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
 
         await self.party.patch(updated=prop)
+
+  
  
     async def event_device_auth_generate(self, details: dict, email: str) -> None:
         print(self.user.display_name)
 
   
  
 #////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
@@ -417,14 +427,15 @@
         
         self.loop.create_task(self.delete_friends_last_logout())
 
         self.loop.create_task(self.auto_add_s())
         self.loop.create_task(self.check_update())
         self.loop.create_task(self.update_settings())
 
+        
 
 
         print(Fore.GREEN + "[+] " + Fore.RESET + f"Client ready as {self.user.display_name}.")
 
 
 
 
@@ -813,16 +824,15 @@
           except fortnitepy.Forbidden:
             pass
           except fortnitepy.PartyIsFull: 
             pass
         else:
           try:
             await invite.decline()
-            if not invite.sender.display_name == "cindy the one":
-                await invite.sender.send(self.inv_msg)
+            await invite.sender.send(self.inv_msg)
             await invite.sender.invite()
           except fortnitepy.HTTPException:
             pass
           except AttributeError:
             pass
           except fortnitepy.PartyError:
             pass
@@ -837,16 +847,15 @@
         if not self.is_ready():
             await self.wait_until_ready()
         if self.inv_all == 'T':
             if old_presence is None:
                 friend = presence.friend
                 if friend.display_name != self.bl_inv:
                     try:
-                        if not friend.display_name == "cindy the one":
-                            await friend.send(self.inv_msg)
+                        await friend.send(self.inv_msg)
                     except:
                         pass
                     else:
                         if not self.party.member_count >= 16:
                           try:
                             await friend.invite()
                           except:
@@ -1043,25 +1052,27 @@
                 await self.party.me.set_outfit(asset=cosmetic.id)
 
               await ctx.send(f'Skin set to {cosmetic.name}.')
 
             except FortniteAPIAsync.exceptions.NotFound:
                 pass
  
- 
     @commands.command(
       name="backpack",
       aliases=[
         'sac'
       ]
     )
     async def backpackx(self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None:
         try:
             cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaBackpack")
-            await self.party.me.set_backpack(asset=cosmetic.id)
+            if "BRCosmetics" in cosmetic.path:
+              await self.party.me.set_backpack(asset=f"/BRCosmetics/Athena/Items/Cosmetics/Backpacks/{cosmetic.id}.{cosmetic.id}")
+            else:
+              await self.party.me.set_backpack(asset=cosmetic.id)
             await ctx.send(f'Backpack set to {cosmetic.name}.')
 
         except FortniteAPIAsync.exceptions.NotFound:
             pass
  
     #@commands.command()
     #async def vips(self, ctx: fortnitepy.ext.commands.Context) -> None:
@@ -1130,15 +1141,18 @@
             await self.party.me.set_emote(asset='EID_KpopDance03')
         elif content.lower() == 'Scenario':
             await self.party.me.set_emote(asset='EID_KpopDance03')     
         else:
             try:
                 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic(lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaDance")
                 await self.party.me.clear_emote()
-                await self.party.me.set_emote(asset=cosmetic.id)
+                if "BRCosmetics" in cosmetic.path:
+                  await self.party.me.set_emote(asset=f"/BRCosmetics/Athena/Items/Cosmetics/Dances/{cosmetic.id}.{cosmetic.id}")
+                else:
+                  await self.party.me.set_emote(asset=cosmetic.id)
                 await ctx.send(f'Emote set to {cosmetic.name}.')
 
             except FortniteAPIAsync.exceptions.NotFound:
                 pass    
  
  
     @commands.command(aliases=['actual','actuel'])
@@ -1220,26 +1234,27 @@
 
         except FortniteAPIAsync.exceptions.NotFound:
             pass
  
     @commands.command(aliases=['news'])
     @commands.cooldown(1, 10)
     async def new(self, ctx: fortnitepy.ext.commands.Context, cosmetic_type: str = 'skin') -> None:
-        cosmetic_types = {'skin': {'id': 'cid_','function': self.party.me.set_outfit},'backpack': {'id': 'bid_','function': self.party.me.set_backpack},'emote': {'id': 'eid_','function': self.party.me.set_emote},}
+        cosmetic_types = {'skin': {'id': 'character_','function': self.party.me.set_outfit},'backpack': {'id': 'backpack_','function': self.party.me.set_backpack},'emote': {'id': 'eid_','function': self.party.me.set_emote},}
+
 
         if cosmetic_type not in cosmetic_types:
             return await ctx.send('Invalid cosmetic type, valid types include: skin, backpack & emote.')
 
         new_cosmetics = await self.fortnite_api.cosmetics.get_new_cosmetics()
 
         for new_cosmetic in [new_id for new_id in new_cosmetics if
                              new_id.id.lower().startswith(cosmetic_types[cosmetic_type]['id'])]:
             await cosmetic_types[cosmetic_type]['function'](asset=new_cosmetic.id)
 
-            await ctx.send(f"{cosmetic_type}s set to {new_cosmetic.name}.")
+            await ctx.send(f"{cosmetic_type} set to {new_cosmetic.name}.")
 
             await asyncio.sleep(3)
 
         await ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')      
  
     @commands.command()
     async def purpleskull(self, ctx: fortnitepy.ext.commands.Context) -> None:
@@ -1470,18 +1485,14 @@
             try:
                 if not member.display_name in info['FullAccess']:
                     await member.kick()
                     await ctx.send(f"Kicked user: {member.display_name}.")
             except fortnitepy.errors.Forbidden:
                 await ctx.send(f"Failed to kick {member.display_name}, as I'm not party leader.")
 
-    async def set_and_update_party_prop(self, schema_key: str, new_value: str):
-        prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
-
-        await self.party.patch(updated=prop)
  
  
     @commands.command(aliases=['ghost'])
     async def hide(self, ctx: fortnitepy.ext.commands.Context, *, user = None):
         if self.party.me.leader:
             if user != "all":
                 try:
```

### html2text {}

```diff
@@ -9,15 +9,15 @@
 import sanic import aiohttp #import uvloop import requests except
 ModuleNotFoundError as e: print(f'Error: {e}\nAttempting to install packages
 now.') for module in ( 'crayons', 'fortnitepy', 'PirxcyPinger',
 'FortniteAPIAsync', 'sanic==21.6.2', 'aiohttp', 'requests' ):
 subprocess.check_call([sys.executable, "-m", "pip", "install", module])
 os.system('clear') print('Packages installed, script restarted.') python =
 sys.executable os.execl(python, python, *sys.argv) os.system('clear') print
-(crayons.blue("Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.")) print
+(crayons.blue("Mathyslolbots by Mathyslol & helped by Pirxcy.")) print
 (crayons.magenta("Discord server: https://discord.gg/GxQQfPRHcE - For support,
 questions, etc.")) sanic_app = sanic.Sanic(__name__) server = None cid = ""
 name = "" friendlist = "" password = "9678" copied_player = "" __version__ =
 "4.0" adminsss = 'MathyslolFN' owner = '097271eaeea9430a9e8e1ebe92a65b6b'
 errordiff = 'errors.com.epicgames.common.throttled',
 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded' party_errors
 = 'errors.com.epicgames.social.party.invite_already_exists',
@@ -99,46 +99,49 @@
 // CHECK/ERROR/PARTY //////////////////////////////////////////////////////////
 ////////////////////////////////////////////// async def check_party_validity
 (self): await asyncio.sleep(80) try: await self.party.set_privacy
 (fortnitepy.PartyPrivacy.PUBLIC) except: pass await asyncio.sleep(80) #////////
 ///////////////////////////////////////////////////////////////////////////////
 ////////////////////// FRIENDS/ADD ////////////////////////////////////////////
 //////////////////////////////////////////////////////////// async def
-set_and_update_party_prop(self, schema_key: str, new_value: Any) -> None: prop
+set_and_update_member_prop(self, schema_key: str, new_value: Any) -> None: prop
 = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)} await
-self.party.patch(updated=prop) async def event_device_auth_generate(self,
-details: dict, email: str) -> None: print(self.user.display_name) #////////////
+self.party.me.patch(updated=prop) async def set_and_update_party_prop(self,
+schema_key: str, new_value: Any) -> None: prop = {schema_key:
+self.party.me.meta.set_prop(schema_key, new_value)} await self.party.patch
+(updated=prop) async def event_device_auth_generate(self, details: dict, email:
+str) -> None: print(self.user.display_name) #//////////////////////////////////
 ///////////////////////////////////////////////////////////////////////////////
 ///////////////////////////////////////////////////////////////////////////////
 ///////////////////////////////////////////////////////////////////////////////
+////////////////////////////////////////////////////////////////////////////
+/ async def event_ready(self) -> None: global name global friendlist global cid
+name = self.user.display_name #get user outfit cid = self.party.me.outfit
+friendlist = len(self.friends) print(Fore.YELLOW + "[?] " + Fore.RESET +
+"Starting client.") if self.party.me.leader: await self.party.set_privacy
+(fortnitepy.PartyPrivacy.PUBLIC) coro = self.sanic_app.create_server
+( host='0.0.0.0', port=8000, return_asyncio_server=True, access_log=False )
+self.server = await coro await asyncio.sleep(3) self.loop.create_task
+(self.add_list()) #self.loop.create_task(self.invitefriends())
+self.loop.create_task(self.pinger()) self.loop.create_task(self.update_api())
+#self.loop.create_task(self.uptimerobot()) #self.loop.create_task
+(self.delete_pending_on_start()) self.loop.create_task(self.checker_skin_bl())
+#self.loop.create_task(self.checker_status()) await asyncio.sleep(2)
+self.loop.create_task(self.check_bots()) self.loop.create_task(self.fix_pending
+()) self.loop.create_task(self.delete_friends_last_logout())
+self.loop.create_task(self.auto_add_s()) self.loop.create_task
+(self.check_update()) self.loop.create_task(self.update_settings()) print
+(Fore.GREEN + "[+] " + Fore.RESET + f"Client ready as
+{self.user.display_name}.") #//////////////////////////////////////////////////
 ///////////////////////////////////////////////////////////////////////////////
-//////////////////// async def event_ready(self) -> None: global name global
-friendlist global cid name = self.user.display_name #get user outfit cid =
-self.party.me.outfit friendlist = len(self.friends) print(Fore.YELLOW + "[?] "
-+ Fore.RESET + "Starting client.") if self.party.me.leader: await
-self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC) coro =
-self.sanic_app.create_server( host='0.0.0.0', port=8000,
-return_asyncio_server=True, access_log=False ) self.server = await coro await
-asyncio.sleep(3) self.loop.create_task(self.add_list()) #self.loop.create_task
-(self.invitefriends()) self.loop.create_task(self.pinger())
-self.loop.create_task(self.update_api()) #self.loop.create_task
-(self.uptimerobot()) #self.loop.create_task(self.delete_pending_on_start())
-self.loop.create_task(self.checker_skin_bl()) #self.loop.create_task
-(self.checker_status()) await asyncio.sleep(2) self.loop.create_task
-(self.check_bots()) self.loop.create_task(self.fix_pending())
-self.loop.create_task(self.delete_friends_last_logout()) self.loop.create_task
-(self.auto_add_s()) self.loop.create_task(self.check_update())
-self.loop.create_task(self.update_settings()) print(Fore.GREEN + "[+] " +
-Fore.RESET + f"Client ready as {self.user.display_name}.") #///////////////////
 ///////////////////////////////////////////////////////////////////////////////
 ///////////////////////////////////////////////////////////////////////////////
-///////////////////////////////////////////////////////////////////////////////
-///////////////////////////////////////////////////////////////////////////////
-///////////// async def fix_pending(self): try: #print(f'Incoming pending
-friends: {len(self.incoming_pending_friends)}') for pending in
+///////////////////////////////////////////////////////////// async def
+fix_pending(self): try: #print(f'Incoming pending friends: {len
+(self.incoming_pending_friends)}') for pending in
 self.incoming_pending_friends: try: epic_friend = await pending.accept() if
 isinstance(epic_friend, fortnitepy.Friend): print(f"Accepted:
 {epic_friend.display_name}.") else: print(f"Declined: {pending.display_name}.")
 except fortnitepy.InviteeMaxFriendshipsExceeded: await pending.decline() print
 (f"Declined: {pending.display_name}.") print(f"Declined:
 {pending.display_name}.") except fortnitepy.HTTPException as epic_error: if
 epic_error.message_code != 'errors.com.epicgames.common.throttled': raise await
@@ -259,44 +262,43 @@
 (self.party.me.set_pickaxe,self.pickaxe),functools.partial
 (self.party.me.set_banner,icon=self.banner,color=self.bn_color,season_level=self.level),functools.partial
 (self.party.me.set_battlepass_info,has_purchased=True,level=self.tier)) except
 fortnitepy.HTTPException: pass elif invite.sender.display_name in self.adminx:
 try: await invite.accept() except fortnitepy.HTTPException: pass except
 AttributeError: pass except fortnitepy.PartyError: pass except
 fortnitepy.Forbidden: pass except fortnitepy.PartyIsFull: pass else: try: await
-invite.decline() if not invite.sender.display_name == "cindy the one": await
-invite.sender.send(self.inv_msg) await invite.sender.invite() except
-fortnitepy.HTTPException: pass except AttributeError: pass except
-fortnitepy.PartyError: pass except fortnitepy.Forbidden: pass except
-fortnitepy.PartyIsFull: pass except: pass async def event_friend_presence(self,
-old_presence: Union[(None, fortnitepy.Presence)], presence:
-fortnitepy.Presence): if not self.is_ready(): await self.wait_until_ready() if
-self.inv_all == 'T': if old_presence is None: friend = presence.friend if
-friend.display_name != self.bl_inv: try: if not friend.display_name == "cindy
-the one": await friend.send(self.inv_msg) except: pass else: if not
-self.party.member_count >= 16: try: await friend.invite() except: pass async
-def event_party_member_update(self, member: fortnitepy.PartyMember) -> None:
-name = member.display_name if any(word in name for word in self.ban_player):
-try: await member.kick() except: pass if member.display_name in
-self.ban_player: try: await member.kick() except: pass if member.outfit in
-(self.skin_bl) and member.id != self.user.id: await member.kick() async def
-event_friend_request(self, request: fortnitepy.IncomingPendingFriend) -> None:
-if isinstance(request, fortnitepy.OutgoingPendingFriend): return print
-(f"Received friend request from: {request.display_name}.") try: await
-request.accept() print(f"Accepted friend request from:
-{request.display_name}.") except fortnitepy.InviteeMaxFriendshipsExceeded:
-await request.decline() print('delete 1 dans event friend req') except
-fortnitepy.MaxFriendshipsExceeded: request.decline() async def event_friend_add
-(self, friend: fortnitepy.Friend) -> None: try: await asyncio.sleep(0.3) await
-friend.send(self.add_msg.replace('{DISPLAY_NAME}', friend.display_name)) await
-friend.invite() except: pass async def event_friend_remove(self, friend:
-fortnitepy.Friend) -> None: try: await self.add_friend(friend.id) except: pass
-async def event_party_member_join(self, member: fortnitepy.PartyMember) -
-> None: try: await self.party.send(self.join_msg.replace('{DISPLAY_NAME}',
-member.display_name)) if self.default_party_member_config.cls is not
+invite.decline() await invite.sender.send(self.inv_msg) await
+invite.sender.invite() except fortnitepy.HTTPException: pass except
+AttributeError: pass except fortnitepy.PartyError: pass except
+fortnitepy.Forbidden: pass except fortnitepy.PartyIsFull: pass except: pass
+async def event_friend_presence(self, old_presence: Union[(None,
+fortnitepy.Presence)], presence: fortnitepy.Presence): if not self.is_ready():
+await self.wait_until_ready() if self.inv_all == 'T': if old_presence is None:
+friend = presence.friend if friend.display_name != self.bl_inv: try: await
+friend.send(self.inv_msg) except: pass else: if not self.party.member_count >=
+16: try: await friend.invite() except: pass async def event_party_member_update
+(self, member: fortnitepy.PartyMember) -> None: name = member.display_name if
+any(word in name for word in self.ban_player): try: await member.kick() except:
+pass if member.display_name in self.ban_player: try: await member.kick()
+except: pass if member.outfit in (self.skin_bl) and member.id != self.user.id:
+await member.kick() async def event_friend_request(self, request:
+fortnitepy.IncomingPendingFriend) -> None: if isinstance(request,
+fortnitepy.OutgoingPendingFriend): return print(f"Received friend request from:
+{request.display_name}.") try: await request.accept() print(f"Accepted friend
+request from: {request.display_name}.") except
+fortnitepy.InviteeMaxFriendshipsExceeded: await request.decline() print('delete
+1 dans event friend req') except fortnitepy.MaxFriendshipsExceeded:
+request.decline() async def event_friend_add(self, friend: fortnitepy.Friend) -
+> None: try: await asyncio.sleep(0.3) await friend.send(self.add_msg.replace('
+{DISPLAY_NAME}', friend.display_name)) await friend.invite() except: pass async
+def event_friend_remove(self, friend: fortnitepy.Friend) -> None: try: await
+self.add_friend(friend.id) except: pass async def event_party_member_join(self,
+member: fortnitepy.PartyMember) -> None: try: await self.party.send
+(self.join_msg.replace('{DISPLAY_NAME}', member.display_name)) if
+self.default_party_member_config.cls is not
 fortnitepy.party.JustChattingClientPartyMember: await self.party.me.edit
 (functools.partial
 (self.party.me.set_outfit,self.skin,variants=self.party.me.create_variants
 (material=self.number,clothing_color=self.number,parts=self.number,progressive=self.number)),functools.partial
 (self.party.me.set_backpack,self.backpack),functools.partial
 (self.party.me.set_pickaxe,self.pickaxe),functools.partial
 (self.party.me.set_banner,icon=self.banner,color=self.bn_color,season_level=self.level),functools.partial
@@ -366,20 +368,22 @@
 BRCosmetics/Athena/Items/Cosmetics/Characters/{cosmetic.id}.{cosmetic.id}")
 else: await self.party.me.set_outfit(asset=cosmetic.id) await ctx.send(f'Skin
 set to {cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
 @commands.command( name="backpack", aliases=[ 'sac' ] ) async def backpackx
 (self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None: try:
 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaBackpack")
-await self.party.me.set_backpack(asset=cosmetic.id) await ctx.send(f'Backpack
-set to {cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
-#@commands.command() #async def vips(self, ctx:
-fortnitepy.ext.commands.Context) -> None: #await ctx.send('you have the perms')
-#await ctx.send('now you can have perms to kick people') #@is_vips()
-#@commands.command() #async def kicked(self, ctx:
+if "BRCosmetics" in cosmetic.path: await self.party.me.set_backpack(asset=f"/
+BRCosmetics/Athena/Items/Cosmetics/Backpacks/{cosmetic.id}.{cosmetic.id}")
+else: await self.party.me.set_backpack(asset=cosmetic.id) await ctx.send
+(f'Backpack set to {cosmetic.name}.') except
+FortniteAPIAsync.exceptions.NotFound: pass #@commands.command() #async def vips
+(self, ctx: fortnitepy.ext.commands.Context) -> None: #await ctx.send('you have
+the perms') #await ctx.send('now you can have perms to kick people') #@is_vips
+() #@commands.command() #async def kicked(self, ctx:
 fortnitepy.ext.commands.Context, *, epic_username: Optional[str] = None) -
 > None: #if epic_username is None: #user = await self.fetch_user
 (ctx.author.display_name) #member = self.party.get_member(user.id) #else: #user
 = await self.fetch_user(epic_username) # member = self.party.get_member
 (user.id) #if member is None: #await ctx.send("Failed to find that user, are
 you sure they're in the party?") # else: # try: # if not member.display_name in
 info['FullAccess']: #await member.kick() # await ctx.send(f"Kicked user:
@@ -403,15 +407,17 @@
 self.party.me.set_emote(asset='EID_KpopDance03') elif content.lower() == 'Sce':
 await self.party.me.set_emote(asset='EID_KpopDance03') elif content.lower() ==
 'scenario': await self.party.me.set_emote(asset='EID_KpopDance03') elif
 content.lower() == 'Scenario': await self.party.me.set_emote
 (asset='EID_KpopDance03') else: try: cosmetic = await
 self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaDance")
-await self.party.me.clear_emote() await self.party.me.set_emote
+await self.party.me.clear_emote() if "BRCosmetics" in cosmetic.path: await
+self.party.me.set_emote(asset=f"/BRCosmetics/Athena/Items/Cosmetics/Dances/
+{cosmetic.id}.{cosmetic.id}") else: await self.party.me.set_emote
 (asset=cosmetic.id) await ctx.send(f'Emote set to {cosmetic.name}.') except
 FortniteAPIAsync.exceptions.NotFound: pass @commands.command(aliases=
 ['actual','actuel']) async def current(self, ctx:
 fortnitepy.ext.commands.Context, content = None) -> None: if content is None:
 await ctx.send("Missing argument. Try: !current (skin, backpack, emote,
 pickaxe, banner)") elif content.lower() == 'banner': await ctx.send(f'Banner
 ID: {self.party.me.banner[0]} - Banner Color ID: {self.party.me.banner[1]}')
@@ -444,24 +450,24 @@
 (self, ctx: fortnitepy.ext.commands.Context, *, content: str) -> None: try:
 cosmetic = await self.fortnite_api.cosmetics.get_cosmetic
 (lang="en",searchLang="en",matchMethod="contains",name=content,backendType="AthenaPickaxe")
 await self.party.me.set_pickaxe(asset=cosmetic.id) await ctx.send(f'Pickaxe set
 to {cosmetic.name}.') except FortniteAPIAsync.exceptions.NotFound: pass
 @commands.command(aliases=['news']) @commands.cooldown(1, 10) async def new
 (self, ctx: fortnitepy.ext.commands.Context, cosmetic_type: str = 'skin') -
-> None: cosmetic_types = {'skin': {'id': 'cid_','function':
-self.party.me.set_outfit},'backpack': {'id': 'bid_','function':
+> None: cosmetic_types = {'skin': {'id': 'character_','function':
+self.party.me.set_outfit},'backpack': {'id': 'backpack_','function':
 self.party.me.set_backpack},'emote': {'id': 'eid_','function':
 self.party.me.set_emote},} if cosmetic_type not in cosmetic_types: return await
 ctx.send('Invalid cosmetic type, valid types include: skin, backpack & emote.')
 new_cosmetics = await self.fortnite_api.cosmetics.get_new_cosmetics() for
 new_cosmetic in [new_id for new_id in new_cosmetics if new_id.id.lower
 ().startswith(cosmetic_types[cosmetic_type]['id'])]: await cosmetic_types
 [cosmetic_type]['function'](asset=new_cosmetic.id) await ctx.send(f"
-{cosmetic_type}s set to {new_cosmetic.name}.") await asyncio.sleep(3) await
+{cosmetic_type} set to {new_cosmetic.name}.") await asyncio.sleep(3) await
 ctx.send(f'Finished equipping all new unencrypted {cosmetic_type}s.')
 @commands.command() async def purpleskull(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await self.party.me.set_outfit
 (asset='CID_030_Athena_Commando_M_Halloween',variants=self.party.me.create_variants
 (clothing_color=1)) await ctx.send("Skin set to Purple Skull Trooper!")
 @commands.command() async def pinkghoul(self, ctx:
 fortnitepy.ext.commands.Context) -> None: await self.party.me.set_outfit
@@ -573,30 +579,28 @@
 = await self.fetch_user(ctx.author.display_name) member = self.party.get_member
 (user.id) else: user = await self.fetch_user(epic_username) member =
 self.party.get_member(user.id) if member is None: await ctx.send("Failed to
 find that user, are you sure they're in the party?") else: try: if not
 member.display_name in info['FullAccess']: await member.kick() await ctx.send
 (f"Kicked user: {member.display_name}.") except fortnitepy.errors.Forbidden:
 await ctx.send(f"Failed to kick {member.display_name}, as I'm not party
-leader.") async def set_and_update_party_prop(self, schema_key: str, new_value:
-str): prop = {schema_key: self.party.me.meta.set_prop(schema_key, new_value)}
-await self.party.patch(updated=prop) @commands.command(aliases=['ghost']) async
-def hide(self, ctx: fortnitepy.ext.commands.Context, *, user = None): if
-self.party.me.leader: if user != "all": try: if user is None: user = await
-self.fetch_profile(ctx.message.author.id) member = self.party.get_member
-(user.id) else: user = await self.fetch_profile(user) member =
-self.party.get_member(user.id) raw_squad_assignments = self.party.meta.get_prop
-('Default:RawSquadAssignments_j')["RawSquadAssignments"] for m in
-raw_squad_assignments: if m['memberId'] == member.id:
-raw_squad_assignments.remove(m) await self.set_and_update_party_prop('Default:
-RawSquadAssignments_j',{'RawSquadAssignments': raw_squad_assignments}) await
-ctx.send(f"Hid {member.display_name}") except AttributeError: await ctx.send("I
-could not find that user.") except fortnitepy.HTTPException: await ctx.send("I
-am not party leader!") else: try: await self.set_and_update_party_prop
-('Default:RawSquadAssignments_j',{'RawSquadAssignments': [{'memberId':
+leader.") @commands.command(aliases=['ghost']) async def hide(self, ctx:
+fortnitepy.ext.commands.Context, *, user = None): if self.party.me.leader: if
+user != "all": try: if user is None: user = await self.fetch_profile
+(ctx.message.author.id) member = self.party.get_member(user.id) else: user =
+await self.fetch_profile(user) member = self.party.get_member(user.id)
+raw_squad_assignments = self.party.meta.get_prop('Default:
+RawSquadAssignments_j')["RawSquadAssignments"] for m in raw_squad_assignments:
+if m['memberId'] == member.id: raw_squad_assignments.remove(m) await
+self.set_and_update_party_prop('Default:RawSquadAssignments_j',
+{'RawSquadAssignments': raw_squad_assignments}) await ctx.send(f"Hid
+{member.display_name}") except AttributeError: await ctx.send("I could not find
+that user.") except fortnitepy.HTTPException: await ctx.send("I am not party
+leader!") else: try: await self.set_and_update_party_prop('Default:
+RawSquadAssignments_j',{'RawSquadAssignments': [{'memberId':
 self.user.id,'absoluteMemberIdx': 1}]}) await ctx.send("Hid everyone in the
 party.") except fortnitepy.HTTPException: await ctx.send("I am not party
 leader!") else: await ctx.send("I need party leader to do this!") @is_admin()
 @commands.command() async def id(self, ctx: fortnitepy.ext.commands.Context, *,
 user = None, hidden=True): if user is not None: user = await self.fetch_profile
 (user) elif user is None: user = await self.fetch_profile
 (ctx.message.author.id) try: await ctx.send(f"{user}'s Epic ID is: {user.id}")
```

## Comparing `XBXBOT-1.1.1.dist-info/METADATA` & `XBXBOT-1.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBXBOT
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Best Fortnite LOBBYBOT with the latest features
 Home-page: https://www.youtube.com/
 Author: Mathyslol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

