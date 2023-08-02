# Comparing `tmp/ECAgent-0.5.4.tar.gz` & `tmp/ECAgent-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ECAgent-0.5.4.tar", last modified: Wed Mar  1 08:40:12 2023, max compression
+gzip compressed data, was "ECAgent-0.5.5.tar", last modified: Wed Aug  2 09:51:36 2023, max compression
```

## Comparing `ECAgent-0.5.4.tar` & `ECAgent-0.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:40:12.788879 ECAgent-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:40:12.788879 ECAgent-0.5.4/ECAgent/
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    29881 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Decode.py
--rw-r--r--   0 runner    (1001) docker     (123)    36942 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17287 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/Visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 08:40:04.000000 ECAgent-0.5.4/ECAgent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 08:40:12.788879 ECAgent-0.5.4/ECAgent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-01 08:40:12.000000 ECAgent-0.5.4/ECAgent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-01 08:40:12.000000 ECAgent-0.5.4/ECAgent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 08:40:12.000000 ECAgent-0.5.4/ECAgent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-01 08:40:12.000000 ECAgent-0.5.4/ECAgent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-01 08:40:12.000000 ECAgent-0.5.4/ECAgent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-01 08:40:04.000000 ECAgent-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-01 08:40:12.788879 ECAgent-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-01 08:40:04.000000 ECAgent-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 08:40:12.788879 ECAgent-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-01 08:40:04.000000 ECAgent-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:36.815721 ECAgent-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:36.815721 ECAgent-0.5.5/ECAgent/
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37219 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17287 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/Visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:25.000000 ECAgent-0.5.5/ECAgent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:51:36.815721 ECAgent-0.5.5/ECAgent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 09:51:36.000000 ECAgent-0.5.5/ECAgent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-08-02 09:51:36.000000 ECAgent-0.5.5/ECAgent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:51:36.000000 ECAgent-0.5.5/ECAgent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 09:51:36.000000 ECAgent-0.5.5/ECAgent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 09:51:36.000000 ECAgent-0.5.5/ECAgent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 09:51:25.000000 ECAgent-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-08-02 09:51:36.815721 ECAgent-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-02 09:51:25.000000 ECAgent-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:51:36.815721 ECAgent-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-02 09:51:25.000000 ECAgent-0.5.5/setup.py
```

### Comparing `ECAgent-0.5.4/ECAgent/Collectors.py` & `ECAgent-0.5.5/ECAgent/Collectors.py`

 * *Files identical despite different names*

### Comparing `ECAgent-0.5.4/ECAgent/Core.py` & `ECAgent-0.5.5/ECAgent/Core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import random
 
 import ECAgent.Tags as Tags
 
 from sys import maxsize
 from deprecated import deprecated
+from typing import Union
 
 
 class Model:
     """This is the base class for your Agent-based Models.
     You inherit this class to again access to all of the ECS functionality
 
     Attributes
@@ -112,38 +113,209 @@
     __slots__ = ['agent', 'model']
 
     def __init__(self, agent, model: Model):
         self.agent = agent
         self.model = model
 
 
-class Agent:
+class _MetaAgent(type):
+    """This is the base metaclass for ``Agent`` classes. The class is responsible for supporting class components (
+    components attached to classes as opposed to agents).
+
+    Class components can be used as follows::
+
+        class CustomComponent(Component):
+            def __init__(self, agent, model):
+                super().__init__(agent, model)
+                self.x = 1
+                self.y = 'Some Text'
+
+        class CustomAgent(Agent):
+            pass
+
+        # Add CustomComponent to CustomAgent class
+        model = Model()
+        CustomAgent.add__class_component(CustomComponent(CustomAgent, model)
+
+        # Get properties of component
+        print(CustomAgent[CustomComponent].x)  # Prints '1'
+        print(CustomAgent.get_class_component(CustomComponent).y)  # Prints 'Some Text'
+
+    You can also set the default tag value of instantiated agents::
+
+        import ECAgent.Tags as Tags
+        Tags.add_tag('SHEEP')  # Add new sheep tag
+
+        CustomAgent.tag = Tags.SHEEP  # All future CustomAgents will have a tag of 'SHEEP'
+
+    Attributes
+    ----------
+    components : dict
+        The components associated with the environment. The key is the Class of the component.
+    id : str
+        The unique identifier of the class (defaults to the class' name).
+    tag : int
+        The value of the Tag associated with the ``Agent``. Defaults to 0 (which is the value ``NONE``) or the
+        default tag value of the Agent's metaclass.
+    """
+
+    def __init__(cls, name: str, bases: tuple, properties: dict):
+        super(_MetaAgent, cls).__init__(name, bases, properties)
+        cls._id = name
+        cls._components = {}
+        cls._tag = Tags.NONE
+
+    @property
+    def id(cls):
+        return cls._id
+
+    @id.setter
+    def id(cls, val):
+        cls._id = val
+
+    @property
+    def components(cls):
+        return cls._components
+
+    @property
+    def tag(cls):
+        return cls._tag
+
+    @tag.setter
+    def tag(cls, val):
+        cls._tag = val
+
+    def __getitem__(self, item: type):
+        """Wrapper for the ``_MetaAgent.get_class_component()`` function."""
+        return self.get_class_component(item)
+
+    def __len__(self) -> int:
+        """Returns the number of class components attached to a given Agent."""
+        return len(self._components)
+
+    def __contains__(self, item: type):
+        """Wrapper method for ``_MetaAgent.has_class_component(item)``."""
+        return self.has_class_component(item)
+
+    def add_class_component(self, component: Component):
+        """Adds a ``Component`` to the ``_MetaAgent``.
+
+        Parameters
+        ----------
+        component : Component
+            The component to add.
+
+        Raises
+        ------
+        ValueError
+            If the agent already has a component of that type.
+        """
+        if type(component) in self.components.keys():
+            raise ValueError(f"Agent {self.id} already has a component of type {type(component)}.")
+        else:
+            self._components[type(component)] = component
+
+    def remove_class_component(self, component_type: type):
+        """Removes component of type ```component_type`` from the agent class.
+
+        Parameters:
+        component_type : type
+            Class of component to be removed from agent.
+
+        Raises
+        ------
+        ComponentNotFoundError
+            If agent does not have a component of class ``component_type``.
+        """
+        if component_type not in self.components.keys():
+            raise ComponentNotFoundError(self, component_type)
+        else:
+            del self._components[component_type]
+
+    def get_class_component(self, component_type: type, throw_error: bool = False):
+        """Gets a component that is the same type as ``component_type``.
+
+        Parameters
+        ----------
+        component_type : type
+            The type of component to search for.
+        throw_error : bool, Optional
+            Boolean that specifies whether a ``ComponentNotFoundError`` should be raised upon failing to find a
+            component of type ``component_type``. Defaults to ``False``.
+        Returns
+        -------
+        Component
+            A component object matching the class specified by ``component_type``.
+        None
+            Returns None if agent does not have a component of class ``component_type``.
+
+        Raises
+        ------
+        ComponentNotFoundError
+            If ``throw_error`` is ``True`` and no component matching ``component_type`` is found.
+        """
+        if component_type in self.components.keys():
+            return self._components[component_type]
+        elif throw_error:
+            raise ComponentNotFoundError(self, component_type)
+        else:
+            return None
+
+    def has_class_component(self, *args) -> bool:
+        """Returns a (True/False) bool if the agent class (does/does not) have the list of specified components.
+
+        The functions uses the ``*args`` so you can check for multiple components at once::
+
+            # Will return true if agent has a PositionComponent
+            agent.has_component(PositionComponent)
+
+            # Will return true if agent has both a PositionComponent and a RotationComponent
+            agent.has_component(PositionComponent, RotationComponent)
+
+        Parameters
+        ----------
+        args
+            The list of ``Component`` classes that will checked.
+
+        Returns
+        -------
+        bool
+            ``True`` if ``Agent`` has all of the components listed, else ``False``
+        """
+        for component in args:
+            if component not in self._components.keys():
+                return False
+        return True
+
+
+class Agent(object, metaclass=_MetaAgent):
     """This is the base class for Agent objects. Inherit from the class when creating custom agent types.
 
     In ECAgent, An ``Agent`` is the ``Entity`` in the Entity-Component-System (ECS) architecture.
 
     Attributes
     ----------
     components : dict
         The components associated with the environment. The key is the Class of the component.
     id : str
-        The agent id of the environment.
+        The agent's unique identifier.
     model : Model
         The ``Model`` the ``Agent`` belongs to.
     tag : int
-        The value of the Tag associated with the environment. Defaults to 0 (which is the value ``NONE``).
+        The value of the Tag associated with the ``Agent``. Defaults to 0 (which is the value ``NONE``) or the
+        default tag value of the Agent's metaclass.
     """
 
     __slots__ = ['id', 'model', 'components', 'tag']
 
-    def __init__(self, id: str, model: Model, tag: int = Tags.NONE):
+    def __init__(self, id: str, model: Model, tag: int = None):
         self.id = id
         self.model = model
         self.components = {}
-        self.tag = tag
+        self.tag = Agent.tag if tag is None else tag
 
     def __getitem__(self, item: type):
         """Wrapper for the ``Agent.get_component()`` function."""
         return self.get_component(item)
 
     def __len__(self) -> int:
         """Returns the number of components attached to a given agent."""
@@ -331,14 +503,67 @@
     def __init__(self, model: Model):
         self.timestep = 0
         self.systems = {}
         self.execution_queue = []
         self.component_pools = {}
         self.model = model
 
+    def __getitem__(self, item: Union[str, type]) -> Union[System, list, None]:
+        """Gets ``System`` with ``id == item`` or ``list`` of components whose ``type == item``.
+
+        This function returns a different result based on the type of ``item``::
+            # When arguments is of type str
+            sid = 'some_system_id'
+            model.systems[sid]  # Returns a System with id == sid
+            model.systems[sid, True] # will throw an error if no system id == sid
+
+            # When argument is of type type
+            # Returns a list of all CustomComponent objects in the model
+            model.systems[CustomComponent]
+            # Will throw an error if no CustomComponent objects exist
+            model.systems[CustomComponent, True]
+
+        Parameters
+        ----------
+        item : Union[str, type]
+            The ``id`` of the ``System`` being accessed or the type of ``Component`` you want to access.
+        throw_error : bool, Optional
+            Determines if the function should raise a ``KeyError`` when it cannot find a System with ``id == item``
+            or components of ``type == item``. Defaults to ``False``
+
+        Returns
+        -------
+        System
+            with ``id == item`` if ``item`` is of type ``str``.
+        list[Component]
+            with ``type == item`` if ``item`` is of type ``type``.
+        None
+            if no components of ``type == item`` exist.
+
+        Raises
+        ------
+        KeyError
+            If no ``System`` with ``id == item`` exists in the execution queue or no components of ``type == item``
+            exist in the component pool.
+        """
+        throw_error = False
+        if type(item) == tuple:
+            item, throw_error = item
+
+        # First check for system access:
+        if type(item) == str:
+            if item in self.systems:
+                return self.systems[item]
+            elif throw_error:
+                raise KeyError(f'Model does not have a System with id == {item}.')
+            else:
+                return None
+        else:
+            return self.get_components(item, throw_error=throw_error)
+
     def add_system(self, s: System):
         """Adds System s to the ``SystemManager`` and registers it with execution queue.
 
         Parameters
         ----------
         s : System
             The ``System`` being added to the ``SystemManager``
@@ -451,32 +676,42 @@
             raise KeyError(f"Cannot deregister Agent {component.agent.id}'s {str(type(component))} Component because "
                            f"it was never registered with the SystemManager to begin with.")
         else:
             self.component_pools[type(component)].remove(component)
             if len(self.component_pools[type(component)]) == 0:
                 del self.component_pools[type(component)]
 
-    def get_components(self, component_type: type):
+    def get_components(self, component_type: type, throw_error: bool = False):
         """Returns the list of components registered to the ``SystemManager`` with a type of ``component_type``.
         Returns ``None`` if there are no components of type ``component_type`` registered with the ``SystemManager``.
 
         Parameters
         ----------
         component_type : type
             The type of components you want to search for (e.g. ``PositionComponent``).
+        throw_error : bool, Optional
+            Determines if the function should raise a ``KeyError`` when it cannot find components of
+            ``type == component_type``. Defaults to ``False``
 
         Returns
         -------
         list
             Of components with type ``component_type``.
         None
             If no components of type ``component_type`` can be found.
+
+        Raises
+        ------
+        KeyError
+            If ``throw_error = True`` and no components of ``type == component_type`` are found.
         """
         if component_type in self.component_pools.keys():
             return self.component_pools[component_type]
+        elif throw_error:
+            raise KeyError(f'No Components of type {component_type} could be found.')
         else:
             return None
 
     @deprecated(reason='For not meeting standard python naming conventions. Use "get_components" instead.')
     def getComponents(self, component_type: type):  # pragma: no cover
         """Deprecated. Use ``get_components`` instead."""
         return self.get_components(component_type)
```

### Comparing `ECAgent-0.5.4/ECAgent/Decode.py` & `ECAgent-0.5.5/ECAgent/Decode.py`

 * *Files identical despite different names*

### Comparing `ECAgent-0.5.4/ECAgent/Environments.py` & `ECAgent-0.5.5/ECAgent/Environments.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,18 +49,23 @@
 
     def __init__(self, agent, model, x: float = 0.0, y: float = 0.0, z: float = 0.0) -> None:
         super().__init__(agent, model)
         self.x = x
         self.y = y
         self.z = z
 
-    def getPosition(self) -> (float, float, float):
+    def get_position(self) -> (float, float, float):
         """Returns the x,y and z values of the component as a tuple"""
         return self.x, self.y, self.z
 
+    @deprecated(reason='For not meeting standard python naming conventions. Use "get_position()" instead.')
+    def getPosition(self) -> (float, float, float):  # pragma: no cover
+        """Deprecated. Use ``get_position()`` instead."""
+        return self.get_position()
+
     def xy(self):
         """Returns the x and y values of the component as a 2-tuple.
         """
         return self.x, self.y
 
     def xz(self):
         """Returns the x and z values of the component as a 2-tuple.
@@ -71,17 +76,17 @@
         """Returns the y and z values of the component as a 2-tuple.
         """
         return self.y, self.z
 
     def xyz(self):
         """Returns the x, y and z values of the component as a 3-tuple.
 
-        Equivalent to ``PositionComponent.getPosition()``
+        Equivalent to ``PositionComponent.get_position()``
         """
-        return self.getPosition()
+        return self.get_position()
 
 
 def distance(a: PositionComponent, b: PositionComponent) -> float:
     """Calculates the distance from ``PositionComponent`` a to ``PositionComponent`` b.
 
     Parameters
     ----------
```

### Comparing `ECAgent-0.5.4/ECAgent/Tags.py` & `ECAgent-0.5.5/ECAgent/Tags.py`

 * *Files 5% similar despite different names*

```diff
@@ -142,14 +142,25 @@
             If the tag cannot be found.
         """
         if tag_id < 0 or tag_id > self._tag_counter - 1:
             raise TagNotFoundError(tag_id)
         else:
             return self._tag_names[tag_id]
 
+    def itemize(self) -> list:
+        """Returns a ``list`` of tags in the ``TagLibrary`` and their values.
+
+        Returns
+        -------
+        list
+            In the following form: ``[('NONE', 0), ('TAG1', 1),..., ('TAGN', N)]``
+
+        """
+        return [(key, val) for val, key in enumerate(self._tag_names)]
+
 
 class DuplicateTagError(Exception):
     """Exception raised when a duplicate Tag is created.
 
     Attributes:
     -----------
     tag_name : str
@@ -232,21 +243,33 @@
     TagNotFoundError
         If the tag cannot be found.
     """
     return _module_library.get_tag_name(tag_id)
 
 
 def __getattr__(tag_name: str) -> int:
-    """Returns
+    """Returns the value of a tag with a matching ``tag_name`` in the global ``TagLibrary``
     ----------
     int
         The unique id for a tag with a ``name == tag_name``.
 
     Raises
     ------
     TagNotFoundError
         If tag does not exist.
     """
     if tag_name not in _module_library.__dict__:
         raise TagNotFoundError(tag_name)
     else:
         return _module_library.__dict__[tag_name]
+
+
+def itemize() -> list:
+    """Returns a ``list`` of tags in the global ``TagLibrary`` and their values.
+
+    Returns
+    -------
+    list
+        In the following form: ``[('NONE', 0), ('TAG1', 1),..., ('TAGN', N)]``
+
+    """
+    return _module_library.itemize()
```

### Comparing `ECAgent-0.5.4/ECAgent/Visualization.py` & `ECAgent-0.5.5/ECAgent/Visualization.py`

 * *Files identical despite different names*

### Comparing `ECAgent-0.5.4/ECAgent.egg-info/PKG-INFO` & `ECAgent-0.5.5/ECAgent.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECAgent
-Version: 0.5.4
+Version: 0.5.5
 Summary: An Agent-based Modelling framework based on the Entity-Component-System architectural pattern.
 Home-page: https://github.com/BrandonGower-Winter/ECAgent
 Author: Brandon Gower-Winter
 Author-email: brandongowerwinter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,20 @@
 # ECAgent - ECS for ABM
 ![Build](https://github.com/BrandonGower-Winter/ABMECS/workflows/Build/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/ecagent/badge/?version=latest)](https://ecagent.readthedocs.io/en/latest/?badge=latest)
 
 An Agent-based Modelling framework based on the Entity-Component-System architectural pattern.
 
 The readme is still WIP but code documentation can be found at: https://ecagent.readthedocs.io/en/latest/
+
+## Installing ECAgent
+
+You can install ECAgent using:
+```bash
+pip install ECAgent
+```
+
+## Developing for ECAgent
+
+* Clone the Repo.
+* Build the virtual environment using `make`
+* Activate the virtual environment using `source ./venv/bin/activate`
```

### Comparing `ECAgent-0.5.4/LICENSE` & `ECAgent-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ECAgent-0.5.4/PKG-INFO` & `ECAgent-0.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ECAgent
-Version: 0.5.4
+Version: 0.5.5
 Summary: An Agent-based Modelling framework based on the Entity-Component-System architectural pattern.
 Home-page: https://github.com/BrandonGower-Winter/ECAgent
 Author: Brandon Gower-Winter
 Author-email: brandongowerwinter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,7 +15,20 @@
 # ECAgent - ECS for ABM
 ![Build](https://github.com/BrandonGower-Winter/ABMECS/workflows/Build/badge.svg) 
 [![Documentation Status](https://readthedocs.org/projects/ecagent/badge/?version=latest)](https://ecagent.readthedocs.io/en/latest/?badge=latest)
 
 An Agent-based Modelling framework based on the Entity-Component-System architectural pattern.
 
 The readme is still WIP but code documentation can be found at: https://ecagent.readthedocs.io/en/latest/
+
+## Installing ECAgent
+
+You can install ECAgent using:
+```bash
+pip install ECAgent
+```
+
+## Developing for ECAgent
+
+* Clone the Repo.
+* Build the virtual environment using `make`
+* Activate the virtual environment using `source ./venv/bin/activate`
```

