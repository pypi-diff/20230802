# Comparing `tmp/habitat-lab-0.2.520230729.tar.gz` & `tmp/habitat-lab-0.2.520230802.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habitat-lab-0.2.520230729.tar", last modified: Sat Jul 29 05:48:26 2023, max compression
+gzip compressed data, was "habitat-lab-0.2.520230802.tar", last modified: Wed Aug  2 17:22:57 2023, max compression
```

## Comparing `habitat-lab-0.2.520230729.tar` & `habitat-lab-0.2.520230802.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      210 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/PKG-INFO
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      887 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9687 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      968 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10558 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_base.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3007 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_interface.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      341 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5425 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/kinematic_humanoid.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18684 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/manipulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6693 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/mobile_manipulator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      634 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4655 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_suction.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1372 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/franka_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7298 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/spot_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/robots/stretch_robot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3802 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/articulated_agents/static_manipulator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20023 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/CONFIG_KEYS.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16816 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      384 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/benchmark/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      435 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_rgbonly_mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      355 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      353 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/imagenav/imagenav_test.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      773 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      904 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      774 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      926 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      754 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.142837 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      537 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      354 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      360 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_habitat_test.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/nav/vln_r2r.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      954 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1350 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1116 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle_single_camera.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1353 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/interact.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      939 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/nav_to_obj.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      951 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      950 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/pick.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/place.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      976 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1189 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_human.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2115 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_spot.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1605 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_stretch.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      802 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/reach_state.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1011 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1746 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4838 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/default.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74397 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/default_structured_configs.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      223 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/eqa/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/imagenav/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/hm3d_v1.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/instance_imagenav/hm3d_v2.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/hssd-hab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/mp3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/objectnav/procthor-hab.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson_0_plus.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/gibson_v2.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/habitat_test.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/hm3d.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/pointnav/mp3d.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/rearrangement/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/rearrangement/replica_cad.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.146839 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      225 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/dataset/vln/mp3d_r2r.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.134834 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.150841 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      148 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      163 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      249 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/depth_head_agent_vis.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      142 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgb_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgb_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      217 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_rgbd_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbd_head_rgbdp_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbdp_head_rgbd_arm_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      298 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/rgbds_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/simulator/agents/semantic_agent.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.150841 habitat-lab-0.2.520230729/habitat/config/habitat/task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      255 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/eqa.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      392 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/imagenav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      748 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/instance_imagenav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      648 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/objectnav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      415 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/pointnav.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/pointnav_franka.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      147 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/fetch_arm.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/agents/fetch_base_arm.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      960 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_fridge.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      246 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/idle.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      314 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/demo/interact.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      900 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/nav_to_obj.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_cab.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1243 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_fridge.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2185 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      442 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      583 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3503 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      916 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pick.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1003 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/place.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play_human.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      672 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/reach_state.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1245 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1223 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1727 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1160 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1076 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/habitat/task/vln_r2r.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1070 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/config/read_write.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/core/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1221 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/agent.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/core/batch_rendering/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18384 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/env_batch_renderer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      330 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/batch_rendering/env_batch_renderer_constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5737 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/benchmark.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      654 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/challenge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19851 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13582 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/embodied_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16056 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/env.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3978 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/environments.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7153 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/registry.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13195 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/simulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/spaces.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5604 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23512 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/core/vector_env.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/datasets/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.154842 habitat-lab-0.2.520230729/habitat/datasets/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      733 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/eqa/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3974 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/eqa/mp3d_eqa_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/image_nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/image_nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3100 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/image_nav/instance_image_nav_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/object_nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/object_nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5664 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/object_nav/object_nav_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/pointnav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1220 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7361 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_generator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.158844 habitat-lab-0.2.520230729/habitat/datasets/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1232 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/combine_datasets.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4250 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/all_receptacles.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3171 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/bench_config.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2132 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/empty.yaml
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6455 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5721 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4326 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4605 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/set_table.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2831 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/tidy_house.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2504 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_drawer.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_fridge.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2369 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/test_config.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1077 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/generate_episode_inits.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3450 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_dataset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43253 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_generator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16486 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/run_episode_generator.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      756 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9654 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/art_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23653 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3987 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_target_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39034 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/receptacle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1154 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/scene_sampler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/datasets/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/vln/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2482 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/datasets/vln/r2r_vln_dataset.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/gym/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4757 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_definitions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1887 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_env_episode_count_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1591 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_env_obs_dict_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12898 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/gym/gym_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/py.typed
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.198860 habitat-lab-0.2.520230729/habitat/sims/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      267 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      711 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2517 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20974 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/debug_visualizer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26504 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/habitat_simulator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12514 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/sim_utilities.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/sims/pyrobot/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      785 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/pyrobot/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8884 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/pyrobot/pyrobot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      721 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/sims/registration.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/eqa/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/eqa/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6173 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/eqa/eqa.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/nav/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      670 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/instance_image_nav_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    46959 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/nav.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6714 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/object_nav_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3276 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/nav/shortest_path_follower.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/rearrange/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1400 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.202862 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27870 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1722 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/articulated_agent_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/grip_actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8828 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/oracle_nav_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/pddl_actions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7368 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/articulated_agent_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1541 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/marker_info.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9441 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2465 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_task.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9792 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9255 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_action.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26009 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4432 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4749 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_predicate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19506 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_sim_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7259 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/rearrange_pddl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2825 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/task_creator_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/policy_modules.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13238 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_grasp_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32786 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37631 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sim.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13425 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_task.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12483 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9450 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9023 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5200 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6174 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3794 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5547 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1329 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3982 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_sensors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17755 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/rearrange/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      875 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/registration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1723 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/tasks/vln/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/vln/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/tasks/vln/vln.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.206863 habitat-lab-0.2.520230729/habitat/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2477 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1244 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/env_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5446 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/geometry_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/pickle5_multiprocessing.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2096 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/profiling_wrapper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1082 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/test_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat/utils/visualizations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      288 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.138836 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5616 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4240 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/fog_of_war.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15090 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/maps.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11969 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/utils/visualizations/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/habitat/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/habitat_lab.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12658 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      253 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2023-07-29 05:48:26.000000 habitat-lab-0.2.520230729/habitat_lab.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      338 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/requirements.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-07-29 05:48:26.210865 habitat-lab-0.2.520230729/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4530 2023-07-29 05:48:00.000000 habitat-lab-0.2.520230729/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      210 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/PKG-INFO
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.381487 habitat-lab-0.2.520230802/habitat/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      887 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.381487 habitat-lab-0.2.520230802/habitat/articulated_agent_controllers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agent_controllers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9687 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.385487 habitat-lab-0.2.520230802/habitat/articulated_agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      968 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10558 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/articulated_agent_base.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3007 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/articulated_agent_interface.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.385487 habitat-lab-0.2.520230802/habitat/articulated_agents/humanoids/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      341 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/humanoids/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5425 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/humanoids/kinematic_humanoid.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18684 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/manipulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6693 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/mobile_manipulator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.385487 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      634 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4655 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/fetch_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      651 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/fetch_suction.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1372 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/franka_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7298 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/spot_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3053 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/robots/stretch_robot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3802 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/articulated_agents/static_manipulator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.385487 habitat-lab-0.2.520230802/habitat/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20023 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/CONFIG_KEYS.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16816 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      384 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.377486 habitat-lab-0.2.520230802/habitat/config/benchmark/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.385487 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/eqa_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      435 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/eqa_rgbonly_mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.389487 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/imagenav/imagenav_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      355 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/imagenav/imagenav_gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      353 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/imagenav/imagenav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/imagenav/imagenav_test.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.389487 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/instance_imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.389487 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      773 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      904 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      732 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      774 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      926 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      754 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.389487 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      537 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      354 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      360 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_habitat_test.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/nav/vln_r2r.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.389487 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/close_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      954 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/close_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1350 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/idle.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1116 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/idle_single_camera.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1353 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/interact.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      939 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/nav_to_obj.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/open_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      951 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/open_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      950 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/pick.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      946 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/place.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      976 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1189 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_human.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2115 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_spot.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1605 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_stretch.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      802 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/reach_state.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1011 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1034 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1746 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4838 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/default.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74397 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/default_structured_configs.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.377486 habitat-lab-0.2.520230802/habitat/config/habitat/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.377486 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      223 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/eqa/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/imagenav/gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/imagenav/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/instance_imagenav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/instance_imagenav/hm3d_v1.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      208 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/instance_imagenav/hm3d_v2.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/objectnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/objectnav/hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/objectnav/hssd-hab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      192 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/objectnav/mp3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/objectnav/procthor-hab.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/gibson.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/gibson_0_plus.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/gibson_v2.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/habitat_test.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/hm3d.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      191 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/pointnav/mp3d.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/rearrangement/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      272 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/rearrangement/replica_cad.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      225 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/dataset/vln/mp3d_r2r.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.377486 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      148 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/depth_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      163 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/depth_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      249 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/depth_head_agent_vis.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      142 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgb_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgb_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      217 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbd_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      241 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbd_head_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbd_head_rgbd_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbd_head_rgbdp_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbdp_head_rgbd_arm_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      298 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/rgbds_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/simulator/agents/semantic_agent.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.393488 habitat-lab-0.2.520230802/habitat/config/habitat/task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      255 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/eqa.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      392 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/imagenav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      748 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/instance_imagenav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      648 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/objectnav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      415 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/pointnav.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/pointnav_franka.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/agents/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      147 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/agents/fetch_arm.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/agents/fetch_base_arm.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      960 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/close_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      980 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/close_fridge.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/demo/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      246 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/demo/idle.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      314 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/demo/interact.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      900 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/nav_to_obj.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/open_cab.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1243 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/open_fridge.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2185 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      442 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      583 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3503 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      916 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pick.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1003 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/place.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/play.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/play_human.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      672 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/reach_state.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1245 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1223 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1727 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1160 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1076 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      240 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/habitat/task/vln_r2r.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1070 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/config/read_write.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/core/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1221 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/agent.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.397488 habitat-lab-0.2.520230802/habitat/core/batch_rendering/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/batch_rendering/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18384 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/batch_rendering/env_batch_renderer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      330 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/batch_rendering/env_batch_renderer_constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5737 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/benchmark.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      654 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/challenge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19851 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13582 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/embodied_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16056 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/env.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3978 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/environments.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1205 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7153 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/registry.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13195 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/simulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/spaces.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5604 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23512 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/core/vector_env.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      733 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/eqa/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3974 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/eqa/mp3d_eqa_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/image_nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1263 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/image_nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3100 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/image_nav/instance_image_nav_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/object_nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1228 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/object_nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5664 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/object_nav/object_nav_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/pointnav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1220 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/pointnav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/pointnav/pointnav_dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7361 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/pointnav/pointnav_generator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.401488 habitat-lab-0.2.520230802/habitat/datasets/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1232 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/combine_datasets.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4250 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/all_receptacles.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3171 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/bench_config.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2132 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/empty.yaml
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6455 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5721 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/rearrange.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4326 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4605 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/set_table.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2831 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/tidy_house.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2504 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/in_drawer.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/in_fridge.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2369 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/test_config.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1077 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/generate_episode_inits.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3450 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/rearrange_dataset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44172 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/rearrange_generator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16848 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/run_episode_generator.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      756 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9654 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/art_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23653 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/object_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3987 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/object_target_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39034 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/receptacle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1154 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/scene_sampler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/datasets/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/vln/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2482 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/datasets/vln/r2r_vln_dataset.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/gym/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      304 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/gym/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4757 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/gym/gym_definitions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1887 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/gym/gym_env_episode_count_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1591 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/gym/gym_env_obs_dict_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12898 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/gym/gym_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       79 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/py.typed
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/sims/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      267 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      711 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2517 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20974 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/debug_visualizer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26504 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/habitat_simulator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12514 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/sim_utilities.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/sims/pyrobot/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      785 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/pyrobot/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8884 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/pyrobot/pyrobot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      721 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/sims/registration.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/tasks/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.429490 habitat-lab-0.2.520230802/habitat/tasks/eqa/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/eqa/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6173 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/eqa/eqa.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.433490 habitat-lab-0.2.520230802/habitat/tasks/nav/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      670 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/nav/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/nav/instance_image_nav_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    46959 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/nav/nav.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6714 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/nav/object_nav_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3276 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/nav/shortest_path_follower.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.433490 habitat-lab-0.2.520230802/habitat/tasks/rearrange/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1400 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.433490 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27870 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1722 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/articulated_agent_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11263 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/grip_actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8828 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/oracle_nav_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/pddl_actions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7368 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/articulated_agent_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1541 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/marker_info.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.433490 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9441 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/composite_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2465 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/composite_task.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.433490 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/domain_configs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9792 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9255 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_action.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26009 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4432 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4749 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_predicate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19506 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_sim_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7259 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/rearrange_pddl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2825 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/task_creator_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/policy_modules.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13238 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_grasp_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32786 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37631 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_sim.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13425 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_task.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      181 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12483 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9450 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9023 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5200 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6174 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/pick_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3794 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/pick_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5547 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/place_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1329 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/place_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3982 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/reach_sensors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/reach_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17755 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/rearrange/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      875 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/registration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1723 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat/tasks/vln/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/vln/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3157 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/tasks/vln/vln.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2477 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1244 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/env_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5446 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/geometry_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/pickle5_multiprocessing.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2096 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/profiling_wrapper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1082 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/test_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat/utils/visualizations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      288 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/visualizations/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.381487 habitat-lab-0.2.520230802/habitat/utils/visualizations/assets/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5616 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4240 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/visualizations/fog_of_war.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15090 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/visualizations/maps.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11969 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/utils/visualizations/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/habitat/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/habitat_lab.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2023-08-02 17:22:57.000000 habitat-lab-0.2.520230802/habitat_lab.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12658 2023-08-02 17:22:57.000000 habitat-lab-0.2.520230802/habitat_lab.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 17:22:57.000000 habitat-lab-0.2.520230802/habitat_lab.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      253 2023-08-02 17:22:57.000000 habitat-lab-0.2.520230802/habitat_lab.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        8 2023-08-02 17:22:57.000000 habitat-lab-0.2.520230802/habitat_lab.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      338 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/requirements.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       46 2023-08-02 17:22:57.437491 habitat-lab-0.2.520230802/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4530 2023-08-02 17:22:34.000000 habitat-lab-0.2.520230802/setup.py
```

### Comparing `habitat-lab-0.2.520230729/PKG-INFO` & `habitat-lab-0.2.520230802/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-lab
-Version: 0.2.520230729
+Version: 0.2.520230802
 Summary: Habitat-Lab: a modular high-level library for end-to-end development in Embodied AI.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-lab-0.2.520230729/habitat/__init__.py` & `habitat-lab-0.2.520230802/habitat/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py` & `habitat-lab-0.2.520230802/habitat/articulated_agent_controllers/humanoid_rearrange_controller.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/__init__.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_base.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/articulated_agent_base.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/articulated_agent_interface.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/articulated_agent_interface.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/humanoids/kinematic_humanoid.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/humanoids/kinematic_humanoid.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/manipulator.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/mobile_manipulator.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/mobile_manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/__init__.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_robot.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/fetch_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/fetch_suction.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/fetch_suction.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/franka_robot.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/franka_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/spot_robot.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/spot_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/robots/stretch_robot.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/robots/stretch_robot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/articulated_agents/static_manipulator.py` & `habitat-lab-0.2.520230802/habitat/articulated_agents/static_manipulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/CONFIG_KEYS.md` & `habitat-lab-0.2.520230802/habitat/config/CONFIG_KEYS.md`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/README.md` & `habitat-lab-0.2.520230802/habitat/config/README.md`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/eqa_mp3d.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/eqa_mp3d.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v1.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/instance_imagenav/instance_imagenav_hm3d_v2.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hm3d.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hm3d_with_semantic.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_hssd-hab_with_semantic.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_mp3d.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_mp3d_with_semantic.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/objectnav/objectnav_procthor-hab_with_semantic.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/pointnav/pointnav_franka.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/nav/vln_r2r.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/nav/vln_r2r.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_cab.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/close_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/close_fridge.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/close_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/idle.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/idle_single_camera.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/idle_single_camera.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/interact.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/interact.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/nav_to_obj.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/nav_to_obj.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_cab.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/open_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/open_fridge.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/open_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/pick.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/pick.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/place.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/place.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_human.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_human.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_spot.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_spot.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/play_stretch.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/play_stretch.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/prepare_groceries.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/reach_state.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/reach_state.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/rearrange_easy_multi_agent.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/set_table.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/benchmark/rearrange/tidy_house.yaml` & `habitat-lab-0.2.520230802/habitat/config/benchmark/rearrange/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/default.py` & `habitat-lab-0.2.520230802/habitat/config/default.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/default_structured_configs.py` & `habitat-lab-0.2.520230802/habitat/config/default_structured_configs.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/instance_imagenav.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/instance_imagenav.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/objectnav.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/objectnav.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_cab.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/close_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/close_fridge.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/close_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/nav_to_obj.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/nav_to_obj.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_cab.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/open_cab.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/open_fridge.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/open_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/set_table.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pddl/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/pick.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/pick.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/place.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/place.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/play.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/play_human.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/play_human.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/prepare_groceries.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/reach_state.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/reach_state.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange_easy_base.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/rearrange_easy_multi_agent.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/set_table.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/habitat/task/rearrange/tidy_house.yaml` & `habitat-lab-0.2.520230802/habitat/config/habitat/task/rearrange/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/config/read_write.py` & `habitat-lab-0.2.520230802/habitat/config/read_write.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/agent.py` & `habitat-lab-0.2.520230802/habitat/core/agent.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/batch_rendering/env_batch_renderer.py` & `habitat-lab-0.2.520230802/habitat/core/batch_rendering/env_batch_renderer.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/benchmark.py` & `habitat-lab-0.2.520230802/habitat/core/benchmark.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/challenge.py` & `habitat-lab-0.2.520230802/habitat/core/challenge.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/dataset.py` & `habitat-lab-0.2.520230802/habitat/core/dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/embodied_task.py` & `habitat-lab-0.2.520230802/habitat/core/embodied_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/env.py` & `habitat-lab-0.2.520230802/habitat/core/env.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/environments.py` & `habitat-lab-0.2.520230802/habitat/core/environments.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/logging.py` & `habitat-lab-0.2.520230802/habitat/core/logging.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/registry.py` & `habitat-lab-0.2.520230802/habitat/core/registry.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/simulator.py` & `habitat-lab-0.2.520230802/habitat/core/simulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/spaces.py` & `habitat-lab-0.2.520230802/habitat/core/spaces.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/utils.py` & `habitat-lab-0.2.520230802/habitat/core/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/core/vector_env.py` & `habitat-lab-0.2.520230802/habitat/core/vector_env.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/eqa/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/eqa/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/eqa/mp3d_eqa_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/eqa/mp3d_eqa_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/image_nav/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/image_nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/image_nav/instance_image_nav_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/image_nav/instance_image_nav_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/object_nav/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/object_nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/object_nav/object_nav_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/object_nav/object_nav_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/pointnav/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/pointnav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/pointnav/pointnav_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/pointnav/pointnav_generator.py` & `habitat-lab-0.2.520230802/habitat/datasets/pointnav/pointnav_generator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/combine_datasets.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/combine_datasets.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/all_receptacles.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/all_receptacles.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/bench_config.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/bench_config.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/empty.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/empty.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/prepare_groceries.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/rearrange.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/rearrange_easy.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/set_table.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/set_table.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/hab/tidy_house.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/hab/tidy_house.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_drawer.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/in_drawer.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/in_fridge.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/in_fridge.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/configs/test_config.yaml` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/configs/test_config.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/generate_episode_inits.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/generate_episode_inits.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/rearrange_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/rearrange_generator.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/rearrange_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,29 +210,37 @@
                 if len(object_handles) == 0:
                     raise ValueError(
                         f"Found no object handles for {obj_sampler_info}"
                     )
                 self._obj_samplers[
                     obj_sampler_info["name"]
                 ] = samplers.ObjectSampler(
-                    object_handles,
-                    obj_sampler_info["params"]["receptacle_sets"],
-                    (
+                    object_set=object_handles,
+                    allowed_recep_set_names=obj_sampler_info["params"][
+                        "receptacle_sets"
+                    ],
+                    num_objects=(
                         obj_sampler_info["params"]["num_samples"][0],
                         obj_sampler_info["params"]["num_samples"][1],
                     ),
-                    obj_sampler_info["params"]["orientation_sampling"],
-                    get_sample_region_ratios(obj_sampler_info),
-                    obj_sampler_info["params"].get(
+                    orientation_sample=obj_sampler_info["params"][
+                        "orientation_sampling"
+                    ],
+                    sample_region_ratio=get_sample_region_ratios(
+                        obj_sampler_info
+                    ),
+                    nav_to_min_distance=obj_sampler_info["params"].get(
                         "nav_to_min_distance", -1.0
                     ),
-                    obj_sampler_info["params"].get("sample_probs", None),
-                    obj_sampler_info["params"].get(
-                        "constrain_to_largest_nav_island", False
+                    recep_set_sample_probs=obj_sampler_info["params"].get(
+                        "sample_probs", None
                     ),
+                    constrain_to_largest_nav_island=obj_sampler_info[
+                        "params"
+                    ].get("constrain_to_largest_nav_island", False),
                 )
             else:
                 logger.info(
                     f"Requested object sampler '{obj_sampler_info['type']}' is not implemented."
                 )
                 raise (NotImplementedError)
 
@@ -252,25 +260,37 @@
             if target_sampler_info["type"] == "uniform":
                 # merge and flatten receptacle sets
 
                 self._target_samplers[
                     target_sampler_info["name"]
                 ] = samplers.ObjectTargetSampler(
                     # Add object set later
-                    [],
-                    target_sampler_info["params"]["receptacle_sets"],
-                    (
+                    object_instance_set=[],
+                    allowed_recep_set_names=target_sampler_info["params"][
+                        "receptacle_sets"
+                    ],
+                    num_objects=(
                         target_sampler_info["params"]["num_samples"][0],
                         target_sampler_info["params"]["num_samples"][1],
                     ),
-                    target_sampler_info["params"]["orientation_sampling"],
-                    get_sample_region_ratios(target_sampler_info),
-                    target_sampler_info["params"].get(
+                    orientation_sample=target_sampler_info["params"][
+                        "orientation_sampling"
+                    ],
+                    sample_region_ratio=get_sample_region_ratios(
+                        target_sampler_info
+                    ),
+                    nav_to_min_distance=target_sampler_info["params"].get(
                         "nav_to_min_distance", -1.0
                     ),
+                    recep_set_sample_probs=target_sampler_info["params"].get(
+                        "sample_probs", None
+                    ),
+                    constrain_to_largest_nav_island=target_sampler_info[
+                        "params"
+                    ].get("constrain_to_largest_nav_island", False),
                 )
             else:
                 logger.info(
                     f"Requested target sampler '{target_sampler_info['type']}' is not implemented."
                 )
                 raise (NotImplementedError)
```

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/run_episode_generator.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/run_episode_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,17 @@
     # Define the desired object target sampling (i.e., where should an existing object be moved to)
     object_target_samplers: List[Any] = field(default_factory=list)
     # {"name":str, "type:str", "params":{})
     # - uniform target sampler params:
     # {"object_samplers":[str], "receptacle_sets":[str], "num_samples":[min, max], "orientation_sampling":str)
     # NOTE: random instances are chosen from the specified, previously excecuted object sampler up to the maximum number specified in params.
     # NOTE: previous samplers referenced must have: combined minimum samples >= minimum requested targets
+    # NOTE: "orientation_sampling" options: "none", "up", "all"
+    # NOTE: (optional) "constrain_to_largest_nav_island" (default False): if True, valid placements must snap to the largest navmesh island
+    # NOTE: (optional) "nav_to_min_distance" (default -1): if not -1, valid placements must snap to the navmesh with horizontal distance less than this value
     # {
     #     "name": "any_one_target",
     #     "type": "uniform",
     #     "params": {
     #         "object_samplers": ["any_one"],
     #         "receptacle_sets": ["any"],
     #         "num_samples": [1, 1],
```

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/art_sampler.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/art_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_sampler.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/object_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/object_target_sampler.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/object_target_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/receptacle.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/receptacle.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/rearrange/samplers/scene_sampler.py` & `habitat-lab-0.2.520230802/habitat/datasets/rearrange/samplers/scene_sampler.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/registration.py` & `habitat-lab-0.2.520230802/habitat/datasets/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/utils.py` & `habitat-lab-0.2.520230802/habitat/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/vln/__init__.py` & `habitat-lab-0.2.520230802/habitat/datasets/vln/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/datasets/vln/r2r_vln_dataset.py` & `habitat-lab-0.2.520230802/habitat/datasets/vln/r2r_vln_dataset.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/gym/gym_definitions.py` & `habitat-lab-0.2.520230802/habitat/gym/gym_definitions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/gym/gym_env_episode_count_wrapper.py` & `habitat-lab-0.2.520230802/habitat/gym/gym_env_episode_count_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/gym/gym_env_obs_dict_wrapper.py` & `habitat-lab-0.2.520230802/habitat/gym/gym_env_obs_dict_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/gym/gym_wrapper.py` & `habitat-lab-0.2.520230802/habitat/gym/gym_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/__init__.py` & `habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/actions.py` & `habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/actions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/debug_visualizer.py` & `habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/debug_visualizer.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/habitat_simulator.py` & `habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/habitat_simulator.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/habitat_simulator/sim_utilities.py` & `habitat-lab-0.2.520230802/habitat/sims/habitat_simulator/sim_utilities.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/pyrobot/__init__.py` & `habitat-lab-0.2.520230802/habitat/sims/pyrobot/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/pyrobot/pyrobot.py` & `habitat-lab-0.2.520230802/habitat/sims/pyrobot/pyrobot.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/sims/registration.py` & `habitat-lab-0.2.520230802/habitat/sims/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/eqa/__init__.py` & `habitat-lab-0.2.520230802/habitat/tasks/eqa/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/eqa/eqa.py` & `habitat-lab-0.2.520230802/habitat/tasks/eqa/eqa.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/nav/__init__.py` & `habitat-lab-0.2.520230802/habitat/tasks/nav/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/nav/instance_image_nav_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/nav/instance_image_nav_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/nav/nav.py` & `habitat-lab-0.2.520230802/habitat/tasks/nav/nav.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/nav/object_nav_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/nav/object_nav_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/nav/shortest_path_follower.py` & `habitat-lab-0.2.520230802/habitat/tasks/nav/shortest_path_follower.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/__init__.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/actions.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/actions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/articulated_agent_action.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/articulated_agent_action.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/grip_actions.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/grip_actions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/oracle_nav_action.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/oracle_nav_action.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/actions/pddl_actions.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/actions/pddl_actions.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/articulated_agent_manager.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/articulated_agent_manager.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/marker_info.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/marker_info.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/composite_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/composite_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/composite_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/domain_configs/replica_cad.yaml`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_action.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_action.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_domain.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_domain.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_logical_expr.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_predicate.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_predicate.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/pddl_sim_state.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/pddl_sim_state.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/rearrange_pddl.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/rearrange_pddl.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/multi_task/task_creator_utils.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/multi_task/task_creator_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_grasp_manager.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_grasp_manager.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_sim.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_sim.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/rearrange_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/rearrange_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/articulated_object_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/articulated_object_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/nav_to_obj_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/nav_to_obj_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/pick_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/pick_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/pick_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/place_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/place_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/place_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_sensors.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/reach_sensors.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/sub_tasks/reach_task.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/sub_tasks/reach_task.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/rearrange/utils.py` & `habitat-lab-0.2.520230802/habitat/tasks/rearrange/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/registration.py` & `habitat-lab-0.2.520230802/habitat/tasks/registration.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/utils.py` & `habitat-lab-0.2.520230802/habitat/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/vln/__init__.py` & `habitat-lab-0.2.520230802/habitat/tasks/vln/__init__.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/tasks/vln/vln.py` & `habitat-lab-0.2.520230802/habitat/tasks/vln/vln.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/common.py` & `habitat-lab-0.2.520230802/habitat/utils/common.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/env_utils.py` & `habitat-lab-0.2.520230802/habitat/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/geometry_utils.py` & `habitat-lab-0.2.520230802/habitat/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/pickle5_multiprocessing.py` & `habitat-lab-0.2.520230802/habitat/utils/pickle5_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/profiling_wrapper.py` & `habitat-lab-0.2.520230802/habitat/utils/profiling_wrapper.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/test_utils.py` & `habitat-lab-0.2.520230802/habitat/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png` & `habitat-lab-0.2.520230802/habitat/utils/visualizations/assets/maps_topdown_agent_sprite/100x100.png`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/visualizations/fog_of_war.py` & `habitat-lab-0.2.520230802/habitat/utils/visualizations/fog_of_war.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/visualizations/maps.py` & `habitat-lab-0.2.520230802/habitat/utils/visualizations/maps.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat/utils/visualizations/utils.py` & `habitat-lab-0.2.520230802/habitat/utils/visualizations/utils.py`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/habitat_lab.egg-info/PKG-INFO` & `habitat-lab-0.2.520230802/habitat_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habitat-lab
-Version: 0.2.520230729
+Version: 0.2.520230802
 Summary: Habitat-Lab: a modular high-level library for end-to-end development in Embodied AI.
 Home-page: https://aihabitat.org
 Author: Meta AI Research
 License: MIT License
 Project-URL: GitHub repo, https://github.com/facebookresearch/habitat-lab/
 Project-URL: Bug Tracker, https://github.com/facebookresearch/habitat-lab/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `habitat-lab-0.2.520230729/habitat_lab.egg-info/SOURCES.txt` & `habitat-lab-0.2.520230802/habitat_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `habitat-lab-0.2.520230729/setup.py` & `habitat-lab-0.2.520230802/setup.py`

 * *Files identical despite different names*

