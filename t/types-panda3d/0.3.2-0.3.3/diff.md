# Comparing `tmp/types-panda3d-0.3.2.tar.gz` & `tmp/types-panda3d-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-panda3d-0.3.2.tar", last modified: Sun Feb 19 00:11:59 2023, max compression
+gzip compressed data, was "types-panda3d-0.3.3.tar", last modified: Sat Jul  8 17:02:58 2023, max compression
```

## Comparing `types-panda3d-0.3.2.tar` & `types-panda3d-0.3.3.tar`

### file list

```diff
@@ -1,466 +1,466 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.652114 types-panda3d-0.3.2/
--rw-rw-rw-   0        0        0     1076 2022-08-03 23:48:00.000000 types-panda3d-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     2606 2023-02-19 00:11:59.651447 types-panda3d-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      848 2022-10-30 20:43:52.000000 types-panda3d-0.3.2/README.md
--rw-rw-rw-   0        0        0     1451 2023-02-18 03:43:09.000000 types-panda3d-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-19 00:11:59.652114 types-panda3d-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.055763 types-panda3d-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.063445 types-panda3d-0.3.2/src/direct-stubs/
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:15.000000 types-panda3d-0.3.2/src/direct-stubs/__init__.pyi
--rw-rw-rw-   0        0        0      657 2023-02-07 02:20:06.000000 types-panda3d-0.3.2/src/direct-stubs/_typing.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.067412 types-panda3d-0.3.2/src/direct-stubs/actor/
--rw-rw-rw-   0        0        0    16000 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/actor/Actor.pyi
--rw-rw-rw-   0        0        0      389 2023-02-11 21:17:30.000000 types-panda3d-0.3.2/src/direct-stubs/actor/DistributedActor.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:30.000000 types-panda3d-0.3.2/src/direct-stubs/actor/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.074509 types-panda3d-0.3.2/src/direct-stubs/cluster/
--rw-rw-rw-   0        0        0     6379 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterClient.pyi
--rw-rw-rw-   0        0        0       74 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterConfig.pyi
--rw-rw-rw-   0        0        0     3351 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterMsgs.pyi
--rw-rw-rw-   0        0        0     3277 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterServer.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.092147 types-panda3d-0.3.2/src/direct-stubs/controls/
--rw-rw-rw-   0        0        0      334 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/controls/BattleWalker.pyi
--rw-rw-rw-   0        0        0     2386 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/controls/ControlManager.pyi
--rw-rw-rw-   0        0        0     2214 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/controls/DevWalker.pyi
--rw-rw-rw-   0        0        0       92 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/controls/GhostWalker.pyi
--rw-rw-rw-   0        0        0     4450 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/controls/GravityWalker.pyi
--rw-rw-rw-   0        0        0     2131 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/InputState.pyi
--rw-rw-rw-   0        0        0     2827 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/NonPhysicsWalker.pyi
--rw-rw-rw-   0        0        0       95 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/ObserverWalker.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/PhysicsRoller.pyi
--rw-rw-rw-   0        0        0     3549 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/PhysicsWalker.pyi
--rw-rw-rw-   0        0        0       91 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/SwimWalker.pyi
--rw-rw-rw-   0        0        0      245 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/TwoDWalker.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:29.000000 types-panda3d-0.3.2/src/direct-stubs/controls/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.097332 types-panda3d-0.3.2/src/direct-stubs/directbase/
--rw-rw-rw-   0        0        0       92 2022-10-01 23:45:06.000000 types-panda3d-0.3.2/src/direct-stubs/directbase/DirectStart.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:07:48.000000 types-panda3d-0.3.2/src/direct-stubs/directbase/TestStart.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:07:48.000000 types-panda3d-0.3.2/src/direct-stubs/directbase/ThreeUpStart.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directbase/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.104149 types-panda3d-0.3.2/src/direct-stubs/directdevices/
--rw-rw-rw-   0        0        0     3612 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectDeviceManager.pyi
--rw-rw-rw-   0        0        0     1014 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectFastrak.pyi
--rw-rw-rw-   0        0        0     4064 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectJoybox.pyi
--rw-rw-rw-   0        0        0     1053 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectRadamec.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directdevices/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.114349 types-panda3d-0.3.2/src/direct-stubs/directnotify/
--rw-rw-rw-   0        0        0      830 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/DirectNotify.pyi
--rw-rw-rw-   0        0        0      387 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/DirectNotifyGlobal.pyi
--rw-rw-rw-   0        0        0      262 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/Logger.pyi
--rw-rw-rw-   0        0        0       99 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/LoggerGlobal.pyi
--rw-rw-rw-   0        0        0     1529 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/Notifier.pyi
--rw-rw-rw-   0        0        0     1122 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/RotatingLog.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directnotify/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.119548 types-panda3d-0.3.2/src/direct-stubs/directscripts/
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directscripts/__init__.pyi
--rw-rw-rw-   0        0        0      722 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directscripts/eggcacher.pyi
--rw-rw-rw-   0        0        0      716 2023-02-11 21:17:28.000000 types-panda3d-0.3.2/src/direct-stubs/directscripts/extract_docs.pyi
--rw-rw-rw-   0        0        0     6474 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/directscripts/gendocs.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.133554 types-panda3d-0.3.2/src/direct-stubs/directtools/
--rw-rw-rw-   0        0        0     4121 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectCameraControl.pyi
--rw-rw-rw-   0        0        0     2572 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGeometry.pyi
--rw-rw-rw-   0        0        0     1380 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGlobals.pyi
--rw-rw-rw-   0        0        0     1606 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGrid.pyi
--rw-rw-rw-   0        0        0     1776 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectLights.pyi
--rw-rw-rw-   0        0        0     6060 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectManipulation.pyi
--rw-rw-rw-   0        0        0     7425 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectSelection.pyi
--rw-rw-rw-   0        0        0     9176 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectSession.pyi
--rw-rw-rw-   0        0        0      684 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/DirectUtil.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directtools/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.148410 types-panda3d-0.3.2/src/direct-stubs/directutil/
--rw-rw-rw-   0        0        0      206 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/DeltaProfiler.pyi
--rw-rw-rw-   0        0        0      205 2022-10-13 21:14:28.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/DirectMySQLdb.pyi
--rw-rw-rw-   0        0        0       56 2022-10-01 23:45:06.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/DirectMySQLdbConnection.pyi
--rw-rw-rw-   0        0        0      713 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/DistributedLargeBlobSender.pyi
--rw-rw-rw-   0        0        0      470 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/DistributedLargeBlobSenderAI.pyi
--rw-rw-rw-   0        0        0      167 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/LargeBlobSenderConsts.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/MemoryLeakHelpers.pyi
--rw-rw-rw-   0        0        0     1581 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/Mopath.pyi
--rw-rw-rw-   0        0        0      128 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/Verify.pyi
--rw-rw-rw-   0        0        0      416 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/WeightedChoice.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/directutil/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.155870 types-panda3d-0.3.2/src/direct-stubs/dist/
--rw-rw-rw-   0        0        0     5430 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/dist/FreezeTool.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/dist/__init__.pyi
--rw-rw-rw-   0        0        0     3640 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/dist/commands.pyi
--rw-rw-rw-   0        0        0     5487 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/dist/pefile.pyi
--rw-rw-rw-   0        0        0      157 2023-02-11 21:17:27.000000 types-panda3d-0.3.2/src/direct-stubs/dist/pfreeze.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.221865 types-panda3d-0.3.2/src/direct-stubs/distributed/
--rw-rw-rw-   0        0        0     1927 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/AsyncRequest.pyi
--rw-rw-rw-   0        0        0      775 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/CRCache.pyi
--rw-rw-rw-   0        0        0      396 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/CRDataCache.pyi
--rw-rw-rw-   0        0        0      128 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/CachedDOData.pyi
--rw-rw-rw-   0        0        0      979 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/CartesianGridBase.pyi
--rw-rw-rw-   0        0        0     2561 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ClientRepository.pyi
--rw-rw-rw-   0        0        0     4187 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ClientRepositoryBase.pyi
--rw-rw-rw-   0        0        0     1763 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ClockDelta.pyi
--rw-rw-rw-   0        0        0     2995 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ConnectionRepository.pyi
--rw-rw-rw-   0        0        0     2081 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCamera.pyi
--rw-rw-rw-   0        0        0      280 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCameraAI.pyi
--rw-rw-rw-   0        0        0     1257 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCameraOV.pyi
--rw-rw-rw-   0        0        0     1880 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCartesianGrid.pyi
--rw-rw-rw-   0        0        0     1442 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCartesianGridAI.pyi
--rw-rw-rw-   0        0        0     1970 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNode.pyi
--rw-rw-rw-   0        0        0     1977 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNodeAI.pyi
--rw-rw-rw-   0        0        0     1526 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNodeUD.pyi
--rw-rw-rw-   0        0        0     3694 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObject.pyi
--rw-rw-rw-   0        0        0     4226 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectAI.pyi
--rw-rw-rw-   0        0        0     1224 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectBase.pyi
--rw-rw-rw-   0        0        0      107 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectGlobal.pyi
--rw-rw-rw-   0        0        0      268 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectGlobalAI.pyi
--rw-rw-rw-   0        0        0      512 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectGlobalUD.pyi
--rw-rw-rw-   0        0        0     1562 2023-02-11 21:17:25.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectOV.pyi
--rw-rw-rw-   0        0        0     3869 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectUD.pyi
--rw-rw-rw-   0        0        0     4219 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNode.pyi
--rw-rw-rw-   0        0        0     2166 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNodeAI.pyi
--rw-rw-rw-   0        0        0     1051 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNodeBase.pyi
--rw-rw-rw-   0        0        0     3433 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DoCollectionManager.pyi
--rw-rw-rw-   0        0        0      746 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DoHierarchy.pyi
--rw-rw-rw-   0        0        0     3088 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/DoInterestManager.pyi
--rw-rw-rw-   0        0        0      822 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/GridChild.pyi
--rw-rw-rw-   0        0        0      695 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/GridParent.pyi
--rw-rw-rw-   0        0        0      962 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/InterestWatcher.pyi
--rw-rw-rw-   0        0        0     5485 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/MsgTypes.pyi
--rw-rw-rw-   0        0        0      615 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/MsgTypesCMU.pyi
--rw-rw-rw-   0        0        0      953 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/NetMessenger.pyi
--rw-rw-rw-   0        0        0      791 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ParentMgr.pyi
--rw-rw-rw-   0        0        0      609 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/PyDatagram.pyi
--rw-rw-rw-   0        0        0      359 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/PyDatagramIterator.pyi
--rw-rw-rw-   0        0        0     1413 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/RelatedObjectMgr.pyi
--rw-rw-rw-   0        0        0      227 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/SampleObject.pyi
--rw-rw-rw-   0        0        0     4035 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/ServerRepository.pyi
--rw-rw-rw-   0        0        0      444 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/StagedObject.pyi
--rw-rw-rw-   0        0        0      817 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/TimeManager.pyi
--rw-rw-rw-   0        0        0      159 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/TimeManagerAI.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:26.000000 types-panda3d-0.3.2/src/direct-stubs/distributed/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.232258 types-panda3d-0.3.2/src/direct-stubs/extensions_native/
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/CInterval_extensions.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/HTTPChannel_extensions.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/Mat3_extensions.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/NodePath_extensions.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/VBase3_extensions.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/VBase4_extensions.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/__init__.pyi
--rw-rw-rw-   0        0        0      435 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/extensions_native/extension_native_helpers.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.245661 types-panda3d-0.3.2/src/direct-stubs/filter/
--rw-rw-rw-   0        0        0     4406 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/CommonFilters.pyi
--rw-rw-rw-   0        0        0     3156 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/FilterManager.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/__init__.pyi
--rw-rw-rw-   0        0        0       60 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterBloomI.pyi
--rw-rw-rw-   0        0        0       60 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterBloomX.pyi
--rw-rw-rw-   0        0        0       60 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterBloomY.pyi
--rw-rw-rw-   0        0        0       59 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterBlurX.pyi
--rw-rw-rw-   0        0        0       59 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterBlurY.pyi
--rw-rw-rw-   0        0        0       57 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterCopy.pyi
--rw-rw-rw-   0        0        0       59 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/filter/filterDown4.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.257803 types-panda3d-0.3.2/src/direct-stubs/fsm/
--rw-rw-rw-   0        0        0     2035 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/ClassicFSM.pyi
--rw-rw-rw-   0        0        0     1842 2023-02-15 18:38:09.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/FSM.pyi
--rw-rw-rw-   0        0        0     1424 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/FourState.pyi
--rw-rw-rw-   0        0        0     1758 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/FourStateAI.pyi
--rw-rw-rw-   0        0        0     1979 2023-02-15 18:38:09.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/SampleFSM.pyi
--rw-rw-rw-   0        0        0     1770 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/State.pyi
--rw-rw-rw-   0        0        0      546 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/StateData.pyi
--rw-rw-rw-   0        0        0     1932 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/StatePush.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/fsm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.288902 types-panda3d-0.3.2/src/direct-stubs/gui/
--rw-rw-rw-   0        0        0      470 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectButton.pyi
--rw-rw-rw-   0        0        0      222 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectCheckBox.pyi
--rw-rw-rw-   0        0        0      341 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectCheckButton.pyi
--rw-rw-rw-   0        0        0     1269 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectDialog.pyi
--rw-rw-rw-   0        0        0     1825 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectEntry.pyi
--rw-rw-rw-   0        0        0      783 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectEntryScroll.pyi
--rw-rw-rw-   0        0        0      938 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectFrame.pyi
--rw-rw-rw-   0        0        0      585 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectGui.pyi
--rw-rw-rw-   0        0        0     4895 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectGuiBase.pyi
--rw-rw-rw-   0        0        0     3526 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectGuiGlobals.pyi
--rw-rw-rw-   0        0        0       87 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectGuiTest.pyi
--rw-rw-rw-   0        0        0      288 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectLabel.pyi
--rw-rw-rw-   0        0        0     1086 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectOptionMenu.pyi
--rw-rw-rw-   0        0        0      596 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectRadioButton.pyi
--rw-rw-rw-   0        0        0      903 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrollBar.pyi
--rw-rw-rw-   0        0        0      673 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrolledFrame.pyi
--rw-rw-rw-   0        0        0     1979 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrolledList.pyi
--rw-rw-rw-   0        0        0      641 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectSlider.pyi
--rw-rw-rw-   0        0        0      716 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/DirectWaitBar.pyi
--rw-rw-rw-   0        0        0     1176 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenGeom.pyi
--rw-rw-rw-   0        0        0     1105 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenImage.pyi
--rw-rw-rw-   0        0        0     4152 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenText.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:24.000000 types-panda3d-0.3.2/src/direct-stubs/gui/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.313233 types-panda3d-0.3.2/src/direct-stubs/interval/
--rw-rw-rw-   0        0        0     1887 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/ActorInterval.pyi
--rw-rw-rw-   0        0        0      970 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/AnimControlInterval.pyi
--rw-rw-rw-   0        0        0     3965 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/interval/FunctionInterval.pyi
--rw-rw-rw-   0        0        0      796 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/IndirectInterval.pyi
--rw-rw-rw-   0        0        0     2865 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/Interval.pyi
--rw-rw-rw-   0        0        0      399 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/IntervalGlobal.pyi
--rw-rw-rw-   0        0        0      936 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/IntervalManager.pyi
--rw-rw-rw-   0        0        0       87 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/IntervalTest.pyi
--rw-rw-rw-   0        0        0      621 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/LerpBlendHelpers.pyi
--rw-rw-rw-   0        0        0    16096 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/LerpInterval.pyi
--rw-rw-rw-   0        0        0     4390 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/interval/MetaInterval.pyi
--rw-rw-rw-   0        0        0      711 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/MopathInterval.pyi
--rw-rw-rw-   0        0        0      676 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/ParticleInterval.pyi
--rw-rw-rw-   0        0        0     1123 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/ProjectileInterval.pyi
--rw-rw-rw-   0        0        0      135 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/ProjectileIntervalTest.pyi
--rw-rw-rw-   0        0        0      919 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/SoundInterval.pyi
--rw-rw-rw-   0        0        0      540 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/TestInterval.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/interval/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.365035 types-panda3d-0.3.2/src/direct-stubs/leveleditor/
--rw-rw-rw-   0        0        0     2752 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ActionMgr.pyi
--rw-rw-rw-   0        0        0     4683 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimControlUI.pyi
--rw-rw-rw-   0        0        0      432 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimGlobals.pyi
--rw-rw-rw-   0        0        0       73 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimMgr.pyi
--rw-rw-rw-   0        0        0     3386 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimMgrBase.pyi
--rw-rw-rw-   0        0        0     1284 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/CurveAnimUI.pyi
--rw-rw-rw-   0        0        0     1239 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/CurveEditor.pyi
--rw-rw-rw-   0        0        0      328 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/FileMgr.pyi
--rw-rw-rw-   0        0        0     3738 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/GraphEditorUI.pyi
--rw-rw-rw-   0        0        0     1046 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/HotKeyUI.pyi
--rw-rw-rw-   0        0        0     1493 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LayerEditorUI.pyi
--rw-rw-rw-   0        0        0      486 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditor.pyi
--rw-rw-rw-   0        0        0     3160 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorBase.pyi
--rw-rw-rw-   0        0        0       27 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorStart.pyi
--rw-rw-rw-   0        0        0      171 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorUI.pyi
--rw-rw-rw-   0        0        0     4315 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorUIBase.pyi
--rw-rw-rw-   0        0        0      146 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelLoader.pyi
--rw-rw-rw-   0        0        0      325 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelLoaderBase.pyi
--rw-rw-rw-   0        0        0     1676 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/MayaConverter.pyi
--rw-rw-rw-   0        0        0     1011 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectGlobals.pyi
--rw-rw-rw-   0        0        0      670 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectHandler.pyi
--rw-rw-rw-   0        0        0       81 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectMgr.pyi
--rw-rw-rw-   0        0        0     4132 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectMgrBase.pyi
--rw-rw-rw-   0        0        0      260 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPalette.pyi
--rw-rw-rw-   0        0        0     1672 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPaletteBase.pyi
--rw-rw-rw-   0        0        0      813 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPaletteUI.pyi
--rw-rw-rw-   0        0        0     4548 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPropertyUI.pyi
--rw-rw-rw-   0        0        0     1118 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/PaletteTreeCtrl.pyi
--rw-rw-rw-   0        0        0      321 2023-02-11 21:17:22.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoObjs.pyi
--rw-rw-rw-   0        0        0     1431 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoObjsUI.pyi
--rw-rw-rw-   0        0        0      107 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoPalette.pyi
--rw-rw-rw-   0        0        0      398 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoPaletteBase.pyi
--rw-rw-rw-   0        0        0     1580 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoPaletteUI.pyi
--rw-rw-rw-   0        0        0      135 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/SceneGraphUI.pyi
--rw-rw-rw-   0        0        0     2282 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/SceneGraphUIBase.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:23.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/__init__.pyi
--rw-rw-rw-   0        0        0      149 2022-11-05 18:06:46.000000 types-panda3d-0.3.2/src/direct-stubs/leveleditor/testData.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.367516 types-panda3d-0.3.2/src/direct-stubs/motiontrail/
--rw-rw-rw-   0        0        0     4426 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/motiontrail/MotionTrail.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/motiontrail/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.390622 types-panda3d-0.3.2/src/direct-stubs/p3d/
--rw-rw-rw-   0        0        0     5014 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/AppRunner.pyi
--rw-rw-rw-   0        0        0      368 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/DWBPackageInstaller.pyi
--rw-rw-rw-   0        0        0     3422 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/DeploymentTools.pyi
--rw-rw-rw-   0        0        0     1351 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/FileSpec.pyi
--rw-rw-rw-   0        0        0     2003 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/HostInfo.pyi
--rw-rw-rw-   0        0        0      483 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/InstalledHostData.pyi
--rw-rw-rw-   0        0        0      412 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/InstalledPackageData.pyi
--rw-rw-rw-   0        0        0     1235 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/JavaScript.pyi
--rw-rw-rw-   0        0        0     2923 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/PackageInfo.pyi
--rw-rw-rw-   0        0        0     2656 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/PackageInstaller.pyi
--rw-rw-rw-   0        0        0     1552 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/PackageMerger.pyi
--rw-rw-rw-   0        0        0    13688 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/Packager.pyi
--rw-rw-rw-   0        0        0     5376 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/PatchMaker.pyi
--rw-rw-rw-   0        0        0      523 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/ScanDirectoryNode.pyi
--rw-rw-rw-   0        0        0      769 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/SeqValue.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/__init__.pyi
--rw-rw-rw-   0        0        0       84 2023-02-11 21:17:21.000000 types-panda3d-0.3.2/src/direct-stubs/p3d/runp3d.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.403991 types-panda3d-0.3.2/src/direct-stubs/particles/
--rw-rw-rw-   0        0        0     1342 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/ForceGroup.pyi
--rw-rw-rw-   0        0        0       79 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/GlobalForceGroup.pyi
--rw-rw-rw-   0        0        0     2951 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/ParticleEffect.pyi
--rw-rw-rw-   0        0        0      304 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/ParticleFloorTest.pyi
--rw-rw-rw-   0        0        0      135 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/ParticleManagerGlobal.pyi
--rw-rw-rw-   0        0        0       62 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/ParticleTest.pyi
--rw-rw-rw-   0        0        0     2472 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/Particles.pyi
--rw-rw-rw-   0        0        0     1041 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/SpriteParticleRendererExt.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/particles/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.407463 types-panda3d-0.3.2/src/direct-stubs/physics/
--rw-rw-rw-   0        0        0      383 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/physics/FallTest.pyi
--rw-rw-rw-   0        0        0      416 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/physics/RotationTest.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/physics/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.479797 types-panda3d-0.3.2/src/direct-stubs/showbase/
--rw-rw-rw-   0        0        0       75 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/AppRunnerGlobal.pyi
--rw-rw-rw-   0        0        0     3399 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Audio3DManager.pyi
--rw-rw-rw-   0        0        0     2219 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/BufferViewer.pyi
--rw-rw-rw-   0        0        0      802 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/BulletinBoard.pyi
--rw-rw-rw-   0        0        0      151 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/BulletinBoardGlobal.pyi
--rw-rw-rw-   0        0        0      719 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/BulletinBoardWatcher.pyi
--rw-rw-rw-   0        0        0     4386 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ContainerLeakDetector.pyi
--rw-rw-rw-   0        0        0      488 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ContainerReport.pyi
--rw-rw-rw-   0        0        0      600 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/CountedResource.pyi
--rw-rw-rw-   0        0        0      279 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/DConfig.pyi
--rw-rw-rw-   0        0        0     3260 2023-02-19 00:01:17.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/DirectObject.pyi
--rw-rw-rw-   0        0        0     1515 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/DistancePhasedNode.pyi
--rw-rw-rw-   0        0        0      511 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/EventGroup.pyi
--rw-rw-rw-   0        0        0     1090 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/EventManager.pyi
--rw-rw-rw-   0        0        0      138 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/EventManagerGlobal.pyi
--rw-rw-rw-   0        0        0      477 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ExceptionVarDump.pyi
--rw-rw-rw-   0        0        0      377 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Factory.pyi
--rw-rw-rw-   0        0        0      110 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/FindCtaPaths.pyi
--rw-rw-rw-   0        0        0     1066 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Finder.pyi
--rw-rw-rw-   0        0        0     1669 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/GarbageReport.pyi
--rw-rw-rw-   0        0        0      171 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/GarbageReportScheduler.pyi
--rw-rw-rw-   0        0        0      151 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/InputStateGlobal.pyi
--rw-rw-rw-   0        0        0      968 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Job.pyi
--rw-rw-rw-   0        0        0      597 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/JobManager.pyi
--rw-rw-rw-   0        0        0      128 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/JobManagerGlobal.pyi
--rw-rw-rw-   0        0        0     1104 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/LeakDetectors.pyi
--rw-rw-rw-   0        0        0    12182 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Loader.pyi
--rw-rw-rw-   0        0        0     2256 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Messenger.pyi
--rw-rw-rw-   0        0        0      131 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/MessengerGlobal.pyi
--rw-rw-rw-   0        0        0      357 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/MessengerLeakDetector.pyi
--rw-rw-rw-   0        0        0      366 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/MirrorDemo.pyi
--rw-rw-rw-   0        0        0     1034 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ObjectPool.pyi
--rw-rw-rw-   0        0        0     1070 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ObjectReport.pyi
--rw-rw-rw-   0        0        0      769 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/OnScreenDebug.pyi
--rw-rw-rw-   0        0        0      627 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/PhasedObject.pyi
--rw-rw-rw-   0        0        0      148 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/PhysicsManagerGlobal.pyi
--rw-rw-rw-   0        0        0      871 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Pool.pyi
--rw-rw-rw-   0        0        0     1962 2023-02-11 21:17:19.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ProfileSession.pyi
--rw-rw-rw-   0        0        0    13660 2023-02-15 19:06:57.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/PythonUtil.pyi
--rw-rw-rw-   0        0        0      779 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/RandomNumGen.pyi
--rw-rw-rw-   0        0        0     1020 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ReferrerSearch.pyi
--rw-rw-rw-   0        0        0     1070 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/SfxPlayer.pyi
--rw-rw-rw-   0        0        0      915 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ShadowDemo.pyi
--rw-rw-rw-   0        0        0     1060 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ShadowPlacer.pyi
--rw-rw-rw-   0        0        0    19892 2023-02-18 03:40:14.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ShowBase.pyi
--rw-rw-rw-   0        0        0      795 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ShowBaseGlobal.pyi
--rw-rw-rw-   0        0        0     1154 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/TaskThreaded.pyi
--rw-rw-rw-   0        0        0      713 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/ThreeUpShow.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/TkGlobal.pyi
--rw-rw-rw-   0        0        0     3026 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/Transitions.pyi
--rw-rw-rw-   0        0        0     2002 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/VFSImporter.pyi
--rw-rw-rw-   0        0        0      317 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/VerboseImport.pyi
--rw-rw-rw-   0        0        0       32 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/WxGlobal.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:20.000000 types-panda3d-0.3.2/src/direct-stubs/showbase/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.487237 types-panda3d-0.3.2/src/direct-stubs/showutil/
--rw-rw-rw-   0        0        0     1903 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/BuildGeometry.pyi
--rw-rw-rw-   0        0        0     2094 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/Effects.pyi
--rw-rw-rw-   0        0        0      785 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/Rope.pyi
--rw-rw-rw-   0        0        0     4576 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/TexMemWatcher.pyi
--rw-rw-rw-   0        0        0      317 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/TexViewer.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/showutil/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.497477 types-panda3d-0.3.2/src/direct-stubs/stdpy/
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/__init__.pyi
--rw-rw-rw-   0        0        0     1788 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/file.pyi
--rw-rw-rw-   0        0        0      430 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/glob.pyi
--rw-rw-rw-   0        0        0     1198 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/pickle.pyi
--rw-rw-rw-   0        0        0     1010 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/thread.pyi
--rw-rw-rw-   0        0        0     4451 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/threading.pyi
--rw-rw-rw-   0        0        0     3893 2023-02-18 03:38:53.000000 types-panda3d-0.3.2/src/direct-stubs/stdpy/threading2.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.507893 types-panda3d-0.3.2/src/direct-stubs/task/
--rw-rw-rw-   0        0        0      320 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/task/FrameProfiler.pyi
--rw-rw-rw-   0        0        0      673 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/task/MiniTask.pyi
--rw-rw-rw-   0        0        0     6505 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/Task.pyi
--rw-rw-rw-   0        0        0      126 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/TaskManagerGlobal.pyi
--rw-rw-rw-   0        0        0     1203 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/TaskProfiler.pyi
--rw-rw-rw-   0        0        0      251 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/TaskTester.pyi
--rw-rw-rw-   0        0        0      707 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/Timer.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:18.000000 types-panda3d-0.3.2/src/direct-stubs/task/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.521781 types-panda3d-0.3.2/src/direct-stubs/tkpanels/
--rw-rw-rw-   0        0        0     2962 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/AnimPanel.pyi
--rw-rw-rw-   0        0        0     5932 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/DirectSessionPanel.pyi
--rw-rw-rw-   0        0        0     2876 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/FSMInspector.pyi
--rw-rw-rw-   0        0        0     3560 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/Inspector.pyi
--rw-rw-rw-   0        0        0    11607 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/MopathRecorder.pyi
--rw-rw-rw-   0        0        0     1012 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/NotifyPanel.pyi
--rw-rw-rw-   0        0        0    15351 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/ParticlePanel.pyi
--rw-rw-rw-   0        0        0     3668 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/Placer.pyi
--rw-rw-rw-   0        0        0     1333 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/TaskManagerPanel.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:17.000000 types-panda3d-0.3.2/src/direct-stubs/tkpanels/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.540629 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/
--rw-rw-rw-   0        0        0     7692 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/AppShell.pyi
--rw-rw-rw-   0        0        0     1804 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Dial.pyi
--rw-rw-rw-   0        0        0     1995 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/EntryScale.pyi
--rw-rw-rw-   0        0        0     1460 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Floater.pyi
--rw-rw-rw-   0        0        0     2934 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/MemoryExplorer.pyi
--rw-rw-rw-   0        0        0     1100 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/ProgressBar.pyi
--rw-rw-rw-   0        0        0     1634 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/SceneGraphExplorer.pyi
--rw-rw-rw-   0        0        0     1029 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Slider.pyi
--rw-rw-rw-   0        0        0     2781 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Tree.pyi
--rw-rw-rw-   0        0        0     2833 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Valuator.pyi
--rw-rw-rw-   0        0        0     1186 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/VectorWidgets.pyi
--rw-rw-rw-   0        0        0     1181 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/WidgetPropertiesDialog.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/tkwidgets/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.550548 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/
--rw-rw-rw-   0        0        0     2194 2023-02-11 21:17:15.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/ViewPort.pyi
--rw-rw-rw-   0        0        0      922 2023-02-11 21:17:15.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxAppShell.pyi
--rw-rw-rw-   0        0        0     1652 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxPandaShell.pyi
--rw-rw-rw-   0        0        0       27 2022-10-01 23:45:06.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxPandaStart.pyi
--rw-rw-rw-   0        0        0     1107 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxPandaWindow.pyi
--rw-rw-rw-   0        0        0      929 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxSlider.pyi
--rw-rw-rw-   0        0        0        0 2023-02-11 21:17:16.000000 types-panda3d-0.3.2/src/direct-stubs/wxwidgets/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.567908 types-panda3d-0.3.2/src/panda3d-stubs/
--rw-rw-rw-   0        0        0        0 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/__init__.pyi
--rw-rw-rw-   0        0        0    56745 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/_rplight.pyi
--rw-rw-rw-   0        0        0     1784 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/_typing.pyi
--rw-rw-rw-   0        0        0    11439 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/ai.pyi
--rw-rw-rw-   0        0        0   116158 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/bullet.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.622183 types-panda3d-0.3.2/src/panda3d-stubs/core/
--rw-rw-rw-   0        0        0     1513 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/__init__.pyi
--rw-rw-rw-   0        0        0    20270 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_audio.pyi
--rw-rw-rw-   0        0        0    51687 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_chan.pyi
--rw-rw-rw-   0        0        0    14908 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_char.pyi
--rw-rw-rw-   0        0        0    64825 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_collide.pyi
--rw-rw-rw-   0        0        0    27796 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_device.pyi
--rw-rw-rw-   0        0        0     2598 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_dgraph.pyi
--rw-rw-rw-   0        0        0   192949 2023-02-18 03:17:03.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_display.pyi
--rw-rw-rw-   0        0        0   109064 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_downloader.pyi
--rw-rw-rw-   0        0        0    20469 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_dtoolbase.pyi
--rw-rw-rw-   0        0        0    72671 2023-02-18 03:17:03.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_dtoolutil.pyi
--rw-rw-rw-   0        0        0    39841 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_dxml.pyi
--rw-rw-rw-   0        0        0    57699 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_event.pyi
--rw-rw-rw-   0        0        0   148274 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_express.pyi
--rw-rw-rw-   0        0        0   500671 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_gobj.pyi
--rw-rw-rw-   0        0        0    78185 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_grutil.pyi
--rw-rw-rw-   0        0        0     3586 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_gsgbase.pyi
--rw-rw-rw-   0        0        0   231981 2023-02-18 03:17:05.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_linmath.pyi
--rw-rw-rw-   0        0        0    97791 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_mathutil.pyi
--rw-rw-rw-   0        0        0    26350 2023-02-18 03:17:03.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_movies.pyi
--rw-rw-rw-   0        0        0    12136 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_nativenet.pyi
--rw-rw-rw-   0        0        0    45121 2023-02-18 03:17:03.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_net.pyi
--rw-rw-rw-   0        0        0    73635 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_parametrics.pyi
--rw-rw-rw-   0        0        0   535940 2023-02-18 03:17:07.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pgraph.pyi
--rw-rw-rw-   0        0        0    37715 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pgraphnodes.pyi
--rw-rw-rw-   0        0        0    62263 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pgui.pyi
--rw-rw-rw-   0        0        0    32473 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pipeline.pyi
--rw-rw-rw-   0        0        0    94059 2023-02-18 03:17:04.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pnmimage.pyi
--rw-rw-rw-   0        0        0    13360 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pnmtext.pyi
--rw-rw-rw-   0        0        0    84389 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_prc.pyi
--rw-rw-rw-   0        0        0    21666 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_pstatclient.pyi
--rw-rw-rw-   0        0        0   162906 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_putil.pyi
--rw-rw-rw-   0        0        0    11810 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_recorder.pyi
--rw-rw-rw-   0        0        0    92666 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_text.pyi
--rw-rw-rw-   0        0        0    69588 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/core/_tform.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.633095 types-panda3d-0.3.2/src/panda3d-stubs/direct/
--rw-rw-rw-   0        0        0      161 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/__init__.pyi
--rw-rw-rw-   0        0        0    62968 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_dcparser.pyi
--rw-rw-rw-   0        0        0    19472 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_deadrec.pyi
--rw-rw-rw-   0        0        0    15120 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_distributed.pyi
--rw-rw-rw-   0        0        0    49674 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_interval.pyi
--rw-rw-rw-   0        0        0     3863 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_motiontrail.pyi
--rw-rw-rw-   0        0        0     1067 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/direct/_showbase.pyi
--rw-rw-rw-   0        0        0       30 2023-02-11 21:17:31.000000 types-panda3d-0.3.2/src/panda3d-stubs/dtoolconfig.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.637559 types-panda3d-0.3.2/src/panda3d-stubs/egg/
--rw-rw-rw-   0        0        0       45 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/egg/__init__.pyi
--rw-rw-rw-   0        0        0   237216 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/egg/_egg.pyi
--rw-rw-rw-   0        0        0      771 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/egg/_egg2pg.pyi
--rw-rw-rw-   0        0        0    24860 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/fx.pyi
--rw-rw-rw-   0        0        0    12596 2023-02-11 21:17:31.000000 types-panda3d-0.3.2/src/panda3d-stubs/interrogatedb.pyi
--rw-rw-rw-   0        0        0    65252 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/ode.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.641558 types-panda3d-0.3.2/src/panda3d-stubs/physics/
--rw-rw-rw-   0        0        0       57 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/physics/__init__.pyi
--rw-rw-rw-   0        0        0    49283 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/physics/_particlesystem.pyi
--rw-rw-rw-   0        0        0    39570 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/physics/_physics.pyi
--rw-rw-rw-   0        0        0     2390 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/skel.pyi
--rw-rw-rw-   0        0        0     4617 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/vision.pyi
--rw-rw-rw-   0        0        0     1052 2023-02-18 03:16:59.000000 types-panda3d-0.3.2/src/panda3d-stubs/vrpn.pyi
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.648967 types-panda3d-0.3.2/src/types_panda3d.egg-info/
--rw-rw-rw-   0        0        0     2606 2023-02-19 00:11:58.000000 types-panda3d-0.3.2/src/types_panda3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    18014 2023-02-19 00:11:59.000000 types-panda3d-0.3.2/src/types_panda3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 00:11:58.000000 types-panda3d-0.3.2/src/types_panda3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-02-19 00:11:58.000000 types-panda3d-0.3.2/src/types_panda3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-02-19 00:11:58.000000 types-panda3d-0.3.2/src/types_panda3d.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-19 00:11:59.649959 types-panda3d-0.3.2/tests/
--rw-rw-rw-   0        0        0     2389 2023-02-15 19:06:20.000000 types-panda3d-0.3.2/tests/test_stubtest.py
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.353090 types-panda3d-0.3.3/
+-rw-rw-rw-   0        0        0     1076 2022-08-03 23:48:00.000000 types-panda3d-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2606 2023-07-08 17:02:58.351106 types-panda3d-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2022-10-30 20:43:52.000000 types-panda3d-0.3.3/README.md
+-rw-rw-rw-   0        0        0     1524 2023-07-07 18:43:38.000000 types-panda3d-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 17:02:58.353090 types-panda3d-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.685284 types-panda3d-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.692962 types-panda3d-0.3.3/src/direct-stubs/
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:07.000000 types-panda3d-0.3.3/src/direct-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0      597 2023-04-08 22:49:20.000000 types-panda3d-0.3.3/src/direct-stubs/_typing.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.696977 types-panda3d-0.3.3/src/direct-stubs/actor/
+-rw-rw-rw-   0        0        0    16083 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/actor/Actor.pyi
+-rw-rw-rw-   0        0        0      389 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/actor/DistributedActor.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/actor/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.705908 types-panda3d-0.3.3/src/direct-stubs/cluster/
+-rw-rw-rw-   0        0        0     6377 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterClient.pyi
+-rw-rw-rw-   0        0        0       74 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterConfig.pyi
+-rw-rw-rw-   0        0        0     3351 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterMsgs.pyi
+-rw-rw-rw-   0        0        0     3277 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterServer.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.726624 types-panda3d-0.3.3/src/direct-stubs/controls/
+-rw-rw-rw-   0        0        0      334 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/controls/BattleWalker.pyi
+-rw-rw-rw-   0        0        0     2386 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/controls/ControlManager.pyi
+-rw-rw-rw-   0        0        0     2214 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/controls/DevWalker.pyi
+-rw-rw-rw-   0        0        0       92 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/GhostWalker.pyi
+-rw-rw-rw-   0        0        0     4450 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/GravityWalker.pyi
+-rw-rw-rw-   0        0        0     2131 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/InputState.pyi
+-rw-rw-rw-   0        0        0     2827 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/NonPhysicsWalker.pyi
+-rw-rw-rw-   0        0        0       95 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/ObserverWalker.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/PhysicsRoller.pyi
+-rw-rw-rw-   0        0        0     3549 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/PhysicsWalker.pyi
+-rw-rw-rw-   0        0        0       91 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/SwimWalker.pyi
+-rw-rw-rw-   0        0        0      245 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/TwoDWalker.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:22.000000 types-panda3d-0.3.3/src/direct-stubs/controls/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.732423 types-panda3d-0.3.3/src/direct-stubs/directbase/
+-rw-rw-rw-   0        0        0       92 2022-10-01 23:45:06.000000 types-panda3d-0.3.3/src/direct-stubs/directbase/DirectStart.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directbase/TestStart.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directbase/ThreeUpStart.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directbase/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.741351 types-panda3d-0.3.3/src/direct-stubs/directdevices/
+-rw-rw-rw-   0        0        0     3612 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectDeviceManager.pyi
+-rw-rw-rw-   0        0        0     1014 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectFastrak.pyi
+-rw-rw-rw-   0        0        0     4065 2023-07-07 21:52:59.000000 types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectJoybox.pyi
+-rw-rw-rw-   0        0        0     1054 2023-07-07 21:52:59.000000 types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectRadamec.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directdevices/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.752079 types-panda3d-0.3.3/src/direct-stubs/directnotify/
+-rw-rw-rw-   0        0        0      853 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/DirectNotify.pyi
+-rw-rw-rw-   0        0        0      358 2023-04-29 04:27:34.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/DirectNotifyGlobal.pyi
+-rw-rw-rw-   0        0        0      262 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/Logger.pyi
+-rw-rw-rw-   0        0        0       99 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/LoggerGlobal.pyi
+-rw-rw-rw-   0        0        0     1529 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/Notifier.pyi
+-rw-rw-rw-   0        0        0     1129 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/RotatingLog.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directnotify/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.757528 types-panda3d-0.3.3/src/direct-stubs/directscripts/
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directscripts/__init__.pyi
+-rw-rw-rw-   0        0        0      676 2023-03-31 02:27:42.000000 types-panda3d-0.3.3/src/direct-stubs/directscripts/eggcacher.pyi
+-rw-rw-rw-   0        0        0      716 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directscripts/extract_docs.pyi
+-rw-rw-rw-   0        0        0     6357 2023-07-07 21:52:59.000000 types-panda3d-0.3.3/src/direct-stubs/directscripts/gendocs.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.773656 types-panda3d-0.3.3/src/direct-stubs/directtools/
+-rw-rw-rw-   0        0        0     4121 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectCameraControl.pyi
+-rw-rw-rw-   0        0        0     2572 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGeometry.pyi
+-rw-rw-rw-   0        0        0     1380 2023-07-07 18:44:24.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGlobals.pyi
+-rw-rw-rw-   0        0        0     1623 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGrid.pyi
+-rw-rw-rw-   0        0        0     1776 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectLights.pyi
+-rw-rw-rw-   0        0        0     6060 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectManipulation.pyi
+-rw-rw-rw-   0        0        0     7423 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectSelection.pyi
+-rw-rw-rw-   0        0        0     9175 2023-07-07 21:52:59.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectSession.pyi
+-rw-rw-rw-   0        0        0      684 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/DirectUtil.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:21.000000 types-panda3d-0.3.3/src/direct-stubs/directtools/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.790340 types-panda3d-0.3.3/src/direct-stubs/directutil/
+-rw-rw-rw-   0        0        0      206 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/DeltaProfiler.pyi
+-rw-rw-rw-   0        0        0      205 2022-10-13 21:14:28.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/DirectMySQLdb.pyi
+-rw-rw-rw-   0        0        0      109 2023-03-30 23:50:39.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/DirectMySQLdbConnection.pyi
+-rw-rw-rw-   0        0        0      713 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/DistributedLargeBlobSender.pyi
+-rw-rw-rw-   0        0        0      470 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/DistributedLargeBlobSenderAI.pyi
+-rw-rw-rw-   0        0        0      162 2023-03-31 02:27:13.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/LargeBlobSenderConsts.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/MemoryLeakHelpers.pyi
+-rw-rw-rw-   0        0        0     1581 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/Mopath.pyi
+-rw-rw-rw-   0        0        0      128 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/Verify.pyi
+-rw-rw-rw-   0        0        0      416 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/WeightedChoice.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/directutil/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.796697 types-panda3d-0.3.3/src/direct-stubs/dist/
+-rw-rw-rw-   0        0        0     5427 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/dist/FreezeTool.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:20.000000 types-panda3d-0.3.3/src/direct-stubs/dist/__init__.pyi
+-rw-rw-rw-   0        0        0     3640 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/dist/commands.pyi
+-rw-rw-rw-   0        0        0     5488 2023-05-20 19:46:06.000000 types-panda3d-0.3.3/src/direct-stubs/dist/pefile.pyi
+-rw-rw-rw-   0        0        0      150 2023-03-31 02:27:13.000000 types-panda3d-0.3.3/src/direct-stubs/dist/pfreeze.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.869698 types-panda3d-0.3.3/src/direct-stubs/distributed/
+-rw-rw-rw-   0        0        0     1927 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/AsyncRequest.pyi
+-rw-rw-rw-   0        0        0      775 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/CRCache.pyi
+-rw-rw-rw-   0        0        0      396 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/CRDataCache.pyi
+-rw-rw-rw-   0        0        0      128 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/CachedDOData.pyi
+-rw-rw-rw-   0        0        0      979 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/CartesianGridBase.pyi
+-rw-rw-rw-   0        0        0     2549 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ClientRepository.pyi
+-rw-rw-rw-   0        0        0     4180 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ClientRepositoryBase.pyi
+-rw-rw-rw-   0        0        0     1750 2023-03-31 02:27:13.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ClockDelta.pyi
+-rw-rw-rw-   0        0        0     2993 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ConnectionRepository.pyi
+-rw-rw-rw-   0        0        0     2080 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCamera.pyi
+-rw-rw-rw-   0        0        0      280 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCameraAI.pyi
+-rw-rw-rw-   0        0        0     1257 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCameraOV.pyi
+-rw-rw-rw-   0        0        0     1830 2023-03-31 02:54:51.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCartesianGrid.pyi
+-rw-rw-rw-   0        0        0     1392 2023-03-31 02:54:51.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCartesianGridAI.pyi
+-rw-rw-rw-   0        0        0     1958 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNode.pyi
+-rw-rw-rw-   0        0        0     1977 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNodeAI.pyi
+-rw-rw-rw-   0        0        0     1526 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNodeUD.pyi
+-rw-rw-rw-   0        0        0     3692 2023-03-31 02:36:30.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObject.pyi
+-rw-rw-rw-   0        0        0     4214 2023-03-31 02:27:12.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectAI.pyi
+-rw-rw-rw-   0        0        0     1224 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectBase.pyi
+-rw-rw-rw-   0        0        0      107 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectGlobal.pyi
+-rw-rw-rw-   0        0        0      268 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectGlobalAI.pyi
+-rw-rw-rw-   0        0        0      512 2023-03-31 00:14:18.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectGlobalUD.pyi
+-rw-rw-rw-   0        0        0     1544 2023-03-31 02:54:51.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectOV.pyi
+-rw-rw-rw-   0        0        0     3854 2023-03-31 02:54:51.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectUD.pyi
+-rw-rw-rw-   0        0        0     4219 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNode.pyi
+-rw-rw-rw-   0        0        0     2166 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNodeAI.pyi
+-rw-rw-rw-   0        0        0     1003 2023-03-31 02:59:36.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNodeBase.pyi
+-rw-rw-rw-   0        0        0     3433 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DoCollectionManager.pyi
+-rw-rw-rw-   0        0        0      746 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DoHierarchy.pyi
+-rw-rw-rw-   0        0        0     3052 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/DoInterestManager.pyi
+-rw-rw-rw-   0        0        0      822 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/GridChild.pyi
+-rw-rw-rw-   0        0        0      695 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/GridParent.pyi
+-rw-rw-rw-   0        0        0      962 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/InterestWatcher.pyi
+-rw-rw-rw-   0        0        0     5481 2023-07-07 18:43:38.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/MsgTypes.pyi
+-rw-rw-rw-   0        0        0      615 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/MsgTypesCMU.pyi
+-rw-rw-rw-   0        0        0      879 2023-07-07 18:43:38.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/NetMessenger.pyi
+-rw-rw-rw-   0        0        0      791 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ParentMgr.pyi
+-rw-rw-rw-   0        0        0      609 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/PyDatagram.pyi
+-rw-rw-rw-   0        0        0      359 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/PyDatagramIterator.pyi
+-rw-rw-rw-   0        0        0     1413 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/RelatedObjectMgr.pyi
+-rw-rw-rw-   0        0        0      227 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/SampleObject.pyi
+-rw-rw-rw-   0        0        0     4009 2023-05-21 03:12:13.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/ServerRepository.pyi
+-rw-rw-rw-   0        0        0      444 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/StagedObject.pyi
+-rw-rw-rw-   0        0        0      817 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/TimeManager.pyi
+-rw-rw-rw-   0        0        0      159 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/TimeManagerAI.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:19.000000 types-panda3d-0.3.3/src/direct-stubs/distributed/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.880714 types-panda3d-0.3.3/src/direct-stubs/extensions_native/
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/CInterval_extensions.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/HTTPChannel_extensions.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/Mat3_extensions.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/NodePath_extensions.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/VBase3_extensions.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/VBase4_extensions.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/__init__.pyi
+-rw-rw-rw-   0        0        0      435 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/extensions_native/extension_native_helpers.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.896443 types-panda3d-0.3.3/src/direct-stubs/filter/
+-rw-rw-rw-   0        0        0     4432 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/CommonFilters.pyi
+-rw-rw-rw-   0        0        0     3156 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/FilterManager.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/__init__.pyi
+-rw-rw-rw-   0        0        0       60 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterBloomI.pyi
+-rw-rw-rw-   0        0        0       60 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterBloomX.pyi
+-rw-rw-rw-   0        0        0       60 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterBloomY.pyi
+-rw-rw-rw-   0        0        0       59 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterBlurX.pyi
+-rw-rw-rw-   0        0        0       59 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterBlurY.pyi
+-rw-rw-rw-   0        0        0       57 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterCopy.pyi
+-rw-rw-rw-   0        0        0       59 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/filter/filterDown4.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.910084 types-panda3d-0.3.3/src/direct-stubs/fsm/
+-rw-rw-rw-   0        0        0     2116 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/ClassicFSM.pyi
+-rw-rw-rw-   0        0        0     1851 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/FSM.pyi
+-rw-rw-rw-   0        0        0     1439 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/FourState.pyi
+-rw-rw-rw-   0        0        0     1789 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/FourStateAI.pyi
+-rw-rw-rw-   0        0        0     1979 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/SampleFSM.pyi
+-rw-rw-rw-   0        0        0     1767 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/State.pyi
+-rw-rw-rw-   0        0        0      553 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/StateData.pyi
+-rw-rw-rw-   0        0        0     1929 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/StatePush.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/fsm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.943897 types-panda3d-0.3.3/src/direct-stubs/gui/
+-rw-rw-rw-   0        0        0      470 2023-05-20 20:20:39.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectButton.pyi
+-rw-rw-rw-   0        0        0      222 2023-05-20 20:20:39.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectCheckBox.pyi
+-rw-rw-rw-   0        0        0      341 2023-05-20 20:20:39.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectCheckButton.pyi
+-rw-rw-rw-   0        0        0     1269 2023-05-20 20:20:39.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectDialog.pyi
+-rw-rw-rw-   0        0        0     1825 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectEntry.pyi
+-rw-rw-rw-   0        0        0      783 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectEntryScroll.pyi
+-rw-rw-rw-   0        0        0      938 2023-05-20 20:20:39.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectFrame.pyi
+-rw-rw-rw-   0        0        0      585 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectGui.pyi
+-rw-rw-rw-   0        0        0     4893 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectGuiBase.pyi
+-rw-rw-rw-   0        0        0     3514 2023-07-07 18:43:38.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectGuiGlobals.pyi
+-rw-rw-rw-   0        0        0       87 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectGuiTest.pyi
+-rw-rw-rw-   0        0        0      288 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectLabel.pyi
+-rw-rw-rw-   0        0        0     1086 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectOptionMenu.pyi
+-rw-rw-rw-   0        0        0      596 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectRadioButton.pyi
+-rw-rw-rw-   0        0        0      903 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrollBar.pyi
+-rw-rw-rw-   0        0        0      673 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrolledFrame.pyi
+-rw-rw-rw-   0        0        0     1979 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrolledList.pyi
+-rw-rw-rw-   0        0        0      641 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectSlider.pyi
+-rw-rw-rw-   0        0        0      716 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/DirectWaitBar.pyi
+-rw-rw-rw-   0        0        0     1176 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenGeom.pyi
+-rw-rw-rw-   0        0        0     1105 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenImage.pyi
+-rw-rw-rw-   0        0        0     4155 2023-03-31 02:27:12.000000 types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenText.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:17.000000 types-panda3d-0.3.3/src/direct-stubs/gui/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:57.973137 types-panda3d-0.3.3/src/direct-stubs/interval/
+-rw-rw-rw-   0        0        0     1887 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/interval/ActorInterval.pyi
+-rw-rw-rw-   0        0        0      982 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/interval/AnimControlInterval.pyi
+-rw-rw-rw-   0        0        0     3964 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/FunctionInterval.pyi
+-rw-rw-rw-   0        0        0      796 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/IndirectInterval.pyi
+-rw-rw-rw-   0        0        0     2865 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/Interval.pyi
+-rw-rw-rw-   0        0        0      399 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/IntervalGlobal.pyi
+-rw-rw-rw-   0        0        0      936 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/IntervalManager.pyi
+-rw-rw-rw-   0        0        0       87 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/IntervalTest.pyi
+-rw-rw-rw-   0        0        0      621 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/interval/LerpBlendHelpers.pyi
+-rw-rw-rw-   0        0        0    16094 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/interval/LerpInterval.pyi
+-rw-rw-rw-   0        0        0     4472 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/interval/MetaInterval.pyi
+-rw-rw-rw-   0        0        0      711 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/MopathInterval.pyi
+-rw-rw-rw-   0        0        0      676 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/ParticleInterval.pyi
+-rw-rw-rw-   0        0        0     1123 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/ProjectileInterval.pyi
+-rw-rw-rw-   0        0        0      135 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/ProjectileIntervalTest.pyi
+-rw-rw-rw-   0        0        0      919 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/SoundInterval.pyi
+-rw-rw-rw-   0        0        0      540 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/TestInterval.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:16.000000 types-panda3d-0.3.3/src/direct-stubs/interval/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.030540 types-panda3d-0.3.3/src/direct-stubs/leveleditor/
+-rw-rw-rw-   0        0        0     2752 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ActionMgr.pyi
+-rw-rw-rw-   0        0        0     4683 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimControlUI.pyi
+-rw-rw-rw-   0        0        0      432 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimGlobals.pyi
+-rw-rw-rw-   0        0        0       73 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimMgr.pyi
+-rw-rw-rw-   0        0        0     3265 2023-07-07 21:53:01.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimMgrBase.pyi
+-rw-rw-rw-   0        0        0     1284 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/CurveAnimUI.pyi
+-rw-rw-rw-   0        0        0     1195 2023-03-31 02:27:12.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/CurveEditor.pyi
+-rw-rw-rw-   0        0        0      328 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/FileMgr.pyi
+-rw-rw-rw-   0        0        0     3738 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/GraphEditorUI.pyi
+-rw-rw-rw-   0        0        0     1046 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/HotKeyUI.pyi
+-rw-rw-rw-   0        0        0     1493 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LayerEditorUI.pyi
+-rw-rw-rw-   0        0        0      486 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditor.pyi
+-rw-rw-rw-   0        0        0     3160 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorBase.pyi
+-rw-rw-rw-   0        0        0       27 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorStart.pyi
+-rw-rw-rw-   0        0        0      171 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorUI.pyi
+-rw-rw-rw-   0        0        0     4315 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorUIBase.pyi
+-rw-rw-rw-   0        0        0      146 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelLoader.pyi
+-rw-rw-rw-   0        0        0      325 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelLoaderBase.pyi
+-rw-rw-rw-   0        0        0     1676 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/MayaConverter.pyi
+-rw-rw-rw-   0        0        0     1011 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectGlobals.pyi
+-rw-rw-rw-   0        0        0      670 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectHandler.pyi
+-rw-rw-rw-   0        0        0       81 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectMgr.pyi
+-rw-rw-rw-   0        0        0     4132 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectMgrBase.pyi
+-rw-rw-rw-   0        0        0      260 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPalette.pyi
+-rw-rw-rw-   0        0        0     1665 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPaletteBase.pyi
+-rw-rw-rw-   0        0        0      813 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPaletteUI.pyi
+-rw-rw-rw-   0        0        0     4548 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPropertyUI.pyi
+-rw-rw-rw-   0        0        0     1118 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/PaletteTreeCtrl.pyi
+-rw-rw-rw-   0        0        0      321 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoObjs.pyi
+-rw-rw-rw-   0        0        0     1431 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoObjsUI.pyi
+-rw-rw-rw-   0        0        0      107 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoPalette.pyi
+-rw-rw-rw-   0        0        0      398 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoPaletteBase.pyi
+-rw-rw-rw-   0        0        0     1580 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoPaletteUI.pyi
+-rw-rw-rw-   0        0        0      135 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/SceneGraphUI.pyi
+-rw-rw-rw-   0        0        0     2282 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/SceneGraphUIBase.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:15.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/__init__.pyi
+-rw-rw-rw-   0        0        0      149 2022-11-05 18:06:46.000000 types-panda3d-0.3.3/src/direct-stubs/leveleditor/testData.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.033019 types-panda3d-0.3.3/src/direct-stubs/motiontrail/
+-rw-rw-rw-   0        0        0     4426 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/motiontrail/MotionTrail.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/motiontrail/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.057724 types-panda3d-0.3.3/src/direct-stubs/p3d/
+-rw-rw-rw-   0        0        0     5013 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/AppRunner.pyi
+-rw-rw-rw-   0        0        0      368 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/DWBPackageInstaller.pyi
+-rw-rw-rw-   0        0        0     3391 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/DeploymentTools.pyi
+-rw-rw-rw-   0        0        0     1351 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/FileSpec.pyi
+-rw-rw-rw-   0        0        0     2003 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/HostInfo.pyi
+-rw-rw-rw-   0        0        0      483 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/InstalledHostData.pyi
+-rw-rw-rw-   0        0        0      412 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/InstalledPackageData.pyi
+-rw-rw-rw-   0        0        0     1235 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/JavaScript.pyi
+-rw-rw-rw-   0        0        0     2923 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/PackageInfo.pyi
+-rw-rw-rw-   0        0        0     2655 2023-07-07 21:53:01.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/PackageInstaller.pyi
+-rw-rw-rw-   0        0        0     1552 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/PackageMerger.pyi
+-rw-rw-rw-   0        0        0    13689 2023-07-07 21:53:01.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/Packager.pyi
+-rw-rw-rw-   0        0        0     5374 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/PatchMaker.pyi
+-rw-rw-rw-   0        0        0      523 2023-07-07 21:53:01.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/ScanDirectoryNode.pyi
+-rw-rw-rw-   0        0        0      769 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/SeqValue.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/__init__.pyi
+-rw-rw-rw-   0        0        0       84 2023-03-31 00:14:14.000000 types-panda3d-0.3.3/src/direct-stubs/p3d/runp3d.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.071118 types-panda3d-0.3.3/src/direct-stubs/particles/
+-rw-rw-rw-   0        0        0     1342 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/particles/ForceGroup.pyi
+-rw-rw-rw-   0        0        0       79 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/particles/GlobalForceGroup.pyi
+-rw-rw-rw-   0        0        0     2951 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/particles/ParticleEffect.pyi
+-rw-rw-rw-   0        0        0      304 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/particles/ParticleFloorTest.pyi
+-rw-rw-rw-   0        0        0      135 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/particles/ParticleManagerGlobal.pyi
+-rw-rw-rw-   0        0        0       62 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/particles/ParticleTest.pyi
+-rw-rw-rw-   0        0        0     2472 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/particles/Particles.pyi
+-rw-rw-rw-   0        0        0     1041 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/particles/SpriteParticleRendererExt.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/particles/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.076079 types-panda3d-0.3.3/src/direct-stubs/physics/
+-rw-rw-rw-   0        0        0      383 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/physics/FallTest.pyi
+-rw-rw-rw-   0        0        0      416 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/physics/RotationTest.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/physics/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.156401 types-panda3d-0.3.3/src/direct-stubs/showbase/
+-rw-rw-rw-   0        0        0       75 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/AppRunnerGlobal.pyi
+-rw-rw-rw-   0        0        0     3419 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Audio3DManager.pyi
+-rw-rw-rw-   0        0        0     2275 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/BufferViewer.pyi
+-rw-rw-rw-   0        0        0      802 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/BulletinBoard.pyi
+-rw-rw-rw-   0        0        0      151 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/BulletinBoardGlobal.pyi
+-rw-rw-rw-   0        0        0      719 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/BulletinBoardWatcher.pyi
+-rw-rw-rw-   0        0        0     4377 2023-04-08 22:49:20.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ContainerLeakDetector.pyi
+-rw-rw-rw-   0        0        0      488 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ContainerReport.pyi
+-rw-rw-rw-   0        0        0      600 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/CountedResource.pyi
+-rw-rw-rw-   0        0        0      279 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/DConfig.pyi
+-rw-rw-rw-   0        0        0     3190 2023-03-31 03:19:38.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/DirectObject.pyi
+-rw-rw-rw-   0        0        0     1513 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/DistancePhasedNode.pyi
+-rw-rw-rw-   0        0        0      511 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/EventGroup.pyi
+-rw-rw-rw-   0        0        0     1090 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/EventManager.pyi
+-rw-rw-rw-   0        0        0      138 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/EventManagerGlobal.pyi
+-rw-rw-rw-   0        0        0      477 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ExceptionVarDump.pyi
+-rw-rw-rw-   0        0        0      377 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Factory.pyi
+-rw-rw-rw-   0        0        0      110 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/FindCtaPaths.pyi
+-rw-rw-rw-   0        0        0     1066 2023-05-21 03:12:14.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Finder.pyi
+-rw-rw-rw-   0        0        0     1669 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/GarbageReport.pyi
+-rw-rw-rw-   0        0        0      171 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/GarbageReportScheduler.pyi
+-rw-rw-rw-   0        0        0      151 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/InputStateGlobal.pyi
+-rw-rw-rw-   0        0        0      968 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Job.pyi
+-rw-rw-rw-   0        0        0      597 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/JobManager.pyi
+-rw-rw-rw-   0        0        0      128 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/JobManagerGlobal.pyi
+-rw-rw-rw-   0        0        0     1104 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/LeakDetectors.pyi
+-rw-rw-rw-   0        0        0    12189 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Loader.pyi
+-rw-rw-rw-   0        0        0     2254 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Messenger.pyi
+-rw-rw-rw-   0        0        0      131 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/MessengerGlobal.pyi
+-rw-rw-rw-   0        0        0      357 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/MessengerLeakDetector.pyi
+-rw-rw-rw-   0        0        0      366 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/MirrorDemo.pyi
+-rw-rw-rw-   0        0        0     1034 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ObjectPool.pyi
+-rw-rw-rw-   0        0        0     1070 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ObjectReport.pyi
+-rw-rw-rw-   0        0        0      769 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/OnScreenDebug.pyi
+-rw-rw-rw-   0        0        0      626 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/PhasedObject.pyi
+-rw-rw-rw-   0        0        0      148 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/PhysicsManagerGlobal.pyi
+-rw-rw-rw-   0        0        0      871 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Pool.pyi
+-rw-rw-rw-   0        0        0     1962 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ProfileSession.pyi
+-rw-rw-rw-   0        0        0    13678 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/PythonUtil.pyi
+-rw-rw-rw-   0        0        0      779 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/RandomNumGen.pyi
+-rw-rw-rw-   0        0        0     1020 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ReferrerSearch.pyi
+-rw-rw-rw-   0        0        0     1070 2023-03-31 00:14:12.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/SfxPlayer.pyi
+-rw-rw-rw-   0        0        0      915 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ShadowDemo.pyi
+-rw-rw-rw-   0        0        0     1060 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ShadowPlacer.pyi
+-rw-rw-rw-   0        0        0    20005 2023-07-07 21:53:01.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ShowBase.pyi
+-rw-rw-rw-   0        0        0      795 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ShowBaseGlobal.pyi
+-rw-rw-rw-   0        0        0     1154 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/TaskThreaded.pyi
+-rw-rw-rw-   0        0        0      722 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/ThreeUpShow.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/TkGlobal.pyi
+-rw-rw-rw-   0        0        0     3020 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/Transitions.pyi
+-rw-rw-rw-   0        0        0     2067 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/VFSImporter.pyi
+-rw-rw-rw-   0        0        0      317 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/VerboseImport.pyi
+-rw-rw-rw-   0        0        0       32 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/WxGlobal.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:13.000000 types-panda3d-0.3.3/src/direct-stubs/showbase/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.164819 types-panda3d-0.3.3/src/direct-stubs/showutil/
+-rw-rw-rw-   0        0        0     1903 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/BuildGeometry.pyi
+-rw-rw-rw-   0        0        0     2094 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/Effects.pyi
+-rw-rw-rw-   0        0        0      729 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/Rope.pyi
+-rw-rw-rw-   0        0        0     4576 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/TexMemWatcher.pyi
+-rw-rw-rw-   0        0        0      317 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/TexViewer.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:11.000000 types-panda3d-0.3.3/src/direct-stubs/showutil/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.178406 types-panda3d-0.3.3/src/direct-stubs/stdpy/
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/__init__.pyi
+-rw-rw-rw-   0        0        0     1706 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/file.pyi
+-rw-rw-rw-   0        0        0      426 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/glob.pyi
+-rw-rw-rw-   0        0        0     1198 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/pickle.pyi
+-rw-rw-rw-   0        0        0     1009 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/thread.pyi
+-rw-rw-rw-   0        0        0     4447 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/threading.pyi
+-rw-rw-rw-   0        0        0     3890 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/stdpy/threading2.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.190310 types-panda3d-0.3.3/src/direct-stubs/task/
+-rw-rw-rw-   0        0        0      320 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/FrameProfiler.pyi
+-rw-rw-rw-   0        0        0      673 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/MiniTask.pyi
+-rw-rw-rw-   0        0        0     6465 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/task/Task.pyi
+-rw-rw-rw-   0        0        0      126 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/TaskManagerGlobal.pyi
+-rw-rw-rw-   0        0        0     1210 2023-06-28 22:32:59.000000 types-panda3d-0.3.3/src/direct-stubs/task/TaskProfiler.pyi
+-rw-rw-rw-   0        0        0      251 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/TaskTester.pyi
+-rw-rw-rw-   0        0        0      707 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/Timer.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/task/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.207701 types-panda3d-0.3.3/src/direct-stubs/tkpanels/
+-rw-rw-rw-   0        0        0     2961 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/AnimPanel.pyi
+-rw-rw-rw-   0        0        0     5930 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/DirectSessionPanel.pyi
+-rw-rw-rw-   0        0        0     2876 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/FSMInspector.pyi
+-rw-rw-rw-   0        0        0     3560 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/Inspector.pyi
+-rw-rw-rw-   0        0        0    11604 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/MopathRecorder.pyi
+-rw-rw-rw-   0        0        0     1012 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/NotifyPanel.pyi
+-rw-rw-rw-   0        0        0    15351 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/ParticlePanel.pyi
+-rw-rw-rw-   0        0        0     3666 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/Placer.pyi
+-rw-rw-rw-   0        0        0     1333 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/TaskManagerPanel.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:10.000000 types-panda3d-0.3.3/src/direct-stubs/tkpanels/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.227930 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/
+-rw-rw-rw-   0        0        0     7690 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/AppShell.pyi
+-rw-rw-rw-   0        0        0     1804 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Dial.pyi
+-rw-rw-rw-   0        0        0     1995 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/EntryScale.pyi
+-rw-rw-rw-   0        0        0     1460 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Floater.pyi
+-rw-rw-rw-   0        0        0     2934 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/MemoryExplorer.pyi
+-rw-rw-rw-   0        0        0     1100 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/ProgressBar.pyi
+-rw-rw-rw-   0        0        0     1610 2023-03-31 02:37:20.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/SceneGraphExplorer.pyi
+-rw-rw-rw-   0        0        0     1029 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Slider.pyi
+-rw-rw-rw-   0        0        0     2745 2023-03-31 02:27:42.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Tree.pyi
+-rw-rw-rw-   0        0        0     2833 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Valuator.pyi
+-rw-rw-rw-   0        0        0     1186 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/VectorWidgets.pyi
+-rw-rw-rw-   0        0        0     1181 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/WidgetPropertiesDialog.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:09.000000 types-panda3d-0.3.3/src/direct-stubs/tkwidgets/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.238842 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/
+-rw-rw-rw-   0        0        0     2192 2023-07-07 18:43:38.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/ViewPort.pyi
+-rw-rw-rw-   0        0        0      922 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxAppShell.pyi
+-rw-rw-rw-   0        0        0     1652 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxPandaShell.pyi
+-rw-rw-rw-   0        0        0       27 2022-10-01 23:45:06.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxPandaStart.pyi
+-rw-rw-rw-   0        0        0     1107 2023-05-21 03:12:15.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxPandaWindow.pyi
+-rw-rw-rw-   0        0        0      934 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxSlider.pyi
+-rw-rw-rw-   0        0        0        0 2023-03-31 00:14:08.000000 types-panda3d-0.3.3/src/direct-stubs/wxwidgets/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.256384 types-panda3d-0.3.3/src/panda3d-stubs/
+-rw-rw-rw-   0        0        0        0 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/__init__.pyi
+-rw-rw-rw-   0        0        0    56745 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/_rplight.pyi
+-rw-rw-rw-   0        0        0     1875 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/_typing.pyi
+-rw-rw-rw-   0        0        0    11439 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/ai.pyi
+-rw-rw-rw-   0        0        0   116158 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/bullet.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.317887 types-panda3d-0.3.3/src/panda3d-stubs/core/
+-rw-rw-rw-   0        0        0     1513 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/__init__.pyi
+-rw-rw-rw-   0        0        0    20270 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_audio.pyi
+-rw-rw-rw-   0        0        0    51681 2023-07-07 21:36:08.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_chan.pyi
+-rw-rw-rw-   0        0        0    14908 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_char.pyi
+-rw-rw-rw-   0        0        0    64802 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_collide.pyi
+-rw-rw-rw-   0        0        0    27884 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_device.pyi
+-rw-rw-rw-   0        0        0     2598 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_dgraph.pyi
+-rw-rw-rw-   0        0        0   192923 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_display.pyi
+-rw-rw-rw-   0        0        0   109048 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_downloader.pyi
+-rw-rw-rw-   0        0        0    20469 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_dtoolbase.pyi
+-rw-rw-rw-   0        0        0    73270 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_dtoolutil.pyi
+-rw-rw-rw-   0        0        0    39841 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_dxml.pyi
+-rw-rw-rw-   0        0        0    57853 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_event.pyi
+-rw-rw-rw-   0        0        0   148663 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_express.pyi
+-rw-rw-rw-   0        0        0   500809 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_gobj.pyi
+-rw-rw-rw-   0        0        0    78156 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_grutil.pyi
+-rw-rw-rw-   0        0        0     3586 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_gsgbase.pyi
+-rw-rw-rw-   0        0        0   233377 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_linmath.pyi
+-rw-rw-rw-   0        0        0    98712 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_mathutil.pyi
+-rw-rw-rw-   0        0        0    26352 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_movies.pyi
+-rw-rw-rw-   0        0        0    12136 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_nativenet.pyi
+-rw-rw-rw-   0        0        0    45088 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_net.pyi
+-rw-rw-rw-   0        0        0    73635 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_parametrics.pyi
+-rw-rw-rw-   0        0        0   537021 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pgraph.pyi
+-rw-rw-rw-   0        0        0    37640 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pgraphnodes.pyi
+-rw-rw-rw-   0        0        0    62209 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pgui.pyi
+-rw-rw-rw-   0        0        0    32473 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pipeline.pyi
+-rw-rw-rw-   0        0        0    94473 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pnmimage.pyi
+-rw-rw-rw-   0        0        0    13360 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pnmtext.pyi
+-rw-rw-rw-   0        0        0    84958 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_prc.pyi
+-rw-rw-rw-   0        0        0    21666 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_pstatclient.pyi
+-rw-rw-rw-   0        0        0   162901 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_putil.pyi
+-rw-rw-rw-   0        0        0    11810 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_recorder.pyi
+-rw-rw-rw-   0        0        0    92666 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_text.pyi
+-rw-rw-rw-   0        0        0    69546 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/core/_tform.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.329282 types-panda3d-0.3.3/src/panda3d-stubs/direct/
+-rw-rw-rw-   0        0        0      161 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/__init__.pyi
+-rw-rw-rw-   0        0        0    62968 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_dcparser.pyi
+-rw-rw-rw-   0        0        0    19472 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_deadrec.pyi
+-rw-rw-rw-   0        0        0    15098 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_distributed.pyi
+-rw-rw-rw-   0        0        0    49674 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_interval.pyi
+-rw-rw-rw-   0        0        0     3863 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_motiontrail.pyi
+-rw-rw-rw-   0        0        0     1067 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/direct/_showbase.pyi
+-rw-rw-rw-   0        0        0       30 2023-03-31 00:14:23.000000 types-panda3d-0.3.3/src/panda3d-stubs/dtoolconfig.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.334242 types-panda3d-0.3.3/src/panda3d-stubs/egg/
+-rw-rw-rw-   0        0        0       45 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/egg/__init__.pyi
+-rw-rw-rw-   0        0        0   237550 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/egg/_egg.pyi
+-rw-rw-rw-   0        0        0      771 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/egg/_egg2pg.pyi
+-rw-rw-rw-   0        0        0    24860 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/fx.pyi
+-rw-rw-rw-   0        0        0    12596 2023-03-31 00:14:23.000000 types-panda3d-0.3.3/src/panda3d-stubs/interrogatedb.pyi
+-rw-rw-rw-   0        0        0    65375 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/ode.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.339699 types-panda3d-0.3.3/src/panda3d-stubs/physics/
+-rw-rw-rw-   0        0        0       57 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/physics/__init__.pyi
+-rw-rw-rw-   0        0        0    49283 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/physics/_particlesystem.pyi
+-rw-rw-rw-   0        0        0    39711 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/physics/_physics.pyi
+-rw-rw-rw-   0        0        0     2390 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/skel.pyi
+-rw-rw-rw-   0        0        0     4617 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/vision.pyi
+-rw-rw-rw-   0        0        0     1052 2023-07-07 21:36:09.000000 types-panda3d-0.3.3/src/panda3d-stubs/vrpn.pyi
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.347138 types-panda3d-0.3.3/src/types_panda3d.egg-info/
+-rw-rw-rw-   0        0        0     2606 2023-07-08 17:02:57.000000 types-panda3d-0.3.3/src/types_panda3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    18014 2023-07-08 17:02:57.000000 types-panda3d-0.3.3/src/types_panda3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 17:02:57.000000 types-panda3d-0.3.3/src/types_panda3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-08 17:02:57.000000 types-panda3d-0.3.3/src/types_panda3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-08 17:02:57.000000 types-panda3d-0.3.3/src/types_panda3d.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 17:02:58.348626 types-panda3d-0.3.3/tests/
+-rw-rw-rw-   0        0        0     1964 2023-03-30 23:50:39.000000 types-panda3d-0.3.3/tests/test_stubtest.py
```

### Comparing `types-panda3d-0.3.2/LICENSE` & `types-panda3d-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/PKG-INFO` & `types-panda3d-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-panda3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: Type stubs for the Panda3D Python bindings
 Author: W. M. Okiishi
 License: Copyright (c) 2022 W. M. Okiishi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `types-panda3d-0.3.2/README.md` & `types-panda3d-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/pyproject.toml` & `types-panda3d-0.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "types-panda3d"
-version = "0.3.2"
+version = "0.3.3"
 authors = [ { name = "W. M. Okiishi" } ]
 description = "Type stubs for the Panda3D Python bindings"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 dependencies = ["panda3d==1.10.13"]
 classifiers = [
@@ -33,24 +33,27 @@
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 combine_as_imports = true
 extra_standard_library = ["typing_extensions"]
 
 [tool.black]
+preview = true
 line_length = 130
-target_version = ["py310"]
+target_version = ["py311"]
 force_exclude = "/(tests|idbstubs)/"
 skip_string_normalization = true
 skip_magic_trailing_comma = true
 
 [tool.mypy]
 show_error_codes = true
 warn_unused_ignores = true
 enable_incomplete_feature = ["TypeVarTuple", "Unpack"]
 
 [tool.pyright]
 stubPath = "src"
 reportSelfClsParameterName = false
 # We use illusory modules to break up large modules, as well as to
-# store often-used typing constructors.
+# store often-used typing constructs.
 reportMissingModuleSource = false
+# Pmw throws Pyright off.
+useLibraryCodeForTypes = false
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/actor/Actor.pyi` & `types-panda3d-0.3.3/src/direct-stubs/actor/Actor.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from direct.interval.ActorInterval import ActorInterval
 from direct.showbase.DirectObject import DirectObject
 from direct.tkpanels.AnimPanel import AnimPanel
 from panda3d._typing import Vec3Like
 from panda3d.core import (
     AnimBundle,
     AnimControl,
-    AnimGroup,
     Character,
     ConfigVariableBool,
     GeomNode,
     LMatrix4f,
     Loader,
     LoaderOptions,
     LODNode,
     ModelNode,
     NodePath,
     PandaNode,
     PartBundle,
     PartBundleHandle,
+    PartGroup,
     PartSubset,
     TransformState,
 )
 
 _BlendType: TypeAlias = Literal[0, 1, 2, 3]
 _NodePathOrFilepath: TypeAlias = NodePath[PandaNode] | StrOrBytesPath
 
@@ -70,15 +70,15 @@
         subset: PartSubset
         def __init__(self, truePartName: str, subset: PartSubset = ...) -> None: ...
         def makeCopy(self) -> Actor.SubpartDef: ...
 
     def __init__(
         self,
         models: dict[str, dict[str, _NodePathOrFilepath] | _NodePathOrFilepath] | _NodePathOrFilepath | None = None,
-        anims: dict[str, Mapping[str, str]] | Mapping[str, str] | None = None,
+        anims: Mapping[str, dict[str, str]] | Mapping[str, str] | None = None,
         other: Actor | None = None,
         copy: bool = True,
         lodNode: LODNode | None = None,
         flattenable: bool = True,
         setFinal: bool = False,
         mergeLODBundles: bool | None = None,
         allowAsyncBind: bool | None = None,
@@ -97,59 +97,59 @@
     def flush(self) -> None: ...
     def get_anim_control_dict(self) -> dict[str, dict[str, dict[str, Actor.AnimDef]]]: ...
     def remove_anim_control_dict(self) -> None: ...
     def get_part_bundle_dict(self) -> dict[str, dict[str, Actor.PartDef]]: ...
     def get_part_bundles(self, partName: str | None = None) -> list[PartBundle]: ...
     def get_lod_names(self) -> list[str]: ...
     def get_part_names(self) -> list[str]: ...
-    def get_geom_node(self) -> GeomNode: ...
-    def set_geom_node(self, node: GeomNode) -> None: ...
+    def get_geom_node(self) -> NodePath[GeomNode]: ...
+    def set_geom_node(self, node: NodePath[GeomNode]) -> None: ...
     def get_lod_node(self) -> LODNode: ...
     def set_lod_node(self, node: LODNode | None = None) -> None: ...
     def use_lod(self, lodName: object) -> None: ...
     def print_lod(self) -> None: ...
     def reset_lod(self) -> None: ...
     def add_lod(self, lodName: str, inDist: float = 0, outDist: float = 0, center: Vec3Like | None = None) -> None: ...
     def set_lod(self, lodName: str, inDist: float = 0, outDist: float = 0) -> None: ...
     def get_lod_index(self, lodName: str) -> int: ...
     def get_lod(self, lodName: str) -> NodePath | None: ...
     def has_lod(self) -> bool: ...
     def set_center(self, center: Vec3Like | None) -> None: ...
     def set_lod_animation(self, farDistance: float, nearDistance: float, delayFactor: float) -> None: ...
     def clear_lod_animation(self) -> None: ...
     def update(self, lod: int = 0, partName: str | None = None, lodName: str | None = None, force: bool = False) -> bool: ...
-    def get_frame_rate(self, animName: str | None = None, partName: str | None = None) -> float: ...
-    def get_base_frame_rate(self, animName: str | None = None, partName: str | None = None) -> float: ...
-    def get_play_rate(self, animName: str | None = None, partName: str | None = None) -> float: ...
+    def get_frame_rate(self, animName: str | None = None, partName: str | None = None) -> float | None: ...
+    def get_base_frame_rate(self, animName: str | None = None, partName: str | None = None) -> float | None: ...
+    def get_play_rate(self, animName: str | None = None, partName: str | None = None) -> float | None: ...
     def set_play_rate(self, rate: float, animName: str, partName: str | None = None) -> None: ...
     def get_duration(
         self,
         animName: str | None = None,
         partName: str | None = None,
         fromFrame: float | None = None,
         toFrame: float | None = None,
     ) -> float | None: ...
-    def get_num_frames(self, animName: str | None = None, partName: str | None = None) -> int: ...
+    def get_num_frames(self, animName: str | None = None, partName: str | None = None) -> int | None: ...
     def get_frame_time(self, anim: str | None, frame: SupportsFloat, partName: str | None = None) -> float: ...
     def get_current_anim(self, partName: str | None = None) -> str | None: ...
-    def get_current_frame(self, animName: str | None = None, partName: str | None = None) -> int: ...
-    def get_part(self, partName: str, lodName: str = 'lodRoot') -> NodePath[Character]: ...
+    def get_current_frame(self, animName: str | None = None, partName: str | None = None) -> int | None: ...
+    def get_part(self, partName: str, lodName: str = 'lodRoot') -> NodePath[Character] | None: ...
     def get_part_bundle(self, partName: str, lodName: str = 'lodRoot') -> PartBundle | None: ...
     def remove_part(self, partName: str, lodName: str = 'lodRoot') -> None: ...
     def hide_part(self, partName: str, lodName: str = 'lodRoot') -> None: ...
     def show_part(self, partName: str, lodName: str = 'lodRoot') -> None: ...
     def show_all_parts(self, partName: str, lodName: str = 'lodRoot') -> None: ...
     def expose_joint(
         self, node: NodePath, partName: str, jointName: str, lodName: str = 'lodRoot', localTransform: bool = ...
     ) -> NodePath | None: ...
     def stop_joint(self, partName: str, jointName: str, lodName: str = 'lodRoot') -> None: ...
-    def get_joints(self, partName: str | None = None, jointName: str = '*', lodName: str | None = None) -> list[AnimGroup]: ...
+    def get_joints(self, partName: str | None = None, jointName: str = '*', lodName: str | None = None) -> list[PartGroup]: ...
     def get_overlapping_joints(
         self, partNameA: str, partNameB: str, jointName: str = '*', lodName: str | None = None
-    ) -> set[AnimGroup]: ...
+    ) -> set[PartGroup]: ...
     def get_joint_transform(self, partName: str, jointName: str, lodName: str = 'lodRoot') -> LMatrix4f | None: ...
     def get_joint_transform_state(self, partName: str, jointName: str, lodName: str = 'lodRoot') -> TransformState | None: ...
     def control_joint(
         self, node: NodePath | None, partName: str, jointName: str, lodName: str = 'lodRoot'
     ) -> NodePath[ModelNode]: ...
     def freeze_joint(
         self,
@@ -157,15 +157,15 @@
         jointName: str,
         transform: TransformState | None = None,
         pos: Vec3Like = ...,
         hpr: Vec3Like = ...,
         scale: Vec3Like = ...,
     ) -> None: ...
     def release_joint(self, partName: str, jointName: str) -> None: ...
-    def instance(self, path: NodePath, partName: str, jointName: str, lodName: str = 'lodRoot') -> None: ...
+    def instance(self, path: NodePath, partName: str, jointName: str, lodName: str = 'lodRoot') -> NodePath | None: ...
     def attach(self, partName: str, anotherPartName: str, jointName: str, lodName: str = 'lodRoot') -> None: ...
     def draw_in_front(
         self, frontPartName: str, backPartName: str, mode: int, root: NodePath | None = None, lodName: str | None = None
     ) -> None: ...
     def fix_bounds(self, partName: str | None = None) -> None: ...
     def fix_bounds_old(self, part: NodePath | None = None) -> None: ...
     def show_all_bounds(self) -> None: ...
@@ -220,22 +220,22 @@
         okMissing: bool | None = None,
         autoBindAnims: bool = True,
     ) -> None: ...
     def make_subpart(
         self,
         partName: str,
         includeJoints: Iterable[str],
-        excludeJoints: Iterable[str] = ...,
+        excludeJoints: Iterable[str] = [],
         parent: str = 'modelRoot',
         overlapping: bool = False,
     ) -> None: ...
     def set_subparts_complete(self, flag: bool) -> None: ...
     def get_subparts_complete(self) -> bool: ...
     def verify_subparts_complete(self, partName: str | None = None, lodName: str | None = None) -> None: ...
-    def load_anims(self, anims: Mapping[str, str], partName: str = 'modelRoot', lodName: str = 'lodRoot') -> None: ...
+    def load_anims(self, anims: Mapping[str, NodePath | str], partName: str = 'modelRoot', lodName: str = 'lodRoot') -> None: ...
     def init_anims_on_all_lods(self, partNames: Iterable[str]) -> None: ...
     def load_anims_on_all_lods(self, anims: Mapping[str, str], partName: str = 'modelRoot') -> None: ...
     def post_flatten(self) -> None: ...
     def unload_anims(
         self, anims: Iterable[str] | None = None, partName: str | None = None, lodName: str | None = None
     ) -> None: ...
     def bind_anim(
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterClient.pyi` & `types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterClient.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -76,18 +76,18 @@
     def addObjectTag(
         self, object: str, selectFunction: Any, deselectFunction: Any, selectArgs: Any, deselectArgs: Any
     ) -> None: ...
     def removeObjectTag(self, object: str) -> None: ...
     def selectNodePath(self, nodePath: NodePath) -> None: ...
     def deselectNodePath(self, nodePath: NodePath) -> None: ...
     def sendCamFrustum(
-        self, focalLength: float, filmSize: LVecBase2f, filmOffset: LVecBase2f, indexList: Iterable[int] = ...
+        self, focalLength: float, filmSize: LVecBase2f, filmOffset: LVecBase2f, indexList: Iterable[int] = []
     ) -> None: ...
     def loadModel(self, nodePath: Unused) -> None: ...
-    def __call__(self, commandString: str, fLocally: bool = ..., serverList: Iterable[int] = ...) -> None: ...
+    def __call__(self, commandString: str, fLocally: bool = ..., serverList: Iterable[int] = []) -> None: ...
     def handleDatagram(self, dgi: DatagramIterator, type: int, server: int) -> int: ...
     def handleMessageQueue(self, server: int) -> None: ...
     def handleNamedMovement(self, data: _NamedMovement) -> None: ...
     def exit(self) -> NoReturn: ...
 
 class ClusterClientSync(ClusterClient):
     waitForSwap: bool
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterMsgs.pyi` & `types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterMsgs.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/cluster/ClusterServer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/cluster/ClusterServer.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/ControlManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/ControlManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/DevWalker.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/DevWalker.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/GravityWalker.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/GravityWalker.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/InputState.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/InputState.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/NonPhysicsWalker.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/NonPhysicsWalker.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/controls/PhysicsWalker.pyi` & `types-panda3d-0.3.3/src/direct-stubs/controls/PhysicsWalker.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectDeviceManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectDeviceManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectFastrak.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectFastrak.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectJoybox.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectJoybox.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 JOYBOX_TREAD_SEPERATION: Final = 1.0
 
 class DirectJoybox(DirectObject):
     joyboxCount: ClassVar[int]
     xyzMultiplier: ClassVar[float]
     hprMultiplier: ClassVar[float]
     name: str
-    devie: str
+    device: str
     analogs: DirectAnalogs
     buttons: DirectButtons
     aList: list[float]
     bList: list[bool]
     mapping: list[int]
     modifier: list[Literal[-1, 0, 1]]
     lastTime: float
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directdevices/DirectRadamec.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directdevices/DirectRadamec.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 RAD_ZOOM: Final = 2
 RAD_FOCUS: Final = 3
 
 class DirectRadamec(DirectObject):
     radamecCount: ClassVar[int]
     notify: ClassVar[Notifier]
     name: str
-    devie: str
+    device: str
     analogs: DirectAnalogs
     numAnalogs: int
     aList: list[float]
     minRange: list[float]
     maxRange: list[float]
     def __init__(self, device: str = 'Analog0', nodePath: Unused = None) -> None: ...
     def enable(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directnotify/DirectNotify.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ReferrerSearch.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from tkinter import Toplevel
-from typing import Any, ClassVar, Protocol
+from collections.abc import Generator, Reversible, Sized
+from typing import Any
 
-from .Logger import Logger
-from .Notifier import Notifier
+from .Job import Job
 
-class _SupportsNotify(Protocol):
-    __name__: ClassVar[str]
-    notify: ClassVar[Notifier]
-
-class DirectNotify:
-    logger: Logger
-    streamWriter: Any
-    def __init__(self) -> None: ...
-    def getCategories(self) -> list[str]: ...
-    def getCategory(self, categoryName: str) -> Notifier | None: ...
-    def newCategory(self, categoryName: str, logger: Logger | None = None) -> Notifier: ...
-    def setDconfigLevel(self, categoryName: str) -> None: ...
-    def setDconfigLevels(self) -> None: ...
-    def setVerbose(self) -> None: ...
-    def popupControls(self, tl: Toplevel | None = None) -> None: ...
-    def giveNotify(self, cls: type[_SupportsNotify]) -> None: ...
+class ReferrerSearch(Job):
+    obj: object
+    maxRefs: int
+    visited: set[int]
+    depth: int
+    found: int
+    shouldPrintStats: bool
+    def __init__(self, obj: object, maxRefs: int = 100) -> None: ...
+    def __call__(self) -> None: ...
+    def run(self) -> Generator[Any | None, None, None]: ...
+    def __del__(self) -> None: ...
+    def truncateAtNewLine(self, s: str) -> str: ...
+    def printStatsWhenAble(self) -> None: ...
+    def myrepr(self, referrer: object, refersTo: object) -> str: ...
+    def step(self, depth: int, path: Reversible[object]) -> None: ...
+    def stepGenerator(self, depth: int, path: Reversible[object]) -> None: ...
+    def printStats(self, path: Reversible[object]) -> None: ...
+    def isAtRoot(self, at: object, path: Reversible[object]) -> bool: ...
+    def isManyRef(self, at: object, path: Reversible[object], referrers: Sized) -> bool | None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directnotify/Notifier.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directnotify/Notifier.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directnotify/RotatingLog.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directnotify/RotatingLog.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     sizeLimit: float | None
     def __init__(self, path: str = './log_file', hourInterval: float | None = 24, megabyteLimit: float | None = 1024) -> None: ...
     def __del__(self) -> None: ...
     def close(self) -> None: ...
     def shouldRotate(self) -> bool: ...
     def filePath(self) -> str: ...
     def rotate(self) -> None: ...
-    def write(self, data: str) -> int: ...
+    def write(self, data: str) -> int | None: ...
     def flush(self) -> None: ...
     def fileno(self) -> int: ...
     def isatty(self) -> bool: ...
     def __next__(self) -> str: ...
     next = __next__
     def read(self, size: int | None) -> str: ...
     def readline(self, size: int) -> str: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directscripts/eggcacher.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directscripts/eggcacher.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from collections.abc import Iterable, Sequence
-from typing_extensions import Literal
 
 from panda3d.core import BamCache, Loader, LoaderOptions
 
 class EggCacher:
     bamcache: BamCache
     pandaloader: Loader
     loaderopts: LoaderOptions
@@ -12,8 +11,8 @@
     paths: Sequence[str]
     def __init__(self, args: Sequence[str]) -> None: ...
     def parseArgs(self, args: Sequence[str]) -> None: ...
     def scanPath(self, eggs: list[tuple[str, int]], path: str) -> None: ...
     def scanPaths(self, paths: Iterable[str]) -> list[tuple[str, int]]: ...
     def processFiles(self, files: Iterable[tuple[str, int]]) -> None: ...
 
-def main(args: Sequence[str] | None = None) -> Literal[0]: ...
+def main(args: Sequence[str] | None = None) -> int: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directscripts/extract_docs.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directscripts/extract_docs.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directscripts/gendocs.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directscripts/gendocs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import Container, Iterable, MutableSequence, Sequence
 from re import Pattern
 from typing import overload
-from typing_extensions import Final, Literal, Never
+from typing_extensions import Final, Never
 
 SECHEADER: Final[Pattern[str]]
 JUNKHEADER: Final[Pattern[str]]
 IMPORTSTAR: Final[Pattern[str]]
 IDENTIFIER: Final[Pattern[str]]
 FILEHEADER: Final[Pattern[str]]
 
@@ -74,15 +74,15 @@
     enumvalues: list[InterrogateEnumValue]
     nested: list[int]
     comment: str
     def __init__(self, tokzr: InterrogateTokenizer, db: InterrogateDatabase) -> None: ...
 
 class InterrogateParameter:
     name: str
-    parameteflags: int
+    parameterflags: int
     type: int
     def __init__(self, tokzr: InterrogateTokenizer) -> None: ...
 
 class InterrogateWrapper:
     db: InterrogateDatabase
     index: int
     componentname: str
@@ -120,17 +120,15 @@
     class_info: dict[str, ParseTreeInfo]
     function_info: dict[str, ParseTreeInfo]
     assign_info: dict
     derivs: dict
     prototype: str
     def __init__(self, tree, name: str, file) -> None: ...
     @overload
-    def match(self, pattern: list[str], data: str, vars: dict | None) -> tuple[Literal[True], dict]: ...
-    @overload
-    def match(self, pattern: str, data: str, vars: dict | None = None) -> tuple[bool, dict]: ...
+    def match(self, pattern: str | list[str], data: str, vars: dict | None = None) -> tuple[bool, dict]: ...
     @overload
     def match(self, pattern: tuple[str, ...], data: Sequence[str], vars: dict | None = None) -> tuple[bool, dict]: ...
     def extract_info(self, tree: Sequence[str]) -> None: ...
     def extract_derivs(self, classinfo: ParseTreeInfo, tree) -> None: ...
     def extract_tokens(self, str: str, tree) -> str: ...
 
 class CodeDatabase:
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectCameraControl.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectCameraControl.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGeometry.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGeometry.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGlobals.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGlobals.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectGrid.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectGrid.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     gridSpacing: float
     snapAngle: float
     fEnabled: bool
     def __init__(
         self,
         gridSize: float = 100.0,
         gridSpacing: float = 5.0,
-        planeColor: Vec3Like | Vec4Like = ...,
+        planeColor: Vec3Like | Vec4Like = (0.5, 0.5, 0.5, 0.5),
         parent: NodePath | None = None,
     ) -> None: ...
     def enable(self, parent: NodePath | None = None) -> None: ...
     def disable(self) -> None: ...
     def toggleGrid(self, parent: NodePath | None = None) -> None: ...
     def isEnabled(self) -> bool: ...
     def updateGrid(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectLights.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectLights.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectManipulation.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectManipulation.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectSelection.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectSelection.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -143,21 +143,21 @@
     ) -> CollisionEntry: ...
 
 class SelectionSegment(SelectionQueue):
     colliders: list[CollisionSolid]
     numColliders: int
     def __init__(self, parentNP: NodePath | None = None, numSegments: int = 1) -> None: ...
     def pickGeom(
-        self, targetNodePath: NodePath | None = None, endPointList: Sequence[tuple[Vec3Like, Vec3Like]] = ..., skipFlags: int = 5
+        self, targetNodePath: NodePath | None = None, endPointList: Sequence[tuple[Vec3Like, Vec3Like]] = [], skipFlags: int = 5
     ) -> CollisionEntry: ...
     def pickBitMask(
         self,
         bitMask: BitMask32 = ...,
         targetNodePath: NodePath | None = None,
-        endPointList: Sequence[tuple[Vec3Like, Vec3Like]] = ...,
+        endPointList: Sequence[tuple[Vec3Like, Vec3Like]] = [],
         skipFlags: int = 5,
     ) -> CollisionEntry: ...
 
 class SelectionSphere(SelectionQueue):
     colliders: list[CollisionSolid]
     numColliders: int
     def __init__(self, parentNP: NodePath | None = None, numSpheres: int = 1) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectSession.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectSession.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     undoList: list[list[tuple[NodePath, TransformState]]]
     redoList: list[list[tuple[NodePath, TransformState]]]
     actionEvents: list[Sequence[Any]]
     modifierEvents: list[str]
     specialKeys: list[str]
     keyEvents: list[str]
     mouseEvents: list[str]
-    directiOnlyKeyMap: dict[str, tuple[str, str]]
+    directOnlyKeyMap: dict[str, tuple[str, str]]
     hotKeyMap: dict[str, tuple[str, str]]
     specialKeyMap: dict[str, str]
     passThroughKeys: list[str]
     panel: DirectSessionPanel
     clusterMode: str
     def __init__(self) -> None: ...
     def addPassThroughKey(self, key: str) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directtools/DirectUtil.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directtools/DirectUtil.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directutil/DistributedLargeBlobSender.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directutil/DistributedLargeBlobSender.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/directutil/Mopath.pyi` & `types-panda3d-0.3.3/src/direct-stubs/directutil/Mopath.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/dist/FreezeTool.pyi` & `types-panda3d-0.3.3/src/direct-stubs/dist/FreezeTool.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     PSDK: str | None
     MD: str | None
     suffix64: str
     dllext: str
     arch: str
     def __init__(self, platform: str) -> None: ...
     def determineStandardSetup(self) -> None: ...
-    def compileExe(self, filename: object, basename: object, extraLink: Iterable[str] = ...) -> None: ...
-    def compileDll(self, filename: object, basename: object, extraLink: Iterable[str] = ...) -> None: ...
+    def compileExe(self, filename: object, basename: object, extraLink: Iterable[str] = []) -> None: ...
+    def compileDll(self, filename: object, basename: object, extraLink: Iterable[str] = []) -> None: ...
 
 frozenMainCode: str
 frozenDllMainCode: str
 mainInitCode: str
 dllInitCode: str
 programFile: str
 okMissing: list[str]
@@ -125,15 +125,15 @@
     def writeCode(self, filename: _OpenFile | None, initCode: str = '') -> None: ...
     def generateCode(self, basename: str, compileToExe: bool = False) -> str: ...
     def generateRuntimeFromStub(
         self,
         target: _OpenFileT,
         stub_file: SupportsRead[bytes],
         use_console: bool,
-        fields: Mapping[str, str | None] = ...,
+        fields: Mapping[str, str | None] = {},
         log_append: bool = False,
         log_filename_strftime: bool = False,
     ) -> _OpenFileT: ...
     def makeModuleDef(self, mangledName: str, code: bytes) -> str: ...
     def makeModuleListEntry(self, mangledName: str, code: bytes, moduleName: str, module: object) -> str: ...
     def makeForbiddenModuleListEntry(self, moduleName: str) -> str: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/dist/commands.pyi` & `types-panda3d-0.3.3/src/direct-stubs/dist/commands.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/dist/pefile.pyi` & `types-panda3d-0.3.3/src/direct-stubs/dist/pefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     class Icon(NamedTuple):
         width: int
         height: int
         planes: int
         bpp: int
         size: int
         id: int
+
     code_page: ClassVar[int]
     type: ClassVar[int]
     icons: list[IconGroupResource.Icon]
     def __init__(self) -> None: ...
     def add_icon(self, width: int, height: int, planes: int, bpp: int, size: int, id: int) -> None: ...
     def get_data(self) -> bytearray: ...
     def unpack_from(self, data: ReadableBuffer, offs: int = 0) -> None: ...
@@ -116,15 +117,15 @@
     def __getitem__(self, key: Literal['VarFileInfo']) -> dict[str, bytearray]: ...
     def __contains__(self, key: object) -> bool: ...
 
 class ResourceTable:
     flags: int
     timdat: int
     version: tuple[int, int]
-    def __init__(self, ident: tuple[int | str, ...] = ...) -> None: ...
+    def __init__(self, ident: tuple[int | str, ...] = ()) -> None: ...
     def __getitem__(self, key: int | str) -> ResourceTable: ...
     def __setitem__(self, key: int | str, value: ResourceTable) -> None: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[int | str]: ...
     def items(self) -> list[tuple[int | str, ResourceTable | None]]: ...
     def count_resources(self) -> int: ...
     def get_nested_tables(self) -> Generator[ResourceTable, None, None]: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/AsyncRequest.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/AsyncRequest.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/CRCache.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/CRCache.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/CartesianGridBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/CartesianGridBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ClientRepository.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ClientRepository.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def createReady(self) -> None: ...
     def handleRequestGenerates(self, di: DatagramIterator) -> None: ...
     def resendGenerate(self, obj: DistributedObjectBase) -> None: ...
     def handleGenerate(self, di: DatagramIterator) -> None: ...
     def allocateDoId(self) -> int: ...
     def reserveDoId(self, doId: int) -> int: ...
     def freeDoId(self, doId: int) -> None: ...
-    def storeObjectLocation(self, object: DistributedObjectBase, parentId: int, zoneId: int) -> None: ...  # type: ignore[override]
+    def storeObjectLocation(self, object: DistributedObjectBase, parentId: int | None, zoneId: int | None) -> None: ...
     def createDistributedObject(
         self,
         className: str | None = None,
         distObj: DistributedObjectBase | None = None,
         zoneId: int = 0,
         optionalFields: Sequence[str] | None = None,
         doId: int | None = None,
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ClientRepositoryBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ClientRepositoryBase.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,12 +80,12 @@
     def getObjectsOfClass(self, objClass: type[_D]) -> dict[int, _D]: ...
     def getObjectsOfExactClass(self, objClass: type[_D]) -> dict[int, _D]: ...
     def considerHeartbeat(self) -> None: ...
     def stopHeartbeat(self) -> None: ...
     def startHeartbeat(self) -> None: ...
     def sendHeartbeatTask(self, task: Unused) -> Literal[2]: ...
     def waitForNextHeartBeat(self) -> None: ...
-    def replaceMethod(self, oldMethod: Unused, newFunction: Unused) -> Literal[0]: ...
+    def replaceMethod(self, oldMethod: Unused, newFunction: Unused) -> int: ...
     def getWorld(self, doId: int) -> NodePath | None: ...
     def isLive(self) -> bool: ...
     def isLocalId(self, id: int) -> bool: ...
     def printDelayDeletes(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ClockDelta.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ClockDelta.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import ClassVar
-from typing_extensions import Final, Literal
+from typing_extensions import Final
 
 from direct.directnotify.Notifier import Notifier
 from direct.showbase.DirectObject import DirectObject
 from panda3d.core import ClockObject
 
-NetworkTimeBits: Literal[16]
+NetworkTimeBits: Final = 16
 NetworkTimePrecision: float
-NetworkTimeMask: Literal[65535]
-NetworkTimeSignedMask: Literal[32767]
-NetworkTimeTopBits: Literal[16]
+NetworkTimeMask: Final = 65535
+NetworkTimeSignedMask: Final = 32767
+NetworkTimeTopBits: Final = 16
 MaxTimeDelta: float
 ClockDriftPerHour: float
 ClockDriftPerSecond: float
 P2PResyncDelay: float
 
 globalClockDelta: Final[ClockDelta]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ConnectionRepository.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ConnectionRepository.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     def readDCFile(self, dcFileNames: str | Iterable[StrOrBytesPath] | None = None) -> None: ...
     def importModule(self, dcImports, moduleName: str, importSymbols: Sequence[str]) -> None: ...
     def getServerAddress(self) -> str: ...
     def connect(
         self,
         serverList: Sequence[str],
         successCallback: Callable[..., object] | None = None,
-        successArgs: Iterable[Any] = ...,
+        successArgs: Iterable[Any] = [],
         failureCallback: Callable[..., object] | None = None,
-        failureArgs: Iterable[Any] = ...,
+        failureArgs: Iterable[Any] = [],
     ) -> None: ...
     def httpConnectCallback(
         self,
         ch: HTTPChannel,
         serverList: Sequence[str],
         serverIndex: int,
         successCallback: Callable[..., object],
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCamera.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCamera.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def exitOff(self) -> None: ...
     def enterOff(self) -> None: ...
     def enterStandby(self) -> None: ...
     def enterBlinking(self) -> None: ...
     def exitBlinking(self) -> None: ...
     def enterRecording(self) -> None: ...
     def exitRecording(self) -> None: ...
-    def enterUsing(self, args: Sequence[Unused] = ...) -> None: ...
+    def enterUsing(self, args: Sequence[Unused] = []) -> None: ...
     def exitUsing(self) -> None: ...
 
 class DistributedCamera(DistributedObject):
     parent: NodePath | None
     fixtures: dict[int, Fixture]
     cameraId: int
     def __getitem__(self, index: int) -> Fixture: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCameraOV.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCameraOV.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCartesianGrid.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCartesianGrid.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     gridVisContext: InterestHandle | None
     cellWidth: float
     style = ...
     startingZone: int
     gridSize: int
     viewingRadius: int
     centerPos: LVector3f
-    def isGridParent(self) -> Literal[True]: ...
     def setCellWidth(self, width: float) -> None: ...
     def setParentingRules(self, style, rule: str) -> None: ...
     def getCenterPos(self) -> LVector3f: ...
     def handleChildArrive(self, child: _HasGridParent, zoneId: int) -> None: ...
     def handleChildArriveZone(self, child: _HasGridParent, zoneId: int) -> None: ...
     def handleChildLeave(self, child: _HasGridParent, zoneId: int) -> None: ...
     def startProcessVisibility(self, avatar) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedCartesianGridAI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedCartesianGridAI.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         air: ClientRepository,
         startingZone: int,
         gridSize: int,
         gridRadius: float,
         cellWidth: float,
         style: str = 'Cartesian',
     ) -> None: ...
-    def isGridParent(self) -> Literal[True]: ...
     def getCellWidth(self) -> float: ...
     def getParentingRules(self) -> tuple[str, str]: ...
     def addObjectToGrid(self, av, useZoneId: int = -1, startAutoUpdate: bool = True) -> None: ...
     def removeObjectFromGrid(self, av) -> None: ...
     def startUpdateGridTask(self) -> None: ...
     def stopUpdateGridTask(self) -> None: ...
     def updateGridTask(self, task: AsyncTask | None = None) -> Literal[2]: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNode.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNode.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class DistributedNode(DistributedObject, NodePath):
     DistributedNode_initialized: Literal[1]
     DistributedNode_deleted: Literal[1]
     gotStringParentToken: bool
     gridParent: GridParent | None
     def __init__(self, cr: ClientRepository) -> None: ...
-    def setLocation(self, parentId: int, zoneId: int, teleport: bool = ...) -> None: ...  # type: ignore[override]
+    def setLocation(self, parentId: int | None, zoneId: int | None, teleport: bool = ...) -> None: ...
     def __cmp__(self, other: object) -> Literal[0, 1]: ...
     def b_setParent(self, parentToken: str | int) -> None: ...
     def d_setParent(self, parentToken: str | int) -> None: ...
     def setParentStr(self, parentTokenStr: str) -> None: ...
     def setParent(self, parentToken: int) -> None: ...
     def do_setParent(self, parentToken: int) -> None: ...
     def d_setX(self, x: float) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNodeAI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNodeAI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedNodeUD.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedNodeUD.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObject.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObject.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,20 @@
     def generate(self) -> None: ...
     def generateInit(self) -> None: ...
     def getDoId(self) -> int: ...
     def postGenerateMessage(self) -> None: ...
     def updateRequiredFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
     def updateAllRequiredFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
     def updateRequiredOtherFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
-    def sendUpdate(self, fieldName: str, args=..., sendToId: int | None = None) -> None: ...
+    def sendUpdate(self, fieldName: str, args=[], sendToId: int | None = None) -> None: ...
     def sendDisableMsg(self) -> None: ...
     def sendDeleteMsg(self) -> None: ...
     def taskName(self, taskString: object) -> str: ...
     def uniqueName(self, idString: object) -> str: ...
-    def getCallbackContext(self, callback: Callable[..., object], extraArgs: Sequence[Any] = ...) -> int: ...
+    def getCallbackContext(self, callback: Callable[..., object], extraArgs: Sequence[Any] = []) -> int: ...
     def getCurrentContexts(self) -> list[int]: ...
     def getCallback(self, context: int) -> Callable[..., object]: ...
     def getCallbackArgs(self, context: int) -> Sequence[Any]: ...
     def doCallbackContext(self, context: int, args: Sequence[Any]) -> None: ...
     def setBarrierData(self, data: Iterable[tuple[Incomplete, Incomplete, Incomplete]]) -> None: ...
     def getBarrierData(self) -> tuple[tuple[int, str, list[Never]]]: ...
     def doneBarrier(self, name: str | None = None) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectAI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectAI.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     air: ClientRepository
     lastNonQuietZone: int | None
     def __init__(self, air: ClientRepository) -> None: ...
     def getDeleteEvent(self) -> str | None: ...
     def sendDeleteEvent(self) -> None: ...
     def getCacheable(self) -> Literal[False]: ...
     def deleteOrDelay(self) -> None: ...
-    def getDelayDeleteCount(self) -> Literal[0]: ...
+    def getDelayDeleteCount(self) -> int: ...
     def isDeleted(self) -> bool: ...
     def isGenerated(self) -> bool: ...
     def getDoId(self) -> int: ...
     def preAllocateDoId(self) -> None: ...
     def announceGenerate(self) -> Literal[False, None]: ...
     def b_setLocation(self, parentId: int, zoneId: int) -> None: ...
     def d_setLocation(self, parentId: int, zoneId: int) -> None: ...
@@ -44,29 +44,29 @@
     def handleLogicalZoneChange(self, newZoneId: int, oldZoneId: int) -> None: ...
     def getZoneData(self): ...
     def releaseZoneData(self) -> None: ...
     def getRender(self): ...
     def getNonCollidableParent(self): ...
     def getParentMgr(self): ...
     def getCollTrav(self, *args, **kArgs): ...
-    def sendUpdate(self, fieldName: str, args=...) -> None: ...
+    def sendUpdate(self, fieldName: str, args=[]) -> None: ...
     def GetPuppetConnectionChannel(self, doId: int) -> None: ...
     def GetAccountConnectionChannel(self, doId: int) -> None: ...
     def GetAccountIDFromChannelCode(self, channel: int) -> None: ...
     def GetAvatarIDFromChannelCode(self, channel: int) -> None: ...
     def sendUpdateToAvatarId(self, avId: int, fieldName: str, args) -> None: ...
     def sendUpdateToAccountId(self, accountId: int, fieldName: str, args) -> None: ...
     def sendUpdateToChannel(self, channelId: int, fieldName: str, args) -> None: ...
-    def generateWithRequired(self, zoneId: int, optionalFields=...) -> None: ...
-    def generateWithRequiredAndId(self, doId: int, parentId: int, zoneId: int, optionalFields=...) -> None: ...
-    def generateOtpObject(self, parentId: int, zoneId: int, optionalFields=..., doId: int | None = None) -> None: ...
+    def generateWithRequired(self, zoneId: int, optionalFields=[]) -> None: ...
+    def generateWithRequiredAndId(self, doId: int, parentId: int, zoneId: int, optionalFields=[]) -> None: ...
+    def generateOtpObject(self, parentId: int, zoneId: int, optionalFields=[], doId: int | None = None) -> None: ...
     def generate(self) -> None: ...
     def generateInit(self, repository=None) -> None: ...
     def generateTargetChannel(self, repository): ...
-    def sendGenerateWithRequired(self, repository, parentId: int, zoneId: int, optionalFields=...) -> None: ...
+    def sendGenerateWithRequired(self, repository, parentId: int, zoneId: int, optionalFields=[]) -> None: ...
     def initFromServerResponse(self, valDict) -> None: ...
     def requestDelete(self) -> None: ...
     def taskName(self, taskString: object) -> str: ...
     def uniqueName(self, idString: object) -> str: ...
     def validate(self, avId, bool: bool, msg) -> bool: ...
     def beginBarrier(self, name, avIds, timeout, callback): ...
     def getBarrierData(self) -> list[tuple[Incomplete, Incomplete, Incomplete]]: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectGlobalUD.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectGlobalUD.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectOV.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectOV.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 ESGenerating: Final = 5
 ESGenerated: Final = 6
 
 class DistributedObjectOV(DistributedObjectBase):
     DistributedObjectOV_initialized: Literal[1]
     DistributedObjectOV_deleted: Literal[1]
     activeState: Literal[1, 2, 3, 4, 5, 6]
-    def getDelayDeleteCount(self) -> Literal[0]: ...
+    def getDelayDeleteCount(self) -> int: ...
     def deleteOrDelay(self) -> None: ...
     def disableAnnounceAndDelete(self) -> None: ...
     def disableAndAnnounce(self) -> None: ...
     def announceGenerate(self) -> None: ...
     def disable(self) -> None: ...
     def isDisabled(self) -> bool: ...
     def isGenerated(self) -> bool: ...
     def generate(self) -> None: ...
     def generateInit(self) -> None: ...
     def getDoId(self) -> int: ...
     def postGenerateMessage(self) -> None: ...
     def updateRequiredFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
     def updateAllRequiredFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
     def updateRequiredOtherFields(self, dclass: DCClass, di: DatagramIterator) -> None: ...
-    def getCacheable(self) -> Literal[False]: ...
-    def sendUpdate(self, fieldName: str, args=..., sendToId: int | None = None) -> None: ...
+    def getCacheable(self) -> bool: ...
+    def sendUpdate(self, fieldName: str, args=[], sendToId: int | None = None) -> None: ...
     def uniqueName(self, idString: object) -> str: ...
     def taskName(self, taskString: object) -> str: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedObjectUD.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedObjectUD.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -37,32 +37,32 @@
     def getZoneChangeEvent(self): ...
     def getLogicalZoneChangeEvent(self): ...
     def handleLogicalZoneChange(self, newZoneId: int, oldZoneId: int) -> None: ...
     def getRender(self): ...
     def getNonCollidableParent(self): ...
     def getParentMgr(self): ...
     def getCollTrav(self, *args, **kArgs): ...
-    def sendUpdate(self, fieldName: str, args=...) -> None: ...
+    def sendUpdate(self, fieldName: str, args=[]) -> None: ...
     def GetPuppetConnectionChannel(self, doId: int) -> int: ...
     def GetAccountConnectionChannel(self, doId: int) -> int: ...
     def GetAccountIDFromChannelCode(self, channel: int) -> int: ...
     def GetAvatarIDFromChannelCode(self, channel: int) -> int: ...
     def sendUpdateToAvatarId(self, avId: int, fieldName: str, args) -> None: ...
     def sendUpdateToAccountId(self, accountId: int, fieldName: str, args) -> None: ...
     def sendUpdateToChannel(self, channelId: int, fieldName: str, args) -> None: ...
-    def generateWithRequired(self, zoneId: int, optionalFields=...): ...
-    def generateWithRequiredAndId(self, doId: int, parentId: int, zoneId: int, optionalFields=...) -> None: ...
-    def generateOtpObject(self, parentId: int, zoneId: int, optionalFields=..., doId: Any | None = None) -> None: ...
+    def generateWithRequired(self, zoneId: int, optionalFields=[]): ...
+    def generateWithRequiredAndId(self, doId: int, parentId: int, zoneId: int, optionalFields=[]) -> None: ...
+    def generateOtpObject(self, parentId: int, zoneId: int, optionalFields=[], doId: Any | None = None) -> None: ...
     def generate(self) -> None: ...
     def generateInit(self, repository: Unused = None) -> None: ...
     def generateTargetChannel(self, repository): ...
-    def sendGenerateWithRequired(self, repository, parentId: int, zoneId: int, optionalFields=...) -> None: ...
+    def sendGenerateWithRequired(self, repository, parentId: int, zoneId: int, optionalFields=[]) -> None: ...
     def initFromServerResponse(self, valDict: Mapping[str, Datagram | bytes]) -> None: ...
     def requestDelete(self) -> None: ...
     def taskName(self, taskString: object) -> str: ...
     def uniqueName(self, idString: object) -> str: ...
     def validate(self, avId, bool: bool, msg) -> bool: ...
     def beginBarrier(self, name, avIds, timeout, callback): ...
     def ignoreBarrier(self, context) -> None: ...
     def setBarrierReady(self, context) -> None: ...
-    def isGridParent(self) -> Literal[False]: ...
+    def isGridParent(self) -> bool: ...
     def execCommand(self, string: str | bytes | CodeType, mwMgrId: Unused, avId: Unused, zoneId: Unused) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNode.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNode.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNodeAI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNodeAI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DistributedSmoothNodeBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DistributedSmoothNodeBase.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import ClassVar
-from typing_extensions import Literal
 
 from direct._typing import Unused
 from direct.showbase.PythonUtil import Enum
 
 class DummyTaskClass:
     def setDelay(self, blah: Unused) -> None: ...
 
@@ -18,10 +17,10 @@
     def b_clearSmoothing(self) -> None: ...
     def d_clearSmoothing(self) -> None: ...
     def getPosHprBroadcastTaskName(self) -> str: ...
     def setPosHprBroadcastPeriod(self, period: float) -> None: ...
     def getPosHprBroadcastPeriod(self) -> float: ...
     def stopPosHprBroadcast(self) -> None: ...
     def posHprBroadcastStarted(self) -> bool: ...
-    def wantSmoothPosBroadcastTask(self) -> Literal[True]: ...
+    def wantSmoothPosBroadcastTask(self) -> bool: ...
     def startPosHprBroadcast(self, period: float = 0.2, stagger: bool = ..., type=None) -> None: ...
     def sendCurrentPosition(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DoCollectionManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DoCollectionManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DoHierarchy.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DoHierarchy.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/DoInterestManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/DoInterestManager.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable
 from typing import ClassVar, Protocol
-from typing_extensions import Final, Self
+from typing_extensions import Final
 
 from direct.directnotify.Notifier import Notifier
 from direct.distributed.DistributedObject import DistributedObject
 from direct.showbase.DirectObject import DirectObject
 from panda3d.core import ConfigVariableBool, DatagramIterator
 
 class _HasNum(Protocol):
@@ -40,15 +40,15 @@
     def sendEvents(self) -> None: ...
     def setDesc(self, desc: str) -> None: ...
     def isPendingDelete(self) -> bool: ...
 
 class InterestHandle:
     def __init__(self, id: int) -> None: ...
     def asInt(self) -> int: ...
-    def __eq__(self, other: Self | int) -> bool: ...  # type: ignore[override]
+    def __eq__(self, other: object) -> bool: ...
 
 class DoInterestManager(DirectObject):
     notify: ClassVar[Notifier]
     InterestDebug: ClassVar[ConfigVariableBool]
     def __init__(self) -> None: ...
     def setNoNewInterests(self, flag: bool) -> None: ...
     def noNewInterests(self) -> bool: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/GridChild.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/GridChild.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/GridParent.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/GridParent.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/InterestWatcher.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/InterestWatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/MsgTypes.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/MsgTypes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing_extensions import Final, Never
+from typing_extensions import Final
 
 MsgName2Id: Final[dict[str, int]]
 MsgId2Names: Final[dict[int, list[str]]]
 
 CLIENT_HELLO: Final = 1
 CLIENT_HELLO_RESP: Final = 2
 CLIENT_DISCONNECT: Final = 3
@@ -121,13 +121,13 @@
 CLIENTAGENT_CLOSE_CHANNEL: Final = 1101
 CLIENTAGENT_ADD_POST_REMOVE: Final = 1110
 CLIENTAGENT_CLEAR_POST_REMOVES: Final = 1111
 CLIENTAGENT_ADD_INTEREST: Final = 1200
 CLIENTAGENT_ADD_INTEREST_MULTIPLE: Final = 1201
 CLIENTAGENT_REMOVE_INTEREST: Final = 1203
 
-QUIET_ZONE_IGNORED_LIST: Final[list[Never]]
+QUIET_ZONE_IGNORED_LIST: Final[list[int]] = []
 
 CLIENT_LOGIN_2_GREEN: Final = 1
 CLIENT_LOGIN_2_PLAY_TOKEN: Final = 2
 CLIENT_LOGIN_2_BLUE: Final = 3
 CLIENT_LOGIN_3_DISL_TOKEN: Final = 4
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/MsgTypesCMU.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/MsgTypesCMU.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ParentMgr.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ParentMgr.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/PyDatagram.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/PyDatagram.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/RelatedObjectMgr.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/RelatedObjectMgr.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/ServerRepository.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/ServerRepository.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         tcpPort: int,
         serverAddress: str | None = None,
         udpPort: Unused = None,
         dcFileNames: Iterable[StrOrBytesPath] | None = None,
         threadedNet: bool | None = None,
     ) -> None: ...
     def flushTask(self, task: Unused) -> Literal[2]: ...
-    def setTcpHeaderSize(self, headerSize: Literal[0, 2, 4]) -> None: ...
-    def getTcpHeaderSize(self) -> Literal[0, 2, 4]: ...
+    def setTcpHeaderSize(self, headerSize: int) -> None: ...
+    def getTcpHeaderSize(self) -> int: ...
     def importModule(self, dcImports: dict[str, Any], moduleName: str, importSymbols: Sequence[str]) -> None: ...
     def readDCFile(self, dcFileNames: Iterable[StrOrBytesPath] | None = None) -> None: ...
     def listenerPoll(self, task: Unused) -> Literal[1]: ...
     def readerPollUntilEmpty(self, task: Unused) -> Literal[1]: ...
     def readerPollOnce(self) -> bool: ...
     def handleDatagram(self, datagram: NetDatagram) -> None: ...
     def handleMessageType(self, msgType: object, di: Unused) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/distributed/TimeManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/distributed/TimeManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/filter/CommonFilters.pyi` & `types-panda3d-0.3.3/src/direct-stubs/filter/CommonFilters.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     ssao: list[NodePath]
     def __init__(self, win: GraphicsOutput, cam: NodePath[Camera]) -> None: ...
     def cleanup(self) -> None: ...
     def reconfigure(self, fullrebuild: bool, changed: str) -> bool | None: ...
     def update(self, task: Task | None = None) -> Literal[1] | None: ...
     def set_msaa(self, samples) -> bool | None: ...
     def del_msaa(self) -> bool | None: ...
-    def set_cartoon_ink(self, separation: int = 1, color: tuple[float, float, float, float] = ...) -> bool | None: ...
+    def set_cartoon_ink(self, separation: int = 1, color: tuple[float, float, float, float] = (0, 0, 0, 1)) -> bool | None: ...
     def del_cartoon_ink(self) -> bool | None: ...
     def set_bloom(
         self,
-        blend: tuple[float, float, float, float] = ...,
+        blend: tuple[float, float, float, float] = (0.3, 0.4, 0.3, 0.0),
         mintrigger: float = 0.6,
         maxtrigger: float | None = 1.0,
         desat: float = 0.6,
         intensity: float = 1.0,
         size: str | int = 'medium',
     ) -> bool | None: ...
     def del_bloom(self) -> bool | None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/filter/FilterManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/filter/FilterManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/ClassicFSM.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/ClassicFSM.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,37 @@
     DISALLOW_VERBOSE: Final = 2
     ERROR: Final = 3
     onUndefTransition: Literal[0, 1, 2, 3]
     inspecting: bool
     def __init__(
         self,
         name: str,
-        states: Iterable[State] = ...,
+        states: Iterable[State] = [],
         initialStateName: str | None = None,
         finalStateName: str | None = None,
         onUndefTransition: Literal[0, 1, 2, 3] = 2,
     ) -> None: ...
-    def enterInitialState(self, argList: Iterable[Any] = ...) -> None: ...
+    def enterInitialState(self, argList: Iterable[Any] = []) -> None: ...
     def getName(self) -> str: ...
     def setName(self, name: str) -> None: ...
     def getStates(self) -> list[str]: ...
     def setStates(self, states: Iterable[State]) -> None: ...
     def addState(self, state: State) -> None: ...
-    def getInitialState(self) -> State: ...
-    def setInitialState(self, initialStateName: str) -> None: ...
-    def getFinalState(self) -> State: ...
-    def setFinalState(self, finalStateName: str) -> None: ...
+    def getInitialState(self) -> State | None: ...
+    def setInitialState(self, initialStateName: str | None) -> None: ...
+    def getFinalState(self) -> State | None: ...
+    def setFinalState(self, finalStateName: str | None) -> None: ...
     def requestFinalState(self) -> None: ...
-    def getCurrentState(self) -> State: ...
-    def getStateNamed(self, stateName: str) -> State: ...
+    def getCurrentState(self) -> State | None: ...
+    def getStateNamed(self, stateName: str | None) -> State | None: ...
     def hasStateNamed(self, stateName: str) -> bool: ...
     def request(
-        self, aStateName: str, enterArgList: Iterable[Any] = ..., exitArgList: Iterable[Any] = ..., force: bool = ...
+        self, aStateName: str | State, enterArgList: Iterable[Any] = [], exitArgList: Iterable[Any] = [], force: bool = ...
     ) -> bool: ...
-    def forceTransition(self, aStateName: str, enterArgList: Iterable[Any] = ..., exitArgList: Iterable[Any] = ...) -> None: ...
+    def forceTransition(
+        self, aStateName: str | State, enterArgList: Iterable[Any] = [], exitArgList: Iterable[Any] = []
+    ) -> None: ...
     def conditional_request(
-        self, aStateName: str, enterArgList: Iterable[Any] = ..., exitArgList: Iterable[Any] = ...
+        self, aStateName: str | State, enterArgList: Iterable[Any] = [], exitArgList: Iterable[Any] = []
     ) -> bool: ...
     def view(self) -> None: ...
     def isInternalStateInFlux(self) -> bool: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/FSM.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/FSM.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     oldState: str | None
     newState: str
     defaultTransitions: Mapping[str, Collection[str]] | None
     def __init__(self, name: str) -> None: ...
     def cleanup(self) -> None: ...
     def setBroadcastStateChanges(self, doBroadcast: bool) -> None: ...
     def getStateChangeEvent(self) -> str: ...
-    def getCurrentFilter(self) -> Callable[..., Any]: ...
+    def getCurrentFilter(self) -> Callable[..., tuple | None]: ...
     def getCurrentOrNextState(self) -> str: ...
     def getCurrentStateOrTransition(self) -> str: ...
     def isInTransition(self) -> bool: ...
     def forceTransition(self, request: str, *args: Any) -> None: ...
     def demand(self, request: str, *args: Any) -> None: ...
     def request(self, request: str, *args: Any) -> Any: ...
     def defaultEnter(self, *args: object) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/FourState.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/FourState.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     track: _Track | None
     stateTime: float
     names: Sequence[str]
     durations: Sequence[float | None]
     duration: float | None
     states: dict[_StateIndex, State]
     fsm: ClassicFSM
-    def __init__(self, names: Sequence[str], durations: Sequence[float | None] = ...) -> None: ...
+    def __init__(self, names: Sequence[str], durations: Sequence[float | None] = [0, 1, None, 1, 1]) -> None: ...
     def setTrack(self, track: _Track | None) -> None: ...
     def enterStateN(self, stateIndex: _StateIndex) -> None: ...
     def isOn(self) -> bool: ...
     def changedOnState(self, isOn: bool) -> None: ...
     def enterState0(self) -> None: ...
     def exitState0(self) -> None: ...
     def enterState1(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/FourStateAI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/FourStateAI.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     stateIndex: _StateIndex
     nextStateIndex: _StateIndex
     doLaterTask: AsyncTask | None
     names: SupportsGetItem[_StateIndex, str]
     durations: SupportsGetItem[_StateIndex, float | None]
     states: dict[_StateIndex, State]
     fsm: ClassicFSM
-    def __init__(self, names: Sequence[str], durations: SupportsGetItem[_StateIndex, float | None] = ...) -> None: ...
+    def __init__(
+        self, names: Sequence[str], durations: SupportsGetItem[_StateIndex, float | None] = [0, 1, None, 1, 1]
+    ) -> None: ...
     def delete(self) -> None: ...
     def getState(self) -> list[int]: ...
     def sendState(self) -> None: ...
     def setIsOn(self, isOn: bool) -> None: ...
     def isOn(self) -> bool: ...
     def changedOnState(self, isOn: bool) -> None: ...
     def switchToNextStateTask(self, task: Unused) -> Literal[0]: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/SampleFSM.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/SampleFSM.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/State.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/State.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Any: Final[_ANY]
     def __init__(
         self,
         name: str,
         enterFunc: _Callback = None,
         exitFunc: _Callback = None,
         transitions: list[str] | _ANY = 'ANY',
-        inspectorPos: typing.Any = ...,
+        inspectorPos: typing.Any = [],
     ) -> None: ...
     def getName(self) -> str: ...
     def setName(self, stateName: str) -> None: ...
     def getEnterFunc(self) -> _Callback: ...
     def setEnterFunc(self, stateEnterFunc: _Callback) -> None: ...
     def getExitFunc(self) -> _Callback: ...
     def setExitFunc(self, stateExitFunc: _Callback) -> None: ...
@@ -36,9 +36,9 @@
     def setTransitions(self, stateTransitions: list[str] | _ANY) -> None: ...
     def addTransition(self, transition: str) -> None: ...
     def getChildren(self) -> list[ClassicFSM]: ...
     def setChildren(self, FSMList: list[ClassicFSM]) -> None: ...
     def addChild(self, ClassicFSM: ClassicFSM) -> None: ...
     def removeChild(self, ClassicFSM: ClassicFSM) -> None: ...
     def hasChildren(self) -> bool: ...
-    def enter(self, argList: Iterable[typing.Any] = ...) -> None: ...
-    def exit(self, argList: Iterable[typing.Any] = ...) -> None: ...
+    def enter(self, argList: Iterable[typing.Any] = []) -> None: ...
+    def exit(self, argList: Iterable[typing.Any] = []) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/StateData.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/StateData.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     isLoaded: bool
     isEntered: bool
     def __init__(self, doneEvent: Any) -> None: ...
     def enter(self) -> bool: ...
     def exit(self) -> bool: ...
     def load(self) -> bool: ...
     def unload(self) -> bool: ...
-    def getDoneStatus(self) -> Any: ...
+    def getDoneStatus(self) -> Any | None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/fsm/StatePush.pyi` & `types-panda3d-0.3.3/src/direct-stubs/fsm/StatePush.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,8 +45,8 @@
 class EventPulse(Pulse, DirectObject):
     def __init__(self, event: str) -> None: ...
 
 class EventArgument(PushesStateChanges[Any], DirectObject):
     def __init__(self, event: str, index: int = 0) -> None: ...
 
 class AttrSetter(StateChangeNode[_T]):
-    def __init__(self, source: PushesStateChanges[_T], object: object, attrName: str) -> None: ...
+    def __init__(self, source: PushesStateChanges[_T], object: Any, attrName: str) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectDialog.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectDialog.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectEntry.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectEntry.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectEntryScroll.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectEntryScroll.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectFrame.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectFrame.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectGui.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectGui.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectGuiBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectGuiBase.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     postInitialiseFuncList: list[Callable[[], object]]
     fInit: bool
     def __init__(self) -> None: ...
     def defineoptions(
         self,
         keywords: Mapping[str, Any],
         optionDefs: Iterable[tuple[str, Any, Callable[[], object] | None]],
-        dynamicGroups: Iterable[str] = ...,
+        dynamicGroups: Iterable[str] = (),
     ) -> None: ...
     def addoptions(
         self, optionDefs: Iterable[tuple[str, Any, Callable[[], object] | None]], optionkeywords: Mapping[str, Any]
     ) -> None: ...
     def initialiseoptions(self, myClass: type[DirectGuiBase]) -> None: ...
     def postInitialiseFunc(self) -> None: ...
     def isinitoption(self, option: str) -> bool: ...
@@ -64,15 +64,15 @@
         **kw: object,
     ) -> None: ...
     def component(self, name: str) -> Any: ...
     def components(self) -> list[str]: ...
     def hascomponent(self, component: str) -> bool: ...
     def destroycomponent(self, name: str) -> None: ...
     def destroy(self) -> None: ...
-    def bind(self, event: str, command: Callable[..., Any], extraArgs: _Args = ...) -> None: ...
+    def bind(self, event: str, command: Callable[..., Any], extraArgs: _Args = []) -> None: ...
     def unbind(self, event: str) -> None: ...
 
 def toggleGuiGridSnap() -> None: ...
 def setGuiGridSpacing(spacing: float) -> None: ...
 
 class DirectGuiWidget(DirectGuiBase, NodePath[PGItem]):
     snapToGrid: ClassVar[bool]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectGuiGlobals.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectGuiGlobals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 defaultClickSound: Any | None
 defaultRolloverSound: Any | None
 defaultDialogGeom: Any | None
 defaultDialogRelief: _PGFrameStyle_Type | None
 drawOrder: int
 panel: Any | None
 
-INITOPT: Final[list[Literal['initopt']]]
+INITOPT: Final = ['initopt']
 
 LMB: Final = 0
 MMB: Final = 1
 RMB: Final = 2
 
 NORMAL: Final = 'normal'
 DISABLED: Final = 'disabled'
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectOptionMenu.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectOptionMenu.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectRadioButton.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectRadioButton.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrollBar.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrollBar.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrolledFrame.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrolledFrame.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectScrolledList.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectScrolledList.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectSlider.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectSlider.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/DirectWaitBar.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/DirectWaitBar.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenGeom.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenGeom.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenImage.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenImage.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/gui/OnscreenText.pyi` & `types-panda3d-0.3.3/src/direct-stubs/gui/OnscreenText.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,26 +30,26 @@
     scale: _OrderedPair
     wordwrap: float
     fg: LColor
     bg: LColor
     shadow: LColor
     frame: LColor
     align: _Alignment
-    unicodeText: Literal[True]
+    unicodeText: bool
     def __init__(
         self,
         text: str = '',
         style: int = 1,
-        pos: _OrderedPair = ...,
+        pos: _OrderedPair = (0, 0),
         roll: float = 0,
         scale: float | _OrderedPair | None = None,
         fg: Vec4Like | None = None,
         bg: Vec4Like | None = None,
         shadow: Vec4Like | None = None,
-        shadowOffset: _OrderedPair = ...,
+        shadowOffset: _OrderedPair = (0.04, 0.04),
         frame: Vec4Like | None = None,
         align: _Alignment | None = None,
         wordwrap: float | None = None,
         drawOrder: int | None = None,
         decal: bool = ...,
         font: TextFont | None = None,
         parent: NodePath | None = None,
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/ActorInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/ActorInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/AnimControlInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/AnimControlInterval.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 class AnimControlInterval(Interval):
     animNum: ClassVar[int]
     controls: AnimControlCollection
     loopAnim: bool
     constrainedLoop: bool
     playRate: float
     frameRate: float
-    startFrame: int
-    endFrame: int
+    startFrame: float
+    endFrame: float
     reverse: bool
     numFrames: int
     implicitDuration: bool
     currT: float
     def __init__(
         self,
         controls: AnimControl | AnimControlCollection,
         loop: bool = ...,
         constrainedLoop: bool = ...,
         duration: float | None = None,
-        startTime: int | None = None,
-        endTime: int | None = None,
-        startFrame: int | None = None,
-        endFrame: int | None = None,
+        startTime: float | None = None,
+        endTime: float | None = None,
+        startFrame: float | None = None,
+        endFrame: float | None = None,
         playRate: float = 1.0,
         name: str | None = None,
     ) -> None: ...
     def getCurrentFrame(self) -> float | None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/FunctionInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/FunctionInterval.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         extraArgs: Iterable[Any] = ...,
         **kw: Any,
     ) -> None: ...
     @staticmethod
     def makeUniqueName(func: object, suffix: str = '') -> str: ...
 
 class EventInterval(FunctionInterval):
-    def __init__(self, event: str, sentArgs: list[Any] = ...) -> None: ...
+    def __init__(self, event: str, sentArgs: list[Any] = []) -> None: ...
 
 class AcceptInterval(FunctionInterval):
     def __init__(self, dirObj: DirectObject, event: str, function: Callable[..., object], name: str | None = None) -> None: ...
 
 class IgnoreInterval(FunctionInterval):
     def __init__(self, dirObj: DirectObject, event: str, name: str | None = None) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/IndirectInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/IndirectInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/Interval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/Interval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/IntervalManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/IntervalManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/LerpBlendHelpers.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/LerpBlendHelpers.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/LerpInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/LerpInterval.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -464,15 +464,15 @@
     def __init__(
         self,
         function: Callable[..., object],
         duration: float = 0.0,
         fromData: float = 0,
         toData: float = 1,
         blendType: _BlendType = 'noBlend',
-        extraArgs: list[Any] = ...,
+        extraArgs: list[Any] = [],
         name: str | None = None,
     ) -> None: ...
 
 class LerpFuncNS(LerpFunctionNoStateInterval): ...
 
 class LerpFunctionInterval(Interval):
     lerpFunctionIntervalNum: ClassVar[int]
@@ -484,12 +484,12 @@
     def __init__(
         self,
         function: Callable[..., object],
         duration: float = 0.0,
         fromData: float = 0,
         toData: float = 1,
         blendType: _BlendType = 'noBlend',
-        extraArgs: list[Any] = ...,
+        extraArgs: list[Any] = [],
         name: str | None = None,
     ) -> None: ...
 
 class LerpFunc(LerpFunctionInterval): ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/MetaInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/MetaInterval.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self, list: Iterable[_Interval], name: str, relTime: float, relTo: _RelativeStart, duration: float
     ) -> None: ...
     def add_parallel_end_together(
         self, list: Iterable[_Interval], name: str, relTime: float, relTo: _RelativeStart, duration: float
     ) -> None: ...
     def add_track(
         self,
-        trackList: Iterable[tuple[_Interval, ...] | list[_Interval]],
+        trackList: Iterable[tuple[float, _Interval] | tuple[float, _Interval, _RelativeStart]],
         name: str,
         relTime: float,
         relTo: _RelativeStart,
         duration: float,
     ) -> None: ...
     def add_interval(self, ival: _Interval, relTime: float, relTo: _RelativeStart) -> None: ...
     def start(self, startT: float = 0.0, endT: float = -1.0, playRate: float = 1.0) -> None: ...
@@ -86,8 +86,8 @@
     privPostEvent = priv_post_event
 
 class Sequence(MetaInterval): ...
 class Parallel(MetaInterval): ...
 class ParallelEndTogether(MetaInterval): ...
 
 class Track(MetaInterval):
-    def validateComponent(self, tupleObj: object) -> TypeGuard[_Interval]: ...
+    def validateComponent(self, tupleObj: object) -> TypeGuard[tuple[_Interval, ...] | list[_Interval]]: ...  # type: ignore[override]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/MopathInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/MopathInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/ParticleInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/ParticleInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/ProjectileInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/ProjectileInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/SoundInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/SoundInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/interval/TestInterval.pyi` & `types-panda3d-0.3.3/src/direct-stubs/interval/TestInterval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ActionMgr.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ActionMgr.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimControlUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimControlUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/AnimMgrBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/AnimMgrBase.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 from direct.showutil.Rope import Rope
 from panda3d.core import LVecBase3f, NodePath
 
 from .LevelEditor import LevelEditor
 
 _T = TypeVar('_T', contravariant=True)
 
-# Mypy says `_T` should be covariant, but Pyright says contravariant.
-# Pyright appears to be correct.
-class _SupportsAppend(Protocol[_T]):  # type: ignore[misc]
-    def append(__item: _T) -> object: ...
+class _SupportsAppend(Protocol[_T]):
+    def append(self, __item: _T) -> object: ...
 
 class AnimMgrBase:
     editor: LevelEditor
     graphEditorCounter: int
     keyFramesInfo: dict
     curveAnimation: dict
     lerpFuncs: dict[str, Callable[..., None]]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/CurveAnimUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/CurveAnimUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/CurveEditor.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/CurveEditor.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 from direct.showutil.Rope import Rope
 from direct.task.Task import Task
 from panda3d._typing import Vec3Like, Vec4Like
 from panda3d.core import NodePath, NurbsCurveEvaluator
 
 from .LevelEditor import LevelEditor
 
-_Order: TypeAlias = Literal[1, 2, 3, 4]
 _Vert: TypeAlias = Vec3Like | Vec4Like
 
 class CurveEditor(DirectObject):
     editor: LevelEditor
     i: int
     ropeNum: int
     curve: list[_Vert]
     curveControl: list[tuple[int, NodePath]]
     currentRope: Rope | None
-    degree: _Order
+    degree: int
     selected: DirectNodePath
     currentCurve: NurbsCurveEvaluator
     def __init__(self, editor: LevelEditor) -> None: ...
     def createCurve(self) -> None: ...
     def editCurve(self, task: Task) -> Literal[1] | None: ...
     def onControlerDelete(self) -> None: ...
     def ropeUpdate(self, curve: Sequence[_Vert]) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/GraphEditorUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/GraphEditorUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/HotKeyUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/HotKeyUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/LayerEditorUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/LayerEditorUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/LevelEditorUIBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/LevelEditorUIBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/MayaConverter.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/MayaConverter.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectGlobals.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectGlobals.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectHandler.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectHandler.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectMgrBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectMgrBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPaletteBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPaletteBase.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     orderedProperties: list
     propertiesMask: dict
     def __init__(
         self,
         name: str = '',
         createFunction=None,
         model=None,
-        models: list = ...,
-        anims: list = ...,
-        animNames: list = ...,
-        animDict: dict = ...,
-        properties: dict[str, Any] = ...,
+        models: list = [],
+        anims: list = [],
+        animNames: list = [],
+        animDict: dict = {},
+        properties: dict[str, Any] = {},
         movable: bool = True,
         actor: bool = False,
         named: bool = False,
         updateModelFunction=None,
-        orderedProperties: list = ...,
-        propertiesMask: dict = ...,
+        orderedProperties: list = [],
+        propertiesMask: dict = {},
     ) -> None: ...
 
 class ObjectCurve(ObjectBase): ...
 
 class ObjectPaletteBase:
     rootName: str
     data: dict[str, Any]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPaletteUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPaletteUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ObjectPropertyUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ObjectPropertyUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/PaletteTreeCtrl.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/PaletteTreeCtrl.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoObjsUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoObjsUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/ProtoPaletteUI.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/ProtoPaletteUI.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/leveleditor/SceneGraphUIBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/leveleditor/SceneGraphUIBase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/motiontrail/MotionTrail.pyi` & `types-panda3d-0.3.3/src/direct-stubs/motiontrail/MotionTrail.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/AppRunner.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/AppRunner.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -131,8 +131,8 @@
     def setRequestFunc(self, func) -> None: ...
     def sendRequest(self, request, *args): ...
     def notifyRequest(self, message: str) -> None: ...
     def evalScript(self, expression, needsResponse: bool = False) -> None: ...
     def scriptRequest(self, operation, object, propertyName: str = '', value=None, needsResponse: bool = True): ...
     def dropObject(self, objectId) -> None: ...
 
-def dummyAppRunner(tokens=..., argv=None) -> AppRunner: ...
+def dummyAppRunner(tokens=[], argv=None) -> AppRunner: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/DeploymentTools.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/DeploymentTools.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ['Installer', 'Standalone']
 
 from _typeshed import StrOrBytesPath
 from collections.abc import Generator, Mapping
 from tarfile import TarInfo
 from typing import AnyStr, ClassVar
-from typing_extensions import Final, Literal
+from typing_extensions import Final
 
 from direct.directnotify.Notifier import Notifier
 from panda3d.core import Filename, HTTPClient, PNMImage
 
 from .HostInfo import HostInfo
 from .PackageInfo import PackageInfo
 
@@ -23,19 +23,19 @@
     notify: ClassVar[Notifier]
     p3dfile: Filename
     basename: str
     tokens: Mapping[str, str]
     tempDir: Filename
     host: HostInfo
     http: HTTPClient
-    def __init__(self, p3dfile: StrOrBytesPath, tokens: Mapping[str, str] = ...) -> None: ...
+    def __init__(self, p3dfile: StrOrBytesPath, tokens: Mapping[str, str] = {}) -> None: ...
     def __del__(self) -> None: ...
     def buildAll(self, outputDir: str = '.') -> None: ...
-    def build(self, output: Filename, platform: str | None = None, extraTokens: Mapping[str, str] = ...) -> None: ...
-    def embed(self, output: Filename, p3dembed: Filename, extraTokens: Mapping[str, str] = ...) -> None: ...
+    def build(self, output: Filename, platform: str | None = None, extraTokens: Mapping[str, str] = {}) -> None: ...
+    def embed(self, output: Filename, p3dembed: Filename, extraTokens: Mapping[str, str] = {}) -> None: ...
     def getExtraFiles(self, platform: str | None) -> list[Filename]: ...
 
 class PackageTree:
     platform: str
     hosts: dict[str, HostInfo]
     packages: dict[tuple[str, str | None], PackageInfo]
     hostUrl: str
@@ -47,16 +47,16 @@
 
 class Icon:
     notify: ClassVar[Notifier]
     images: dict[int, PNMImage]
     def __init__(self) -> None: ...
     def addImage(self, image: PNMImage | Filename | str) -> bool: ...
     def generateMissingImages(self) -> None: ...
-    def makeICO(self, fn: Filename | str) -> Literal[True]: ...
-    def makeICNS(self, fn: Filename | str) -> Literal[True]: ...
+    def makeICO(self, fn: Filename | str) -> bool: ...
+    def makeICNS(self, fn: Filename | str) -> bool: ...
 
 class Installer:
     notify: ClassVar[Notifier]
     p3dFilename: Filename
     shortname: str
     fullname: str
     version: str
@@ -70,15 +70,15 @@
     authoremail: str
     icon: Icon | None
     hostUrl: str | None
     requires: list[tuple[str, str, str]]
     extracts: list[str]
     tempDir: Filename
     standalone: Standalone
-    def __init__(self, p3dfile: Filename, shortname: str, fullname: str, version: object, tokens=...) -> None: ...
+    def __init__(self, p3dfile: Filename, shortname: str, fullname: str, version: object, tokens={}) -> None: ...
     def __del__(self) -> None: ...
     def installPackagesInto(self, hostDir: StrOrBytesPath, platform: str) -> None: ...
     def buildAll(self, outputDir: str = '.') -> None: ...
     def build(self, output: StrOrBytesPath, platform: str | None = None) -> None: ...
     def buildDEB(self, output: StrOrBytesPath, platform: str) -> Filename: ...
     def buildArch(self, output: StrOrBytesPath, platform: str) -> Filename: ...
     def buildAPP(self, output: StrOrBytesPath, platform: str) -> Filename: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/FileSpec.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/FileSpec.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/HostInfo.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/HostInfo.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/JavaScript.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/JavaScript.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/PackageInfo.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/PackageInfo.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/PackageInstaller.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/PackageInstaller.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     S_ready: Final = 1
     S_started: Final = 2
     S_done: Final = 3
     uniqueId: int
     appRunner: AppRunner
     taskChain: str
     callbackLock: Lock
-    calldedDownloadStarted: bool
+    calledDownloadStarted: bool
     calledDownloadFinished: bool
     packageLock: RLock
     packages: list[PackageInstaller.PendingPackage]
     state: Literal[0, 1, 2, 3]
     needsDescFile: list[PackageInstaller.PendingPackage]
     descFileTask: PythonTask | None
     needsDownload: list[PackageInstaller.PendingPackage]
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/PackageMerger.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/PackageMerger.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/Packager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/Packager.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         def installMultifile(self) -> bool: ...
         def installSolo(self) -> Literal[True, None]: ...
         def cleanup(self) -> None: ...
         def addFile(
             self,
             filename: Filename,
             newName: str | None = None,
-            delteTemp: bool = False,
+            deleteTemp: bool = False,
             explicit: bool = False,
             compress: bool | None = None,
             extract: bool | None = None,
             text: str | None = None,
             unprocessed: bool | None = None,
             executable: bool | None = None,
             dependencyDir: str | None = None,
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/PatchMaker.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/PatchMaker.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,18 +26,18 @@
         toPatches: list[PatchMaker.Patchfile]
         tempFile: Filename | None
         def __init__(
             self, packageName: str | None, platform: str | None, version: str | None, hostUrl: str | None, file: FileSpec | None
         ) -> None: ...
         def cleanup(self) -> None: ...
         def getPatchChain(
-            self, startPv: Self, alreadyVisited: MutableSequence[Self] = ...
+            self, startPv: Self, alreadyVisited: MutableSequence[Self] = []
         ) -> list[PatchMaker.Patchfile] | None: ...
         def getRecreateFilePlan(
-            self, alreadyVisited: MutableSequence[Self] = ...
+            self, alreadyVisited: MutableSequence[Self] = []
         ) -> tuple[Filename, PatchMaker.PackageVersion, _Plan] | tuple[None, None, None]: ...
         def getFile(self) -> Filename | None: ...
         def applyPatch(self, origFile: StrOrBytesPath, patchFilename: StrOrBytesPath) -> Filename | None: ...
         def getNext(self, package: PatchMaker.Package) -> PatchMaker.Patchfile: ...
 
     class Patchfile:
         package: PatchMaker.Package
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/ScanDirectoryNode.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/ScanDirectoryNode.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 vfs: Final[VirtualFileSystem]
 
 class ScanDirectoryNode:
     pathname: Filename
     filenames: list[Filename]
     fileSize: int
     nested: list[ScanDirectoryNode]
-    nextedSize: int
+    nestedSize: int
     def __init__(self, pathname: Filename, ignoreUsageXml: bool = False) -> None: ...
     def getTotalSize(self) -> int: ...
     def extractSubdir(self, pathname: Filename) -> ScanDirectoryNode: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/p3d/SeqValue.pyi` & `types-panda3d-0.3.3/src/direct-stubs/p3d/SeqValue.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/particles/ForceGroup.pyi` & `types-panda3d-0.3.3/src/direct-stubs/particles/ForceGroup.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/particles/ParticleEffect.pyi` & `types-panda3d-0.3.3/src/direct-stubs/particles/ParticleEffect.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/particles/Particles.pyi` & `types-panda3d-0.3.3/src/direct-stubs/particles/Particles.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/particles/SpriteParticleRendererExt.pyi` & `types-panda3d-0.3.3/src/direct-stubs/particles/SpriteParticleRendererExt.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Audio3DManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Audio3DManager.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 __all__ = ['Audio3DManager']
 
 from _typeshed import StrOrBytesPath
 from typing_extensions import Literal
 
 from direct._typing import Unused
-from panda3d.core import AudioManager, AudioSound, LVecBase3f, NodePath
+from panda3d.core import AudioManager, AudioSound, LVecBase3f, NodePath, WeakNodePath
 
 class Audio3DManager:
     audio_manager: AudioManager
     listener_target: NodePath | None
     root: NodePath
-    sound_dict: dict[NodePath, list[AudioSound]]
+    sound_dict: dict[WeakNodePath, list[AudioSound]]
     vel_dict: dict[AudioSound, LVecBase3f | None]
     listener_vel: LVecBase3f | None
     def __init__(
         self,
         audio_manager: AudioManager,
         listener_target: NodePath | None = None,
         root: NodePath | None = None,
@@ -27,25 +27,25 @@
     def get_doppler_factor(self) -> float: ...
     def set_drop_off_factor(self, factor: float) -> None: ...
     def get_drop_off_factor(self) -> float: ...
     def set_sound_min_distance(self, sound: AudioSound, dist: float) -> None: ...
     def get_sound_min_distance(self, sound: AudioSound) -> float: ...
     def set_sound_max_distance(self, sound: AudioSound, dist: float) -> None: ...
     def get_sound_max_distance(self, sound: AudioSound) -> float: ...
-    # `velocity` is purposely not `Vec3OrTuple`
+    # `velocity` is purposely not `Vec3Like`
     def set_sound_velocity(self, sound: AudioSound, velocity: LVecBase3f | tuple[float, float, float]) -> None: ...
     def set_sound_velocity_auto(self, sound: AudioSound) -> None: ...
     def get_sound_velocity(self, sound: AudioSound) -> LVecBase3f: ...
-    # `velocity` is purposely not `Vec3OrTuple`
+    # `velocity` is purposely not `Vec3Like`
     def set_listener_velocity(self, velocity: LVecBase3f | tuple[float, float, float]) -> None: ...
     def set_listener_velocity_auto(self) -> None: ...
     def get_listener_velocity(self) -> LVecBase3f: ...
-    def attach_sound_to_object(self, sound: AudioSound, object: NodePath) -> Literal[1]: ...
+    def attach_sound_to_object(self, sound: AudioSound, object: WeakNodePath) -> Literal[1]: ...
     def detach_sound(self, sound: AudioSound) -> bool: ...
-    def get_sounds_on_object(self, object: NodePath) -> list[AudioSound]: ...
+    def get_sounds_on_object(self, object: WeakNodePath) -> list[AudioSound]: ...
     def attach_listener(self, object: NodePath) -> Literal[1]: ...
     def detach_listener(self) -> Literal[1]: ...
     def update(self, task: Unused = None) -> Literal[1]: ...
     def disable(self) -> None: ...
     loadSfx = load_sfx
     setDistanceFactor = set_distance_factor
     getDistanceFactor = get_distance_factor
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/BufferViewer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/BufferViewer.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections.abc import MutableMapping
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias, TypeGuard
 
 from direct._typing import Unused
 from direct.directnotify.Notifier import Notifier
-from panda3d.core import CardMaker, GeomNode, GraphicsEngine, GraphicsOutput, NodePath, PythonTask, Texture
+from panda3d.core import CardMaker, GeomNode, GraphicsEngine, GraphicsOutput, NodePath, PythonTask, Texture, WindowProperties
 
 _Layout: TypeAlias = Literal['vline', 'hline', 'vgrid', 'hgrid', 'cycle']
 _Position: TypeAlias = Literal['llcorner', 'lrcorner', 'ulcorner', 'urcorner']
 _Texture: TypeAlias = Texture | GraphicsOutput | Literal['all']
 
 class BufferViewer:
     notify: ClassVar[Notifier]
@@ -19,23 +19,23 @@
     sizey: float
     position: _Position
     layout: _Layout
     include: _Texture | list[_Texture]
     exclude: _Texture | list[_Texture]
     cullbin: str
     cullsort: int
-    win: GraphicsOutput
+    win: GraphicsOutput | WindowProperties
     engine: GraphicsEngine
     renderParent: NodePath
     cards: list[NodePath]
     cardindex: int
     cardmaker: CardMaker
     task: PythonTask | Literal[0]
     dirty: bool
-    def __init__(self, win: GraphicsOutput, parent: NodePath) -> None: ...
+    def __init__(self, win: GraphicsOutput | WindowProperties, parent: NodePath) -> None: ...
     def refreshReadout(self) -> None: ...
     def isValidTextureSet(self, x: object) -> TypeGuard[_Texture | list[_Texture]]: ...
     def isEnabled(self) -> bool: ...
     def enable(self, x: bool) -> None: ...
     def toggleEnable(self) -> None: ...
     def setCardSize(self, x: float, y: float) -> None: ...
     def setPosition(self, pos: _Position) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/BulletinBoard.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/BulletinBoard.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/BulletinBoardWatcher.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/BulletinBoardWatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ContainerLeakDetector.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ContainerLeakDetector.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from collections.abc import Generator, Hashable, Mapping
+from collections.abc import Callable, Generator, Hashable, Mapping
 from typing import Any, ClassVar, TypeVar, overload
 
-from direct._typing import SimpleCallback
 from direct.directnotify.Notifier import Notifier
 
 from .Job import Job
 
 _T = TypeVar('_T')
 
 intTypes: tuple[type[int]]
@@ -60,22 +59,22 @@
     notify: Notifier
     def __init__(self, name: str, leakDetector: ContainerLeakDetector, index: int) -> None: ...
     def run(self) -> Generator[Any | None, None, None]: ...
 
 class FPTObjsOfType(Job):
     notify: Notifier
     def __init__(
-        self, name: str, leakDetector: ContainerLeakDetector, otn: str, doneCallback: SimpleCallback | None = None
+        self, name: str, leakDetector: ContainerLeakDetector, otn: str, doneCallback: Callable[[], object] | None = None
     ) -> None: ...
     def run(self) -> Generator[Any | None, None, None]: ...
 
 class FPTObjsNamed(Job):
     notify: Notifier
     def __init__(
-        self, name: str, leakDetector: ContainerLeakDetector, on: str, doneCallback: SimpleCallback | None = None
+        self, name: str, leakDetector: ContainerLeakDetector, on: str, doneCallback: Callable[[], object] | None = None
     ) -> None: ...
     def run(self) -> Generator[Any | None, None, None]: ...
 
 class PruneObjectRefs(Job):
     notify: Notifier
     def __init__(self, name: str, leakDetector: ContainerLeakDetector) -> None: ...
     def run(self) -> Generator[Any | None, None, None]: ...
@@ -92,9 +91,9 @@
     def getContainerIds(self) -> list[int]: ...
     def getContainerByIdGen(self, id: int, *, getInstance: bool = ...) -> Generator[Any | None, None, None]: ...
     def getContainerById(self, id: int) -> Any | None: ...
     def getContainerNameByIdGen(self, id: int, *, getInstance: bool = ...) -> Generator[str | None, None, None]: ...
     def getContainerNameById(self, id: int) -> str: ...
     def removeContainerById(self, id: int) -> None: ...
     def run(self) -> Generator[Any, None, None]: ...
-    def getPathsToContainers(self, name: str, ot: str, doneCallback: SimpleCallback | None = None) -> FPTObjsOfType: ...
-    def getPathsToContainersNamed(self, name: str, on: str, doneCallback: SimpleCallback | None = None) -> FPTObjsNamed: ...
+    def getPathsToContainers(self, name: str, ot: str, doneCallback: Callable[[], object] | None = None) -> FPTObjsOfType: ...
+    def getPathsToContainersNamed(self, name: str, on: str, doneCallback: Callable[[], object] | None = None) -> FPTObjsNamed: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/CountedResource.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/CountedResource.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/DirectObject.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/DirectObject.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 __all__ = ['DirectObject']
 
 from collections.abc import Callable, Sequence
 from typing import Any, overload
 from typing_extensions import TypeAlias
 
-from panda3d._typing import TaskCoroutine
+from panda3d._typing import TaskCoroutine, TaskFunction
 from panda3d.core import AsyncTask, PythonTask
 
 # Ideally, this should just be Sequence[Any], but the code here and in Messenger
 # means that it has to be one of these.
 _Args: TypeAlias = tuple[Any, ...] | list[Any]
 
 class DirectObject:
     def __init__(self) -> None: ...
-    def accept(self, event: str, method: Callable[..., Any], extraArgs: _Args = ...) -> None: ...
-    def accept_once(self, event: str, method: Callable[..., Any], extraArgs: _Args = ...) -> None: ...
+    def accept(self, event: str, method: Callable[..., Any], extraArgs: _Args = []) -> None: ...
+    def accept_once(self, event: str, method: Callable[..., Any], extraArgs: _Args = []) -> None: ...
     def ignore(self, event: str) -> None: ...
     def ignore_all(self) -> None: ...
     def is_accepting(self, event: str) -> bool: ...
     def get_all_accepting(self) -> list[tuple[str, int]]: ...
     def is_ignoring(self, event: str) -> bool: ...
     @overload
     def add_task(
         self,
-        funcOrTask: PythonTask | Callable[..., int | TaskCoroutine[int | None] | None] | TaskCoroutine[Any],
+        funcOrTask: PythonTask | TaskFunction | TaskCoroutine[Any],
         name: str | None = None,
         sort: int | None = None,
         extraArgs: Sequence[Any] | None = None,
         priority: int | None = None,
         appendTask: bool = False,
         uponDeath: Callable[..., object] | None = None,
         taskChain: str | None = None,
@@ -48,15 +48,15 @@
         *,
         delay: float | None = None,
     ) -> AsyncTask: ...
     @overload
     def do_method_later(
         self,
         delayTime: float,
-        funcOrTask: PythonTask | Callable[..., int | TaskCoroutine[int | None] | None] | TaskCoroutine[Any],
+        funcOrTask: PythonTask | TaskFunction | TaskCoroutine[Any],
         name: str | None,
         extraArgs: Sequence[Any] | None = None,
         sort: int | None = None,
         priority: int | None = None,
         taskChain: str | None = None,
         uponDeath: Callable[..., object] | None = None,
         appendTask: bool = False,
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/DistancePhasedNode.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/DistancePhasedNode.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     exitPrefix: str
     phaseCollideMask: CollideMask
     cTrav: CollisionTraverser
     fromCollideNode: CollisionNode | None
     def __init__(
         self,
         name: str,
-        phaseParamMap: Mapping[str, float] = ...,
+        phaseParamMap: Mapping[str, float] = {},
         autoCleanup: bool = True,
         enterPrefix: str = 'enter',
         exitPrefix: str = 'exit',
         phaseCollideMask: CollideMask = ...,
         fromCollideNode: CollisionNode | None = None,
     ) -> None: ...
     def __del__(self) -> None: ...
@@ -30,14 +30,14 @@
 
 class BufferedDistancePhasedNode(DistancePhasedNode):
     bufferParamMap: Mapping[str, tuple[float, int]]
     bufferParamList: list[tuple[str, tuple[float, int]]]
     def __init__(
         self,
         name: str,
-        bufferParamMap: Mapping[str, tuple[float, int]] = ...,
+        bufferParamMap: Mapping[str, tuple[float, int]] = {},
         autoCleanup: bool = True,
         enterPrefix: str = 'enter',
         exitPrefix: str = 'exit',
         phaseCollideMask: CollideMask = ...,
         fromCollideNode: CollisionNode | None = None,
     ) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/EventManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/EventManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Finder.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Finder.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/GarbageReport.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/GarbageReport.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Job.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Job.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/JobManager.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/JobManager.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/LeakDetectors.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/LeakDetectors.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Loader.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Loader.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ['Loader']
 
 from _typeshed import StrOrBytesPath
-from collections.abc import Callable, Iterable, Sequence
+from collections.abc import Callable, Collection, Iterable, Sequence
 from typing import Any, ClassVar, overload
 from typing_extensions import Literal, Self, TypeAlias
 
 from direct.directnotify.Notifier import Notifier
 from panda3d import core
 from panda3d._typing import Vec4Like
 from panda3d.core import (
@@ -36,22 +36,22 @@
     def __init__(self, requestList: Sequence[AsyncTask]) -> None: ...
     def __await__(self) -> Self: ...
     def __anext__(self) -> Self: ...
     def __iter__(self) -> Self: ...
     def __next__(self) -> AsyncTask: ...
 
 class _Callback:
-    objects: list[Any]
+    objects: list[Any | None]
     gotList: bool
-    callback: Callable[..., object]
+    callback: Callable[..., object] | None
     extraArgs: Iterable[Any]
     requests: set[AsyncTask] | None
     requestList: list[AsyncTask] | None
     def __init__(
-        self, loader: Loader, numObjects: int, gotList: bool, callback: Callable[..., object], extraArgs: Iterable[Any]
+        self, loader: Loader, numObjects: int, gotList: bool, callback: Callable[..., object] | None, extraArgs: Iterable[Any]
     ) -> None: ...
     def gotObject(self, index: int, object: Any) -> None: ...
     def cancel(self) -> None: ...
     def cancelled(self) -> bool: ...
     def done(self) -> bool: ...
     def result(self) -> list[Any] | Any: ...
     def exception(self) -> None: ...
@@ -71,110 +71,110 @@
         self,
         modelPath: str,
         loaderOptions: LoaderOptions | None = None,
         noCache: bool | None = None,
         allowInstance: bool = False,
         okMissing: Literal[True] | None = None,
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
         priority: float | None = None,
         blocking: Literal[True] | None = None,
     ) -> NodePath | None: ...
     @overload
     def load_model(
         self,
         modelPath: str,
         loaderOptions: LoaderOptions | None = None,
         noCache: bool | None = None,
         allowInstance: bool = False,
         *,
         okMissing: Literal[False],
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> NodePath: ...
     @overload
     def load_model(
         self,
         modelPath: str,
         loaderOptions: LoaderOptions | None,
         noCache: bool | None,
         allowInstance: bool,
         okMissing: Literal[False],
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> NodePath: ...
     @overload
     def load_model(
         self,
         modelPath: list[str] | set[str] | tuple[str, ...],
         loaderOptions: LoaderOptions | None = None,
         noCache: bool | None = None,
         allowInstance: bool = False,
         okMissing: Literal[True] | None = None,
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> list[NodePath | None]: ...
     @overload
     def load_model(
         self,
         modelPath: list[str] | set[str] | tuple[str, ...],
         loaderOptions: LoaderOptions | None = None,
         noCache: bool | None = None,
         allowInstance: bool = False,
         *,
         okMissing: Literal[False],
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> list[NodePath]: ...
     @overload
     def load_model(
         self,
         modelPath: list[str] | set[str] | tuple[str, ...],
         loaderOptions: LoaderOptions | None,
         noCache: bool | None,
         allowInstance: bool,
         okMissing: Literal[False],
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> list[NodePath]: ...
     @overload
     def load_model(
         self,
         modelPath: str | list[str] | set[str] | tuple[str, ...],
         loaderOptions: LoaderOptions | None = None,
         noCache: bool | None = None,
         allowInstance: bool = False,
         okMissing: bool | None = None,
         *,
         callback: Callable[..., object],
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[False] | None = None,
     ) -> _Callback: ...
     @overload
     def load_model(
         self,
         modelPath: str | list[str] | set[str] | tuple[str, ...],
         loaderOptions: LoaderOptions | None,
         noCache: bool | None,
         allowInstance: bool,
         okMissing: bool | None,
         callback: Callable[..., object],
-        extraArgs: Iterable[Any] = ...,
-        priority: float | None = None,
+        extraArgs: Iterable[Any] = [],
+        priority: int | None = None,
         blocking: Literal[False] | None = None,
     ) -> _Callback: ...
     def cancelRequest(self, cb: _Callback) -> None: ...
     def isRequestPending(self, cb: _Callback) -> bool: ...
     def loadModelOnce(self, modelPath: str) -> NodePath | None: ...
     def loadModelCopy(self, modelPath: str, loaderOptions: LoaderOptions | None = None) -> NodePath | None: ...
     def loadModelNode(self, modelPath: str) -> PandaNode | None: ...
@@ -182,49 +182,49 @@
     @overload
     def save_model(
         self,
         modelPath: str,
         node: NodePath | PandaNode,
         loaderOptions: LoaderOptions | None = None,
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
         priority: int | None = None,
         blocking: Literal[True] | None = None,
     ) -> bool: ...
     @overload
     def save_model(
         self,
         modelPath: list[str] | set[str] | tuple[str, ...],
         node: NodePath | PandaNode,
         loaderOptions: LoaderOptions | None = None,
         callback: None = None,
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
         priority: int | None = None,
         blocking: bool | None = None,
     ) -> list[bool]: ...
     @overload
     def save_model(
         self,
         modelPath: str | list[str] | set[str] | tuple[str, ...],
         node: NodePath | PandaNode,
         loaderOptions: LoaderOptions | None = None,
         *,
         callback: Callable[..., object],
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
         priority: int | None = None,
         blocking: Literal[False] | None = None,
     ) -> _Callback: ...
     @overload
     def save_model(
         self,
         modelPath: str | list[str] | set[str] | tuple[str, ...],
         node: NodePath | PandaNode,
         loaderOptions: LoaderOptions | None,
         callback: Callable[..., object],
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
         priority: int | None = None,
         blocking: Literal[False] | None = None,
     ) -> _Callback: ...
     def load_font(
         self,
         modelPath: str,
         spaceAdvance: float | None = None,
@@ -308,25 +308,25 @@
     ) -> _Callback | None: ...
     def load_sound(
         self,
         manager: AudioManager,
         soundPath: StrOrBytesPath | list[StrOrBytesPath] | set[StrOrBytesPath] | tuple[StrOrBytesPath, ...],
         positional: bool = False,
         callback: Callable[..., object] | None = None,
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
     ) -> _Callback: ...
     def unload_sfx(self, sfx: AudioSound) -> None: ...
     def load_shader(self, shaderPath: StrOrBytesPath, okMissing: bool = False) -> Shader: ...
     def unload_shader(self, shaderPath: StrOrBytesPath | None) -> None: ...
     def async_flatten_strong(
         self,
-        model: NodePath | Iterable[NodePath],
+        model: NodePath | Collection[NodePath],
         inPlace: bool = True,
         callback: Callable[..., object] | None = None,
-        extraArgs: Iterable[Any] = ...,
+        extraArgs: Iterable[Any] = [],
     ) -> _Callback: ...
     loadModel = load_model
     unloadModel = unload_model
     saveModel = save_model
     loadFont = load_font
     loadTexture = load_texture
     load3DTexture = load_3d_texture
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Messenger.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Messenger.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 class Messenger:
     notify: ClassVar[Notifier]
     lock: Lock
     quieting: dict[str, bool]
     def __init__(self) -> None: ...
     def future(self, event: str) -> AsyncFuture: ...
     def accept(
-        self, event: str, object: DirectObject, method: Callable[..., object], extraArgs: _Args = ..., persistent: bool = ...
+        self, event: str, object: DirectObject, method: Callable[..., object], extraArgs: _Args = [], persistent: bool = ...
     ) -> None: ...
     def ignore(self, event: str, object: DirectObject) -> None: ...
     def ignore_all(self, object: DirectObject) -> None: ...
     def get_all_accepting(self, object: DirectObject) -> list[str]: ...
     def is_accepting(self, event: str, object: DirectObject) -> bool: ...
     def who_accepts(self, event: str) -> _EventDict | None: ...
     def is_ignoring(self, event: str, object: DirectObject) -> bool: ...
-    def send(self, event: str, sentArgs: _Args = ..., taskChain: str | None = None) -> None: ...
+    def send(self, event: str, sentArgs: _Args = [], taskChain: str | None = None) -> None: ...
     def clear(self) -> None: ...
     def is_empty(self) -> bool: ...
     def get_events(self) -> list[str]: ...
     def replace_method(self, oldMethod: Callable[..., object], newFunction: Callable[..., object]) -> int: ...
     def toggle_verbose(self) -> None: ...
     def find(self, needle: str) -> dict[str, _EventDict]: ...
     def find_all(self, needle: str, limit: int | None = None) -> dict[str, _EventDict]: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ObjectPool.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ObjectPool.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ObjectReport.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ObjectReport.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/OnScreenDebug.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/OnScreenDebug.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/PhasedObject.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/PhasedObject.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 from direct.directnotify.Notifier import Notifier
 
 class PhasedObject:
     notify: ClassVar[Notifier]
     phase: int
     phaseAliasMap: dict[int, str]
     aliasPhaseMap: dict[str, int]
-    def __init__(self, aliasMap: Mapping[int, str] = ...) -> None: ...
+    def __init__(self, aliasMap: Mapping[int, str] = {}) -> None: ...
     def setAlias(self, phase: int, alias: str) -> None: ...
     def getPhaseAlias(self, phase: int) -> str: ...
     def getAliasPhase(self, alias: str) -> int: ...
     def getPhase(self) -> str: ...
     def setPhase(self, aPhase: int | str) -> None: ...
     def cleanup(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Pool.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Pool.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ProfileSession.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ProfileSession.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/PythonUtil.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/PythonUtil.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from _typeshed import SupportsWrite
 from collections.abc import Callable, Collection, Container, Generator, Iterable, Mapping, MutableSequence, Sequence
 from typing import Any, ClassVar, Generic, TextIO, TypeVar, overload
 from typing_extensions import Never, Self, TypeAlias
 
-from direct._typing import AnyReal, SimpleCallback
+from direct._typing import AnyReal
 from direct.directnotify.Notifier import Notifier
 from direct.tkwidgets.Valuator import ValuatorGroupPanel
 from panda3d.core import PStatCollector
 
 _T = TypeVar('_T')
 _S = TypeVar('_S')
 _KT = TypeVar('_KT')
 _VT = TypeVar('_VT')
-_CallbackT = TypeVar('_CallbackT', bound=SimpleCallback)
+_CallbackT = TypeVar('_CallbackT', bound=Callable[[], object])
 
 _RNG: TypeAlias = Callable[[], float]
 
 class Functor(Generic[_T]):
     def __init__(self, function: Callable[..., _T], *args: Any, **kargs: Any) -> None: ...
     def destroy(self) -> None: ...
     def __call__(self, *args: Any, **kargs: Any) -> _T: ...
@@ -194,31 +194,31 @@
 def getNumberedTypedString(items: Sequence[object], maxLen: int = 5000, numPrefix: str = '') -> str: ...
 def getNumberedTypedSortedString(items: Sequence[object], maxLen: int = 5000, numPrefix: str = '') -> str: ...
 def printNumberedTyped(items: Sequence[object], maxLen: int = 5000) -> None: ...
 def printNumberedTypesGen(items: Sequence[object], maxLen: int = 5000) -> Generator[None, None, None]: ...
 def printNumberedTypes(items: Sequence[object], maxLen: int = 5000) -> Generator[None, None, None]: ...
 
 class DelayedCall:
-    def __init__(self, func: SimpleCallback, name: str | None = None, delay: float | None = None) -> None: ...
+    def __init__(self, func: Callable[[], object], name: str | None = None, delay: float | None = None) -> None: ...
     def destroy(self) -> None: ...
     def finish(self) -> None: ...
 
 class FrameDelayedCall:
     def __init__(
-        self, name: str, callback: SimpleCallback, frames: int | None = None, cancelFunc: SimpleCallback | None = None
+        self, name: str, callback: Callable[[], object], frames: int | None = None, cancelFunc: Callable[[], object] | None = None
     ) -> None: ...
     def destroy(self) -> None: ...
     def finish(self) -> None: ...
 
 class DelayedFunctor:
     def __init__(self, functor: Callable[..., object], name: str | None = None, delay: float | None = None) -> None: ...
     def __call__(self, *args: Any, **kwArgs: Any) -> None: ...
 
 class SubframeCall:
-    def __init__(self, functor: SimpleCallback, taskPriority: int | None, name: str | None = None) -> None: ...
+    def __init__(self, functor: Callable[[], object], taskPriority: int | None, name: str | None = None) -> None: ...
     def cleanup(self) -> None: ...
 
 class PStatScope:
     collectors: ClassVar[dict[str, PStatCollector]]
     levels: list[str]
     def __init__(self, level: str | None = None) -> None: ...
     def copy(self, push: bool | None = None) -> PStatScope: ...
@@ -226,19 +226,19 @@
     def pop(self) -> str: ...
     def start(self, push: bool | None = None) -> None: ...
     def stop(self, pop: bool = False) -> None: ...
     def getCollector(self) -> PStatCollector: ...
 
 def pstatcollect(scope: PStatScope, level: str | None = None) -> Callable[[_T], _T]: ...
 def report(
-    types: Container[str] = ...,
+    types: Container[str] = [],
     prefix: str = '',
     xform: Callable[[Any], object] | None = None,
     notifyFunc: Callable[[str], object] | None = None,
-    dConfigParam: str | list[str] | tuple[str, ...] = ...,
+    dConfigParam: str | list[str] | tuple[str, ...] = [],
 ) -> Callable[[_T], _T]: ...
 def getBase(): ...
 def getRepository(): ...
 
 exceptionLoggedNotify: Notifier | None
 
 GoldenRatio: float
@@ -321,9 +321,9 @@
 def histogramDict(l: Iterable[_T]) -> dict[_T, int]: ...
 def unescapeHtmlString(s: str) -> str: ...
 
 class PriorityCallbacks:
     def __init__(self) -> None: ...
     def clear(self) -> None: ...
     def add(self, callback: _CallbackT, priority: int | None = None) -> tuple[int, _CallbackT]: ...
-    def remove(self, item: tuple[int, SimpleCallback]) -> None: ...
+    def remove(self, item: tuple[int, Callable[[], object]]) -> None: ...
     def __call__(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/RandomNumGen.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/RandomNumGen.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ReferrerSearch.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Slider.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
-from collections.abc import Generator, Reversible, Sized
-from typing import Any
+__all__ = ['Slider', 'SliderWidget', 'rgbPanel']
 
-from .Job import Job
+import Pmw  # type: ignore[import]
+from direct._typing import Unused
 
-class ReferrerSearch(Job):
-    obj: object
-    maxRefs: int
-    visited: set[int]
-    depth: int
-    found: int
-    shouldPrintStats: bool
-    def __init__(self, obj: object, maxRefs: int = 100) -> None: ...
-    def __call__(self) -> None: ...
-    def run(self) -> Generator[Any | None, None, None]: ...
-    def __del__(self) -> None: ...
-    def truncateAtNewLine(self, s: str) -> str: ...
-    def printStatsWhenAble(self) -> None: ...
-    def myrepr(self, referrer: object, refersTo: object) -> str: ...
-    def step(self, depth: int, path: Reversible[object]) -> None: ...
-    def stepGenerator(self, depth: int, path: Reversible[object]) -> None: ...
-    def printStats(self, path: Reversible[object]) -> None: ...
-    def isAtRoot(self, at: object, path: Reversible[object]) -> bool: ...
-    def isManyRef(self, at: object, path: Reversible[object], referrers: Sized) -> bool | None: ...
+from .Valuator import Valuator, rgbPanel as rgbPanel
+
+class Slider(Valuator):
+    def setMin(self) -> None: ...
+    def setMax(self) -> None: ...
+
+class SliderWidget(Pmw.MegaWidget):
+    value: float
+    formatString: str
+    increment: float
+    xPad: int
+    left: float
+    right: float
+    def __init__(self, parent=None, **kw) -> None: ...
+    def destroy(self) -> None: ...
+    def set(self, value: float, fCommand: bool = ...) -> None: ...
+    def get(self) -> float: ...
+    def updateIndicator(self, value: float) -> None: ...
+    def setMin(self) -> None: ...
+    def setMax(self) -> None: ...
+    def setNumDigits(self) -> None: ...
+    def setRelief(self) -> None: ...
+    def setBorderwidth(self) -> None: ...
+    def setBackground(self) -> None: ...
+    def highlightWidget(self, event: Unused) -> None: ...
+    def restoreWidget(self, event: Unused) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/SfxPlayer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/SfxPlayer.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ShadowDemo.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ShadowDemo.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ShadowPlacer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ShadowPlacer.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ShowBase.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ShowBase.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __all__ = ['ShowBase', 'WindowControls']
 
 from _typeshed import StrOrBytesPath
+from collections.abc import Callable
 from types import ModuleType
 from typing import Any, ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
-from direct._typing import SimpleCallback, Unused
+from direct._typing import Unused
 from direct.directnotify.Notifier import Notifier
 from direct.directtools.DirectSession import DirectSession
 from direct.p3d.AppRunner import AppRunner
 from direct.showutil.TexMemWatcher import TexMemWatcher
 from direct.task.Task import Task, TaskManager
 from panda3d._typing import Vec4Like
 from panda3d.core import (
@@ -84,16 +85,16 @@
     musicManagerIsValid: bool
     sfxManagerList: list[AudioManager]
     sfxManagerIsValidList: list[bool]
     wantStats: bool
     wantTk: bool
     wantWx: bool
     wantDirect: bool
-    exitFunc: SimpleCallback | None
-    finalExitCallbacks: list[SimpleCallback]
+    exitFunc: Callable[[], object] | None
+    finalExitCallbacks: list[Callable[[], object]]
     windowType: _WindowType
     requireWindow: bool
     win: GraphicsEngine
     frameRateMeter: FrameRateMeter | None
     sceneGraphAnalyzerMeter: SceneGraphAnalyzerMeter | None
     winList: list[GraphicsEngine]
     winControls: list[WindowControls]
@@ -144,15 +145,15 @@
     bboard: BulletinBoard
     taskMgr: TaskManager
     task_mgr: TaskManager
     jobMgr: JobManager
     particleMgr: ParticleSystemManager | None
     particleMgrEnabled: bool
     physicsMgr: PhysicsManager | None
-    phyiscsMgrEnabled: bool
+    physicsMgrEnabled: bool
     physicsMgrAngular: bool
     devices: InputDeviceManager
     AppHasAudioFocus: bool
     clock: ClockObject
     transitions: Transitions
     clientSleep: float
     multiClientSleep: bool
@@ -222,15 +223,15 @@
         size: LVecBase2i | tuple[int, int] | None = None,
         aspectRatio: float | None = None,
         makeCamera: bool = True,
         keepCamera: bool = False,
         scene: NodePath | None = None,
         stereo: bool | None = None,
         unexposedDraw: bool | None = None,
-        callbackWindowDict: dict[str, SimpleCallback] | None = None,
+        callbackWindowDict: dict[str, Callable[[], object]] | None = None,
         requireWindow: bool | None = None,
     ) -> GraphicsWindow: ...
     def close_window(self, win: GraphicsOutput, keepCamera: bool = False, removeWindow: bool = True) -> None: ...
     def open_default_window(
         self,
         props: WindowProperties | None = None,
         fbprops: FrameBufferProperties | None = None,
@@ -242,15 +243,15 @@
         size: LVecBase2i | tuple[int, int] | None = None,
         aspectRatio: float | None = None,
         makeCamera: bool = True,
         keepCamera: bool = ...,
         scene: NodePath | None = None,
         stereo: bool | None = None,
         unexposedDraw: bool | None = None,
-        callbackWindowDict: dict[str, SimpleCallback] | None = None,
+        callbackWindowDict: dict[str, Callable[[], object]] | None = None,
         requireWindow: bool | None = None,
         *,
         startDirect: bool = True,
     ) -> bool: ...
     def open_main_window(
         self,
         props: WindowProperties | None = None,
@@ -263,15 +264,15 @@
         size: LVecBase2i | tuple[int, int] | None = None,
         aspectRatio: float | None = None,
         makeCamera: bool = True,
         keepCamera: bool = ...,
         scene: NodePath | None = None,
         stereo: bool | None = None,
         unexposedDraw: bool | None = None,
-        callbackWindowDict: dict[str, SimpleCallback] | None = None,
+        callbackWindowDict: dict[str, Callable[[], object]] | None = None,
         requireWindow: bool | None = None,
     ) -> bool: ...
     def set_sleep(self, amount: float) -> None: ...
     def set_frame_rate_meter(self, flag: bool) -> None: ...
     def set_scene_graph_analyzer_meter(self, flag: bool) -> None: ...
     def setup_window_controls(self, winCtrl: WindowControls | None = None) -> None: ...
     def setup_render(self) -> None: ...
@@ -281,39 +282,39 @@
     def get_aspect_ratio(self, win: GraphicsEngine | None = None) -> float: ...
     def get_size(self, win: GraphicsEngine | None = None) -> tuple[float, float]: ...
     def make_camera(
         self,
         win: GraphicsOutput,
         sort: int = 0,
         scene: NodePath | None = None,
-        displayRegion: Vec4Like = ...,
+        displayRegion: Vec4Like = (0, 1, 0, 1),
         stereo: bool | None = None,
         aspectRatio: float | None = None,
         clearDepth: bool = ...,
         clearColor: Vec4Like | None = None,
         lens: Lens | None = None,
         camName: str = 'cam',
         mask: BitMask32 | int | None = None,
         useCamera: NodePath[Camera] | None = None,
     ) -> NodePath[Camera]: ...
     def make_camera2d(
         self,
         win: GraphicsOutput,
         sort: int = 10,
-        displayRegion: Vec4Like = ...,
-        coords: Vec4Like = ...,
+        displayRegion: Vec4Like = (0, 1, 0, 1),
+        coords: Vec4Like = (-1, 1, -1, 1),
         lens: Lens | None = None,
         cameraName: str | None = None,
     ) -> NodePath[Camera]: ...
     def make_camera2dp(
         self,
         win: GraphicsOutput,
         sort: int = 20,
-        displayRegion: Vec4Like = ...,
-        coords: Vec4Like = ...,
+        displayRegion: Vec4Like = (0, 1, 0, 1),
+        coords: Vec4Like = (-1, 1, -1, 1),
         lens: Lens | None = None,
         cameraName: str | None = None,
     ) -> NodePath[Camera]: ...
     def setup_data_graph(self) -> None: ...
     def setup_mouse(self, win: GraphicsWindow, fMultiWin: bool = False) -> NodePath[ButtonThrower]: ...
     def setup_mouse_cb(self, win: GraphicsWindow) -> tuple[list[NodePath[ButtonThrower]], list[MouseWatcher]]: ...
     def enable_software_mouse_pointer(self) -> None: ...
@@ -508,20 +509,20 @@
 class WindowControls:
     win: GraphicsEngine
     camera: NodePath | None
     camNode: Camera | None
     camera2d: NodePath | None
     mouseWatcher: MouseWatcher | None
     mouseKeyboard: NodePath | None
-    closeCommand: SimpleCallback
+    closeCommand: Callable[[], object]
     grid: Any
     def __init__(
         self,
         win: GraphicsEngine,
         cam: NodePath | None = None,
         camNode: Camera | None = None,
         cam2d: NodePath | None = None,
         mouseWatcher: MouseWatcher | None = None,
         mouseKeyboard: NodePath | None = None,
-        closeCmd: SimpleCallback = ...,
+        closeCmd: Callable[[], object] = ...,
         grid: Any = None,
     ) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ShowBaseGlobal.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ShowBaseGlobal.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/TaskThreaded.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/TaskThreaded.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/ThreeUpShow.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/ThreeUpShow.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class ThreeUpShow(ShowBase):
     def __init__(self) -> None: ...
     def makeCamera(  # type: ignore[override]
         self,
         win: GraphicsOutput,
         sort: Unused = 0,
         scene: Unused = None,
-        displayRegion: Unused = ...,
+        displayRegion: Unused = (0, 1, 0, 1),
         stereo: Unused = None,
         aspectRatio: Unused = None,
         clearDepth: Unused = 0,
         clearColor: Unused = None,
         lens: Unused = None,
         camName: Unused = 'cam',
         mask: Unused = None,
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/Transitions.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/Transitions.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     iris: NodePath | None
     fade: DirectFrame | None
     letterbox: NodePath | None
     fadeModel: NodePath | None
     imagePos: LVecBase3f
     alphaOff: LColor
     alphaOn: LColor
-    lerpFunc: type[LerpColorScaleInterval] | type[LerpColorInterval]
+    lerpFunc: type[LerpColorScaleInterval | LerpColorInterval]
     irisTaskName: str
     fadeTaskName: str
     letterboxTaskName: str
     def __init__(self, loader: object, model: NodePath | None = None, scale: float = 3.0, pos: LVecBase3f = ...) -> None: ...
     def __del__(self) -> None: ...
     def setFadeModel(self, model: NodePath | None, scale: float = 1.0) -> None: ...
     def loadFade(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showbase/VFSImporter.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showbase/VFSImporter.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 __all__ = ['register', 'reloadSharedPackage', 'reloadSharedPackages', 'sharedPackages']
 
 from _typeshed import StrOrBytesPath
 from collections.abc import Iterable
-from types import ModuleType
-from typing import Any
+from types import CodeType, ModuleType
 from typing_extensions import Final, Literal
 
 from direct._typing import Unused
 from panda3d.core import Filename, VirtualFile, VirtualFileSystem
 
 sharedPackages: dict[str, Literal[True]]
 vfs: Final[VirtualFileSystem]
 compiledExtensions: list[str]
 
 class VFSImporter:
     dir_path: Filename
     def __init__(self, path: Filename | str) -> None: ...
-    def find_module(self, fullname: str, path: Filename | None = None) -> VFSLoader | None: ...
+    def find_module(self, fullname: str, path: StrOrBytesPath | None = None) -> VFSLoader | None: ...
 
 class VFSLoader:
-    dir_path: Filename
+    dir_path: StrOrBytesPath
     timestamp: int | None
     filename: Filename
-    desc: bytes
+    desc: tuple[str, str, int]
     packagePath: Filename | None
     def __init__(
-        self, dir_path: Filename, vfile: VirtualFile | None, filename: Filename, desc: bytes, packagePath: Filename | None = None
+        self,
+        dir_path: StrOrBytesPath,
+        vfile: VirtualFile | None,
+        filename: Filename,
+        desc: tuple[str, str, int],
+        packagePath: Filename | None = None,
     ) -> None: ...
     def load_module(self, fullname: str, loadingShared: bool = False) -> ModuleType: ...
-    def getdata(self, path: StrOrBytesPath) -> bytes: ...
+    def getdata(self, path: str) -> bytes: ...
     def is_package(self, fullname: Unused) -> bool: ...
-    def get_code(self, fullname: Unused) -> Any | None: ...
+    def get_code(self, fullname: Unused) -> CodeType | None: ...
     def get_source(self, fullname: Unused) -> str | None: ...
     def get_filename(self, fullname: Unused) -> str: ...
 
 class VFSSharedImporter:
     def __init__(self) -> None: ...
-    def find_module(self, fullname: str, path: Iterable[str] | None = None, reload: bool = False) -> VFSSharedImporter | None: ...
+    def find_module(self, fullname: str, path: Iterable[str] | None = None, reload: bool = False) -> VFSSharedLoader | None: ...
     def getLoadedDirname(self, mod: ModuleType) -> str | None: ...
 
 class VFSSharedLoader:
     loaders: Iterable[VFSLoader]
     reload: bool
     def __init__(self, loaders: Iterable[VFSLoader], reload: bool) -> None: ...
-    def load_module(self, fullname: str) -> ModuleType | None: ...
+    def load_module(self, fullname: str) -> ModuleType: ...
 
 def register() -> None: ...
 def reloadSharedPackage(mod: ModuleType) -> None: ...
 def reloadSharedPackages() -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showutil/BuildGeometry.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showutil/BuildGeometry.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showutil/Effects.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showutil/Effects.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/showutil/TexMemWatcher.pyi` & `types-panda3d-0.3.3/src/direct-stubs/showutil/TexMemWatcher.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/stdpy/file.pyi` & `types-panda3d-0.3.3/src/direct-stubs/stdpy/file.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 __all__ = ['execfile', 'exists', 'getmtime', 'getsize', 'isdir', 'isfile', 'join', 'lexists', 'listdir', 'open', 'walk']
 
 from _typeshed import ReadableBuffer, StrOrBytesPath
 from collections.abc import Generator, Iterable, Mapping
 from io import IOBase
 from posixpath import join as join
-from typing import Any, TypeVar
+from typing import Any
 
 from direct._typing import Unused
 from panda3d.core import VirtualFile, istream, ostream
 
-_StrOrBytesPathT = TypeVar('_StrOrBytesPathT', bound=StrOrBytesPath)
-
 def open(
     file: StrOrBytesPath | VirtualFile | istream | ostream,
     mode: str = 'r',
     buffering: int = -1,
     encoding: str | None = None,
     errors: str | None = None,
     newline: str | None = None,
@@ -28,16 +26,16 @@
     def readline(self, size: Unused = -1) -> bytes: ...
     def seek(self, offset: int, whence: int = 0) -> None: ...  # type: ignore[override]
     def write(self, b: bytes) -> int: ...
     def writelines(self, lines: Iterable[ReadableBuffer]) -> None: ...
 
 def listdir(path: str) -> list[str]: ...
 def walk(
-    top: _StrOrBytesPathT, topdown: bool = True, onerror: object = None, followlinks: bool = True
-) -> Generator[tuple[_StrOrBytesPathT, list[str], list[str]], None, None]: ...
+    top: StrOrBytesPath, topdown: bool = True, onerror: object = None, followlinks: bool = True
+) -> Generator[tuple[StrOrBytesPath, list[str], list[str]], None, None]: ...
 def isfile(path: str) -> bool: ...
 def isdir(path: str) -> bool: ...
 def exists(path: str) -> bool: ...
 def lexists(path: str) -> bool: ...
 def getmtime(path: str) -> int: ...
 def getsize(path: str) -> int: ...
-def execfile(path: str, globals: dict[str, Any] | None = None, locals: Mapping[str, Any] | None = None) -> None: ...
+def execfile(path: str, globals: dict[str, Any] | None = None, locals: Mapping[str, object] | None = None) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/stdpy/pickle.pyi` & `types-panda3d-0.3.3/src/direct-stubs/stdpy/pickle.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/stdpy/thread.pyi` & `types-panda3d-0.3.3/src/direct-stubs/stdpy/thread.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Callable, Mapping, Sequence
+from collections.abc import Callable, Iterable, Mapping
 from typing import Any, NoReturn
 from typing_extensions import Final
 
 from direct._typing import Unused
 
 TIMEOUT_MAX: Final[float]
 
@@ -19,14 +19,14 @@
     def release(self) -> None: ...
     def locked(self) -> bool: ...
     def __enter__(self, waitflag: bool = ..., timeout: float = -1) -> bool: ...
     def __exit__(self, t: Unused, v: Unused, tb: Unused) -> None: ...  # noqa: Y036
     acquire = __enter__
 
 def start_new_thread(
-    function: Callable[..., object], args: Sequence[Any], kwargs: Mapping[str, Any] = ..., name: str | None = None
+    function: Callable[..., object], args: Iterable[Any], kwargs: Mapping[str, Any] = {}, name: str | None = None
 ) -> int: ...
 def interrupt_main() -> None: ...
 def exit() -> NoReturn: ...
 def allocate_lock() -> LockType: ...
 def get_ident() -> int: ...
 def stack_size(size: Unused = 0) -> NoReturn: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/stdpy/threading.pyi` & `types-panda3d-0.3.3/src/direct-stubs/stdpy/threading.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
 class Thread(ThreadBase):
     def __init__(
         self,
         group: None = None,
         target: Callable[..., object] | None = None,
         name: str | None = None,
-        args: Iterable[Any] = ...,
-        kwargs: Mapping[str, Any] = ...,
+        args: Iterable[Any] = (),
+        kwargs: Mapping[str, Any] = {},
         daemon: bool | None = None,
     ) -> None: ...
     def __del__(self) -> None: ...
     def is_alive(self) -> bool: ...
     isAlive = is_alive
     def start(self) -> None: ...
     def run(self) -> None: ...
@@ -115,15 +115,15 @@
 class Timer(Thread):
     interval: float
     function: Callable[..., object]
     args: Iterable[Any]
     kwargs: Mapping[str, Any]
     finished: Event
     def __init__(
-        self, interval: float, function: Callable[..., object], args: Iterable[Any] = ..., kwargs: Mapping[str, Any] = ...
+        self, interval: float, function: Callable[..., object], args: Iterable[Any] = [], kwargs: Mapping[str, Any] = {}
     ) -> None: ...
     def cancel(self) -> None: ...
 
 def current_thread() -> ExternalThread: ...
 def main_thread() -> MainThread: ...
 
 currentThread = current_thread
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/stdpy/threading2.pyi` & `types-panda3d-0.3.3/src/direct-stubs/stdpy/threading2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     name: str
     daemon: bool
     def __init__(
         self,
         group: None = None,
         target: Callable[..., object] | None = None,
         name: object = None,
-        args: Iterable[Any] = ...,
+        args: Iterable[Any] = (),
         kwargs: Mapping[str, Any] | None = None,
         verbose: bool | None = None,
         daemon: bool | None = None,
     ) -> None: ...
     def start(self) -> None: ...
     def run(self) -> None: ...
     def join(self, timeout: float | None = None) -> None: ...
@@ -104,15 +104,15 @@
 
 def Timer(
     interval: float | None, function: Callable[..., Any], args: Iterable[Any] = ..., kwargs: Mapping[str, Any] = ...
 ) -> _Timer: ...
 
 class _Timer(Thread):
     def __init__(
-        self, interval: float | None, function: Callable[..., Any], args: Iterable[Any] = ..., kwargs: Mapping[str, Any] = ...
+        self, interval: float | None, function: Callable[..., Any], args: Iterable[Any] = [], kwargs: Mapping[str, Any] = {}
     ) -> None: ...
     def cancel(self) -> None: ...
 
 def current_thread() -> Thread: ...
 
 currentThread = current_thread
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/task/MiniTask.pyi` & `types-panda3d-0.3.3/src/direct-stubs/task/MiniTask.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/task/Task.pyi` & `types-panda3d-0.3.3/src/direct-stubs/task/Task.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Final, Literal
 
 from direct._typing import Unused
 from direct.directnotify.Notifier import Notifier
 from direct.fsm.StatePush import StateVar
 from direct.showbase.ProfileSession import ProfileSession
 from direct.tkpanels.TaskManagerPanel import TaskManagerPanel
-from panda3d._typing import TaskCoroutine
+from panda3d._typing import TaskCoroutine, TaskFunction
 from panda3d.core import (
     AsyncFuture,
     AsyncTask,
     AsyncTaskManager,
     AsyncTaskPause,
     AsyncTaskPause as pause,
     AsyncTaskSequence,
@@ -66,37 +66,37 @@
     clock: ClockObject
     def __init__(self) -> None: ...
     def finalInit(self) -> None: ...
     def destroy(self) -> None: ...
     def setClock(self, clockObject: ClockObject) -> None: ...
     def invokeDefaultHandler(self, signalNumber: Unused, stackFrame: Unused) -> NoReturn: ...
     def keyboardInterruptHandler(self, signalNumber: Unused, stackFrame: Unused) -> None: ...
-    def getCurrentTask(self) -> Task | None: ...
+    def getCurrentTask(self) -> AsyncTask | None: ...
     def hasTaskChain(self, chainName: str) -> bool: ...
     def setupTaskChain(
         self,
         chainName: str,
         numThreads: int | None = None,
         tickClock: bool | None = None,
         threadPriority: Literal[0, 1, 2, 3, None] = None,
         frameBudget: float | None = None,
         frameSync: bool | None = None,
         timeslicePriority: bool | None = None,
     ) -> None: ...
     def hasTaskNamed(self, taskName: str) -> bool: ...
-    def getTasksNamed(self, taskName: str) -> list[Task]: ...
-    def getTasksMatching(self, taskPattern: str | GlobPattern) -> list[Task]: ...
-    def getAllTasks(self) -> list[Task]: ...
-    def getTasks(self) -> list[Task]: ...
-    def getDoLaters(self) -> list[Task]: ...
+    def getTasksNamed(self, taskName: str) -> list[AsyncTask]: ...
+    def getTasksMatching(self, taskPattern: str | GlobPattern) -> list[AsyncTask]: ...
+    def getAllTasks(self) -> list[AsyncTask]: ...
+    def getTasks(self) -> list[AsyncTask]: ...
+    def getDoLaters(self) -> list[AsyncTask]: ...
     @overload
     def do_method_later(
         self,
         delayTime: float,
-        funcOrTask: PythonTask | Callable[..., int | TaskCoroutine[int | None] | None] | TaskCoroutine[Any],
+        funcOrTask: PythonTask | TaskFunction | TaskCoroutine[Any],
         name: str | None,
         extraArgs: Sequence[Any] | None = None,
         sort: int | None = None,
         priority: int | None = None,
         taskChain: str | None = None,
         uponDeath: Callable[..., object] | None = None,
         appendTask: bool = False,
@@ -116,15 +116,15 @@
         appendTask: bool = False,
         owner: _TaskOwner | None = None,
     ) -> AsyncTask: ...
     doMethodLater = do_method_later
     @overload
     def add(
         self,
-        funcOrTask: PythonTask | Callable[..., int | TaskCoroutine[int | None] | None] | TaskCoroutine[Any],
+        funcOrTask: PythonTask | TaskFunction | TaskCoroutine[Any],
         name: str | None = None,
         sort: int | None = None,
         extraArgs: Sequence[Any] | None = None,
         priority: int | None = None,
         uponDeath: Callable[..., object] | None = None,
         appendTask: bool = False,
         taskChain: str | None = None,
@@ -163,8 +163,8 @@
     def getProfileFramesSV(self) -> StateVar[bool]: ...
     def setProfileFrames(self, profileFrames: bool) -> None: ...
     def getProfileTasks(self) -> bool: ...
     def getProfileTasksSV(self) -> StateVar[bool]: ...
     def setProfileTasks(self, profileTasks: bool) -> None: ...
     def logTaskProfiles(self, name: str | None = None) -> None: ...
     def flushTaskProfiles(self, name: str | None = None) -> None: ...
-    def doYield(self, frameStartTime: Unused, nextScheduledTaskTime: Unused) -> None: ...
+    def doYield(self, frameStartTime: float, nextScheduledTaskTime: float) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/task/TaskProfiler.pyi` & `types-panda3d-0.3.3/src/direct-stubs/task/TaskProfiler.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -23,10 +23,10 @@
     def __init__(self) -> None: ...
     def destroy(self) -> None: ...
     @staticmethod
     def GetDefaultSpikeThreshold() -> float: ...
     @staticmethod
     def SetSpikeThreshold(spikeThreshold: float) -> None: ...
     @staticmethod
-    def GetSpikeThreshold() -> float: ...
+    def GetSpikeThreshold() -> float | None: ...
     def logProfiles(self, name: str | None = None) -> None: ...
     def flush(self, name: str | None) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/task/Timer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/task/Timer.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/AnimPanel.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/AnimPanel.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     playList: list[ActorControl]
     actorControlIndex: int
     destroyCallBack: Callable[[], object] | None
     actorFrame: tkinter.Frame | None
     lastT: float
     fToggleAll: bool
     actorControlList: list[ActorControl]
-    def __init__(self, aList=..., parent=None, session=None, **kw) -> None: ...
+    def __init__(self, aList=[], parent=None, session=None, **kw) -> None: ...
     def createActorControls(self) -> None: ...
     def clearActorControls(self) -> None: ...
     def setActors(self) -> None: ...
     def loadAnim(self) -> None: ...
     def playActorControls(self) -> None: ...
     def play(self, task) -> Literal[1]: ...
     def stopActorControls(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/DirectSessionPanel.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/DirectSessionPanel.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,14 @@
     def toggleJoybox(self) -> None: ...
     def updateInfo(self, page: str = 'Environment') -> None: ...
     def updateEnvironmentInfo(self) -> None: ...
     def updateDisplayRegionInfo(self) -> None: ...
     def updateLightInfo(self, page=None) -> None: ...
     def updateGridInfo(self) -> None: ...
     def pushUndo(self, fResetRedo: bool = ...) -> None: ...
-    def undoHook(self, nodePathList=...) -> None: ...
+    def undoHook(self, nodePathList=[]) -> None: ...
     def pushUndoHook(self) -> None: ...
     def undoListEmptyHook(self) -> None: ...
     def pushRedo(self) -> None: ...
-    def redoHook(self, nodePathList=...) -> None: ...
+    def redoHook(self, nodePathList=[]) -> None: ...
     def pushRedoHook(self) -> None: ...
     def redoListEmptyHook(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/FSMInspector.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/FSMInspector.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/Inspector.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/Inspector.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/MopathRecorder.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/MopathRecorder.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -93,27 +93,27 @@
     extendPage: tkinter.Frame
     cropPage: tkinter.Frame
     drawPage: tkinter.Frame
     optionsPage: tkinter.Frame
     sf: Pmw.ScrolledFrame
     def __init__(self, parent: Unused = None, **kw) -> None: ...
     def pushUndo(self, fResetRedo: bool = ...) -> None: ...
-    def undoHook(self, nodePathList: Unused = ...) -> None: ...
+    def undoHook(self, nodePathList: Unused = []) -> None: ...
     def pushUndoHook(self) -> None: ...
     def undoListEmptyHook(self) -> None: ...
     def pushRedo(self) -> None: ...
-    def redoHook(self, nodePathList: Unused = ...) -> None: ...
+    def redoHook(self, nodePathList: Unused = []) -> None: ...
     def pushRedoHook(self) -> None: ...
     def redoListEmptyHook(self) -> None: ...
     def selectedNodePathHook(self, nodePath: NodePath) -> None: ...
     def getChildIds(self, nodePath: NodePath) -> list[int]: ...
     def deselectedNodePathHook(self, nodePath: NodePath) -> None: ...
     def curveEditTask(self, state: Unused) -> Literal[1]: ...
     def manipulateObjectStartHook(self) -> None: ...
-    def manipulateObjectCleanupHook(self, nodePathList: Unused = ...) -> None: ...
+    def manipulateObjectCleanupHook(self, nodePathList: Unused = []) -> None: ...
     def createNewPointSet(self) -> None: ...
     def extractPointSetFromCurveFitter(self) -> None: ...
     def extractPointSetFromCurveCollection(self) -> None: ...
     def selectPointSetNamed(self, name: str) -> None: ...
     def setPathVis(self) -> None: ...
     def setKnotVis(self) -> None: ...
     def setCvVis(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/NotifyPanel.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/NotifyPanel.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/ParticlePanel.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/ParticlePanel.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/Placer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/Placer.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -73,17 +73,17 @@
     def unitScale(self) -> None: ...
     def updateResetValues(self, nodePath: NodePath) -> None: ...
     def resetAll(self) -> None: ...
     def resetPos(self) -> None: ...
     def resetHpr(self) -> None: ...
     def resetScale(self) -> None: ...
     def pushUndo(self, fResetRedo: bool = ...) -> None: ...
-    def undoHook(self, nodePathList: Unused = ...) -> None: ...
+    def undoHook(self, nodePathList: Unused = []) -> None: ...
     def pushUndoHook(self) -> None: ...
     def undoListEmptyHook(self) -> None: ...
     def pushRedo(self) -> None: ...
-    def redoHook(self, nodePathList: Unused = ...) -> None: ...
+    def redoHook(self, nodePathList: Unused = []) -> None: ...
     def pushRedoHook(self) -> None: ...
     def redoListEmptyHook(self) -> None: ...
     def printNodePathInfo(self) -> None: ...
 
 def place(nodePath: NodePath) -> Placer: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkpanels/TaskManagerPanel.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkpanels/TaskManagerPanel.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/AppShell.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/AppShell.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
     def newCreateOptionMenu(
         self,
         parent,
         category: str,
         text: str,
         help: str = '',
         command=None,
-        items: list[str] = ...,
+        items: list[str] = [],
         labelpos='w',
         label_anchor: _TkAnchor = 'w',
         label_width: int = 16,
         menu_tearoff: int = 1,
         side: _TkSide = 'left',
         fill: _TkFill = 'x',
         expand: int = 0,
@@ -241,15 +241,15 @@
     def newCreateComboBox(
         self,
         parent,
         category: str,
         text: str,
         help: str = '',
         command=None,
-        items=...,
+        items=[],
         state: _TkState = 'disabled',
         history: Unused = 0,
         labelpos='w',
         label_anchor: _TkAnchor = 'w',
         label_width: int = 16,
         entry_width: int = 16,
         side: _TkSide = 'left',
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Dial.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Dial.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/EntryScale.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/EntryScale.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Floater.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Floater.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/MemoryExplorer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/MemoryExplorer.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/ProgressBar.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/ProgressBar.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/SceneGraphExplorer.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/SceneGraphExplorer.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __all__ = ['SceneGraphExplorer', 'SceneGraphExplorerItem', 'explore']
 
 from collections.abc import Mapping
-from typing_extensions import Final, Literal
+from typing_extensions import Final
 
 import Pmw  # type: ignore[import]
 from direct.showbase.DirectObject import DirectObject
 from panda3d.core import NodePath
 
 from .Tree import TreeItem
 
@@ -26,14 +26,14 @@
     nodePath: NodePath
     isItemEditable: bool
     def __init__(self, nodePath: NodePath, isItemEditable: bool = True) -> None: ...
     def GetText(self) -> str: ...
     def GetKey(self) -> int: ...
     def IsEditable(self) -> bool: ...
     def SetText(self, text: str) -> None: ...
-    def GetIconName(self) -> Literal['sphere2']: ...
+    def GetIconName(self) -> str: ...
     def IsExpandable(self) -> bool: ...
     def GetSubList(self) -> list[SceneGraphExplorerItem]: ...
     def OnSelect(self) -> None: ...
     def MenuCommand(self, command: str) -> None: ...
 
 def explore(nodePath: NodePath | None = None) -> SceneGraphExplorer: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Tree.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Tree.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 __all__ = ['TreeItem', 'TreeNode']
 
 import tkinter
 from abc import ABCMeta, abstractmethod
 from collections.abc import Mapping
 from typing import Any
-from typing_extensions import Final, Literal
+from typing_extensions import Final
 
 ICONDIR: Final[str]
 
 class TreeNode:
     canvas: tkinter.Canvas
     parent: TreeNode
     item: TreeItem
@@ -21,26 +21,26 @@
     iconimages: dict[str, tkinter.PhotoImage]
     menuList: list
     menuVar: Any
     fSortChildren: bool
     fModeChildrenTag: bool
     childrenTag: Mapping[str, bool]
     setAsTarget: bool
-    def __init__(self, canvas: tkinter.Canvas, parent, item, menuList: list = ...) -> None: ...
+    def __init__(self, canvas: tkinter.Canvas, parent, item, menuList: list = []) -> None: ...
     def setFSortChildren(self, fSortChildren: bool) -> None: ...
     def setChildrenTag(self, tag: Mapping[str, bool], fModeChildrenTag: bool) -> None: ...
     def destroy(self) -> None: ...
     def geticonimage(self, name: str) -> tkinter.PhotoImage: ...
     def select(self, event=None) -> None: ...
     def deselect(self, event=None) -> None: ...
     def deselectall(self) -> None: ...
     def deselecttree(self) -> None: ...
-    def flip(self, event=None) -> Literal['break']: ...
+    def flip(self, event=None) -> str: ...
     def createPopupMenu(self) -> None: ...
-    def popupMenu(self, event=None) -> Literal['break'] | None: ...
+    def popupMenu(self, event=None) -> str | None: ...
     def popupMenuCommand(self) -> None: ...
     def expand(self, event=None) -> None: ...
     def collapse(self, event=None) -> None: ...
     def view(self) -> None: ...
     def reveal(self) -> None: ...
     def lastvisiblechild(self): ...
     def updateAll(self, fMode: bool, depth: int = 0, fUseCachedChildren: bool = ...) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/Valuator.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/Valuator.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/VectorWidgets.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/VectorWidgets.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/tkwidgets/WidgetPropertiesDialog.pyi` & `types-panda3d-0.3.3/src/direct-stubs/tkwidgets/WidgetPropertiesDialog.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/wxwidgets/ViewPort.pyi` & `types-panda3d-0.3.3/src/direct-stubs/wxwidgets/ViewPort.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import wx.siplib as sip  # type: ignore[import]
 from direct.directtools.DirectGrid import DirectGrid
 from direct.showbase.DirectObject import DirectObject
 from panda3d.core import ButtonThrower, Camera, CollisionNode, Lens, LPoint3f, NodePath
 
 from .WxPandaWindow import WxPandaWindow
 
-HORIZONTAL: Final[Any]
-VERTICAL: Final[Any]
+HORIZONTAL: Final = 1
+VERTICAL: Final = 2
 CREATENEW: Final = 99
 VPLEFT: Final = 10
 VPFRONT: Final = 11
 VPTOP: Final = 12
 VPPERSPECTIVE: Final = 13
 
 class ViewportManager:
```

### Comparing `types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxAppShell.pyi` & `types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxAppShell.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxPandaShell.pyi` & `types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxPandaShell.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxPandaWindow.pyi` & `types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxPandaWindow.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/direct-stubs/wxwidgets/WxSlider.pyi` & `types-panda3d-0.3.3/src/direct-stubs/wxwidgets/WxSlider.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         minValue: float,
         maxValue: float,
         pos=...,
         size=...,
         style=4,
         validator=...,
         name: str = 'slider',
-        textSize: tuple[int, int] = ...,
+        textSize: tuple[int, int] = (40, 20),
     ) -> None: ...
     def GetValue(self) -> float: ...
     def SetValue(self, value: float) -> None: ...
     def onChange(self, event) -> None: ...
     def onEnter(self, event) -> None: ...
     def bindFunc(self, updateCB) -> None: ...
     def Disable(self) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/_rplight.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/_rplight.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/_typing.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/_typing.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from collections.abc import Coroutine, Generator
+from collections.abc import Callable, Coroutine, Generator
 from typing import Any, TypeVar
 from typing_extensions import TypeAlias
 
 from panda3d.core._downloader import URLSpec
 from panda3d.core._dtoolutil import DSearchPath, Filename
 from panda3d.core._linmath import (
     ConfigVariableColor,
@@ -35,7 +35,8 @@
 DoubleVec4Like: TypeAlias = LVecBase4d | LMatrix4d.Row | LMatrix4d.CRow | tuple[float, float, float, float]
 IntVec4Like: TypeAlias = LVecBase4i | tuple[int, int, int, int]
 Mat4Like: TypeAlias = LMatrix3f | LMatrix4f | UnalignedLMatrix4f
 DoubleMat4Like: TypeAlias = LMatrix3d | LMatrix4d | UnalignedLMatrix4d
 URL: TypeAlias = URLSpec | str
 SearchPathLike: TypeAlias = ConfigVariableFilename | ConfigVariableSearchPath | DSearchPath | Filename | str
 TaskCoroutine: TypeAlias = Coroutine[Any, None, _T_co] | Generator[Any, None, _T_co]
+TaskFunction: TypeAlias = Callable[..., int | TaskCoroutine[int | None] | None]
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/ai.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/ai.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/bullet.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/bullet.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/__init__.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_audio.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_audio.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_chan.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_chan.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -713,15 +713,15 @@
     @overload
     def __init__(self, __param0: BindAnimRequest) -> None: ...
     @overload
     def __init__(
         self,
         name: str,
         filename: StrOrBytesPath,
-        options: LoaderOptions | int,
+        options: LoaderOptions,
         loader: Loader,
         control: AnimControl,
         hierarchy_match_flags: int,
         subset: PartSubset,
     ) -> None: ...
 
 class PartBundle(PartGroup):
@@ -1061,32 +1061,32 @@
         to get_max_bound().
         """
     def output_value(self, out: ostream) -> None: ...
     getMaxBound = get_max_bound
     getBound = get_bound
     outputValue = output_value
 
-class MovingPartMatrix(MovingPart_ACMatrixSwitchType):
-    """This is a particular kind of MovingPart that accepts a matrix each frame."""
-
 class MovingPart_ACMatrixSwitchType(MovingPartBase):
     def get_value(self) -> LMatrix4: ...
     def get_default_value(self) -> LMatrix4: ...
     getValue = get_value
     getDefaultValue = get_default_value
 
-class MovingPartScalar(MovingPart_ACScalarSwitchType):
-    """This is a particular kind of MovingPart that accepts a scalar each frame."""
+class MovingPartMatrix(MovingPart_ACMatrixSwitchType):
+    """This is a particular kind of MovingPart that accepts a matrix each frame."""
 
 class MovingPart_ACScalarSwitchType(MovingPartBase):
     def get_value(self) -> float: ...
     def get_default_value(self) -> float: ...
     getValue = get_value
     getDefaultValue = get_default_value
 
+class MovingPartScalar(MovingPart_ACScalarSwitchType):
+    """This is a particular kind of MovingPart that accepts a scalar each frame."""
+
 def auto_bind(root_node: PandaNode, controls: AnimControlCollection, hierarchy_match_flags: int = ...) -> None: ...
 
 autoBind = auto_bind
 AnimChannelACMatrixSwitchType = AnimChannel_ACMatrixSwitchType
 AnimChannelMatrix = AnimChannel_ACMatrixSwitchType
 AnimChannelACScalarSwitchType = AnimChannel_ACScalarSwitchType
 AnimChannelScalar = AnimChannel_ACScalarSwitchType
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_char.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_char.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_collide.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_collide.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import MutableSequence, Sequence
 from typing import overload
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 from panda3d._typing import Vec2Like, Vec3Like, Vec4Like
 from panda3d.core._dtoolbase import TypedObject
 from panda3d.core._dtoolutil import ostream
 from panda3d.core._express import Datagram, DatagramIterator, Namable, TypedReferenceCount
 from panda3d.core._linmath import LPoint3, LPoint3i, LVector3
 from panda3d.core._mathutil import BoundingVolume, LParabola, LPlane
@@ -101,21 +101,21 @@
 
         `(self, center: LPoint3, x: float, y: float, z: float)`:
         Create the Box by giving a Center and distances of each of the sides of
         box from the Center.
         """
     @overload
     def __init__(self, center: Vec3Like, x: float, y: float, z: float) -> None: ...
-    def get_num_points(self) -> Literal[8]:
+    def get_num_points(self) -> int:
         """Returns 8: the number of vertices of a rectangular solid."""
     def get_point_aabb(self, n: int) -> LPoint3:
         """Returns the nth vertex of the Axis Aligned Bounding Box."""
     def get_point(self, n: int) -> LPoint3:
         """Returns the nth vertex of the OBB."""
-    def get_num_planes(self) -> Literal[6]:
+    def get_num_planes(self) -> int:
         """Returns 6: the number of faces of a rectangular solid."""
     def set_plane(self, n: int) -> LPlane:
         """Creates the nth face of the rectangular solid."""
     def get_plane(self, n: int) -> LPlane:
         """Returns the nth face of the rectangular solid."""
     @overload
     def set_center(self, center: Vec3Like) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_device.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_device.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     def _pointer_data(self) -> PointerData: ...
     @property
     def _battery_data(self) -> InputDevice.BatteryData: ...
     @property
     def _tracker_data(self) -> TrackerData: ...
     def has_feature(self, feature: InputDevice.Feature) -> bool:
         """Returns true if the device supports the indicated feature."""
-    def map_button(self, index: int, handle: ButtonHandle | int | str) -> None:
+    def map_button(self, index: int, handle: ButtonHandle | str) -> None:
         """Associates the indicated ButtonHandle with the button of the indicated index
         number.  When the given button index changes state, a corresponding
         ButtonEvent will be generated with the given ButtonHandle.  Pass
         ButtonHandle::none() to turn off any association.
 
         It is not necessary to call this if you simply want to query the state of
         the various buttons by index number; this is only necessary in order to
@@ -180,15 +180,15 @@
     def map_axis(self, index: int, axis: InputDevice.Axis) -> None:
         """Associates the indicated Axis with the axis of the indicated index
         number.  Pass Axis::none to turn off any association.
 
         It is not necessary to call this if you simply want to query the state of
         the various axes by index number.
         """
-    def find_button(self, handle: ButtonHandle | int | str) -> InputDevice.ButtonState:
+    def find_button(self, handle: ButtonHandle | str) -> InputDevice.ButtonState:
         """Returns the first ButtonState found with the given axis, or throw an assert
         if the button handle was not found in the list.
         """
     def find_axis(self, axis: InputDevice.Axis) -> InputDevice.AxisState:
         """Returns the first AnalogAxis found with the given axis, or throw an assert
         if the axis was not found in the list.
         """
@@ -374,15 +374,15 @@
         """
     def get_num_buttons(self) -> int:
         """Returns the number of buttons known to the ButtonNode.  This includes those
         buttons whose state has been seen, as well as buttons that have been
         associated with a ButtonHandle even if their state is unknown.  This number
         may change as more buttons are discovered.
         """
-    def set_button_map(self, index: int, button: ButtonHandle | int | str) -> None:
+    def set_button_map(self, index: int, button: ButtonHandle | str) -> None:
         """Associates the indicated ButtonHandle with the button of the indicated
         index number.  When the given button index changes state, a corresponding
         ButtonEvent will be generated with the given ButtonHandle.  Pass
         ButtonHandle::none() to turn off any association.
 
         It is not necessary to call this if you simply want to query the state of
         the various buttons by index number; this is only necessary in order to
@@ -451,16 +451,18 @@
     """Manages a list of InputDevice objects, as returned by various
     InputDeviceManager methods.  This is implemented like a set, meaning the
     same device cannot occur more than once.
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: InputDeviceSet = ...) -> None: ...
-    def __getitem__(self, index: int) -> InputDevice: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> InputDevice:
+        """Returns the nth InputDevice in the collection."""
+    def __len__(self) -> int:
+        """Returns the number of devices in the collection."""
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[InputDevice]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def clear(self) -> None:
         """Removes all InputDevices from the collection."""
     def reserve(self, num: int) -> None:
@@ -614,20 +616,20 @@
         meaning of the values passed to set_mouse_pos().
         """
     def set_mouse_on(self, flag: bool) -> None:
         """Sets whether the mouse should appear to be within the window or not.  If
         this is true, the mouse is within the window; if false, the mouse is not
         within the window (and set_mouse_pos() means nothing).
         """
-    def press_button(self, button: ButtonHandle | int | str) -> None:
+    def press_button(self, button: ButtonHandle | str) -> None:
         """Simulates a mouse or keyboard button being depressed.  This should be
         followed up by a call to release_button() sometime later (possibly
         immediately).
         """
-    def release_button(self, button: ButtonHandle | int | str) -> None:
+    def release_button(self, button: ButtonHandle | str) -> None:
         """Simulates the button being released.  This should follow a previous call to
         press_button().
         """
     setMousePos = set_mouse_pos
     setWindowSize = set_window_size
     setMouseOn = set_mouse_on
     pressButton = press_button
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_dgraph.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_dgraph.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_display.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_display.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -524,14 +524,15 @@
             for the particular representation.  Returns 0 if it is not.
             """
         def output(self, out: ostream) -> None: ...
         @staticmethod
         def get_class_type() -> TypeHandle: ...
         getIntHandle = get_int_handle
         getClassType = get_class_type
+
     os_handle: WindowHandle.OSHandle
     @overload
     def __init__(self, copy: WindowHandle) -> None: ...
     @overload
     def __init__(self, os_handle: WindowHandle.OSHandle) -> None: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
@@ -3267,24 +3268,24 @@
 
 class GraphicsWindowInputDevice(InputDevice):
     """This is a virtual input device that represents the keyboard and mouse pair
     that is associated with a particular window.  It collects mouse and
     keyboard events from the windowing system while the window is in focus.
     """
 
-    def button_down(self, button: ButtonHandle | int | str, time: float = ...) -> None:
+    def button_down(self, button: ButtonHandle | str, time: float = ...) -> None:
         """The following interface is for the various kinds of GraphicsWindows to
         record the data incoming on the device.
         """
-    def button_resume_down(self, button: ButtonHandle | int | str, time: float = ...) -> None:
+    def button_resume_down(self, button: ButtonHandle | str, time: float = ...) -> None:
         """Records that the indicated button was depressed earlier, and we only just
         detected the event after the fact.  This is mainly useful for tracking the
         state of modifier keys.
         """
-    def button_up(self, button: ButtonHandle | int | str, time: float = ...) -> None:
+    def button_up(self, button: ButtonHandle | str, time: float = ...) -> None:
         """Records that the indicated button has been released."""
     def keystroke(self, keycode: int, time: float = ...) -> None:
         """Records that the indicated keystroke has been generated."""
     def candidate(self, candidate_string: str, highlight_start: int, highlight_end: int, cursor_pos: int) -> None:
         """Records that the indicated candidate string has been highlighted.  This is
         used to implement IME support for typing in international languages,
         especially Chinese/Japanese/Korean.
@@ -3292,17 +3293,17 @@
     def focus_lost(self, time: float = ...) -> None:
         """This should be called when the window focus is lost, so that we may miss
         upcoming button events (especially "up" events) for the next period of
         time.  It generates keyboard and mouse "up" events for those buttons that
         we previously sent unpaired "down" events, so that the Panda application
         will believe all buttons are now released.
         """
-    def raw_button_down(self, button: ButtonHandle | int | str, time: float = ...) -> None:
+    def raw_button_down(self, button: ButtonHandle | str, time: float = ...) -> None:
         """Records that the indicated button has been depressed."""
-    def raw_button_up(self, button: ButtonHandle | int | str, time: float = ...) -> None:
+    def raw_button_up(self, button: ButtonHandle | str, time: float = ...) -> None:
         """Records that the indicated button has been released."""
     def get_pointer(self) -> PointerData:
         """Returns the PointerData associated with the input device's pointer.  This
         only makes sense if has_pointer() also returns true.
         """
     def set_pointer_in_window(self, x: float, y: float, time: float = ...) -> None:
         """To be called by a particular kind of GraphicsWindow to indicate that the
@@ -3629,14 +3630,15 @@
         @staticmethod
         def get_class_type() -> TypeHandle: ...
         getCallbackType = get_callback_type
         getFrameMode = get_frame_mode
         setRenderFlag = set_render_flag
         getRenderFlag = get_render_flag
         getClassType = get_class_type
+
     RCT_begin_frame: Final = 0
     RCTBeginFrame: Final = 0
     RCT_end_frame: Final = 1
     RCTEndFrame: Final = 1
     RCT_begin_flip: Final = 2
     RCTBeginFlip: Final = 2
     RCT_end_flip: Final = 3
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_downloader.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_downloader.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """Receives a datagram over the socket by expecting a little-endian 16-bit
         byte count as a prefix.  If the socket stream is non-blocking, may return
         false if the data is not available; otherwise, returns false only if the
         socket closes.
         """
     def is_closed(self) -> bool: ...
     def close(self) -> None: ...
-    def set_tcp_header_size(self, tcp_header_size: Literal[0, 2, 4]) -> None:
+    def set_tcp_header_size(self, tcp_header_size: int) -> None:
         """Sets the header size for datagrams.  At the present, legal values for this
         are 0, 2, or 4; this specifies the number of bytes to use encode the
         datagram length at the start of each TCP datagram.  Sender and receiver
         must independently agree on this.
         """
     def get_tcp_header_size(self) -> int:
         """Returns the header size for datagrams.  See set_tcp_header_size()."""
@@ -86,15 +86,15 @@
         meaning if "collect-tcp" mode is enabled; see set_collect_tcp().
         """
     def get_collect_tcp_interval(self) -> float:
         """Returns the interval in time, in seconds, for which to hold TCP packets
         before sending all of the recently received packets at once.  This only has
         meaning if "collect-tcp" mode is enabled; see set_collect_tcp().
         """
-    def set_tcp_header_size(self, tcp_header_size: Literal[0, 2, 4]) -> None:
+    def set_tcp_header_size(self, tcp_header_size: int) -> None:
         """Sets the header size for datagrams.  At the present, legal values for this
         are 0, 2, or 4; this specifies the number of bytes to use encode the
         datagram length at the start of each TCP datagram.  Sender and receiver
         must independently agree on this.
         """
     def get_tcp_header_size(self) -> int:
         """Returns the header size for datagrams.  See set_tcp_header_size()."""
@@ -1034,15 +1034,15 @@
     tag: HTTPEntityTag
     date: HTTPDate
     request_mode: _DocumentSpec_RequestMode
     cache_control: _DocumentSpec_CacheControl
     @overload
     def __init__(self, copy: DocumentSpec = ...) -> None: ...
     @overload
-    def __init__(self, url: URL) -> None: ...
+    def __init__(self, url: URLSpec | str) -> None: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: DocumentSpec | URL) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def assign(self, copy: DocumentSpec | URL) -> Self: ...
     def compare_to(self, other: DocumentSpec | URL) -> int: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_dtoolbase.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_dtoolbase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_dtoolutil.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_dtoolutil.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -7,44 +7,34 @@
 from panda3d.core._dtoolbase import TypeHandle
 
 _ios_base_seekdir: TypeAlias = Literal[0, 1, 2]
 _ios_base_openmode: TypeAlias = int
 _TextEncoder_Encoding: TypeAlias = Literal[0, 1, 2, 2]
 _Filename_Type: TypeAlias = Literal[0, 1, 2]
 
-class basic_ios_char(ios_base):
-    def good(self) -> bool: ...
-    def eof(self) -> bool: ...
-    def fail(self) -> bool: ...
-    def bad(self) -> bool: ...
-    def clear(self) -> None: ...
-
 class ios_base:
     """We need to expose one method in each class to force it to publish.
     But we'd like to expose some of these methods anyway, so no
     problem.
     """
 
     beg: Final = 0
     Beg: Final = 0
     cur: Final = 1
     Cur: Final = 1
     end: Final = 2
     End: Final = 2
     DtoolClassDict: ClassVar[dict[str, Any]]
 
-class fstream(iostream):
-    def __init__(self) -> None: ...
-    def close(self) -> None: ...
-
-class iostream(istream, ostream):  # type: ignore[misc]
-    def upcast_to_istream(self) -> istream: ...
-    def upcast_to_ostream(self) -> ostream: ...
-    upcastToIstream = upcast_to_istream
-    upcastToOstream = upcast_to_ostream
+class basic_ios_char(ios_base):
+    def good(self) -> bool: ...
+    def eof(self) -> bool: ...
+    def fail(self) -> bool: ...
+    def bad(self) -> bool: ...
+    def clear(self) -> None: ...
 
 class istream(basic_ios_char):
     def upcast_to_basic_ios_char(self) -> basic_ios_char: ...
     def get(self) -> int: ...
     def tellg(self) -> int: ...
     @overload
     def seekg(self, pos: int) -> None: ...
@@ -59,14 +49,24 @@
     def tellp(self) -> int: ...
     @overload
     def seekp(self, pos: int) -> None: ...
     @overload
     def seekp(self, off: int, dir: _ios_base_seekdir) -> None: ...
     upcastToBasicIosChar = upcast_to_basic_ios_char
 
+class iostream(istream, ostream):  # type: ignore[misc]
+    def upcast_to_istream(self) -> istream: ...
+    def upcast_to_ostream(self) -> ostream: ...
+    upcastToIstream = upcast_to_istream
+    upcastToOstream = upcast_to_ostream
+
+class fstream(iostream):
+    def __init__(self) -> None: ...
+    def close(self) -> None: ...
+
 class ifstream(istream):
     def __init__(self) -> None: ...
     def close(self) -> None: ...
 
 class ofstream(ostream):
     def __init__(self) -> None: ...
     def close(self) -> None: ...
@@ -400,18 +400,27 @@
     @overload
     def __init__(self, dirname: StrOrBytesPath, basename: StrOrBytesPath) -> None: ...
     def __getitem__(self, n: int) -> str: ...
     def __fspath__(self) -> str: ...
     def __iadd__(self, other: str) -> Self: ...
     def __add__(self, other: str) -> Filename: ...
     def __truediv__(self, other: StrOrBytesPath) -> Filename: ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison operators are handy."""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: str) -> bool: ...
-    def __bool__(self) -> bool: ...
+    def __bool__(self) -> bool:
+        """Returns true if the Filename is valid (not empty), or false if it is an
+        empty string.
+
+        This implements the Python equivalent to operator bool.  Defining an actual
+        operator bool method for C++ use would work too, but it seems to cause too
+        many ambiguities for the C++ compiler, so we use this Python-only approach
+        instead.
+        """
     @staticmethod
     def text_filename(filename: StrOrBytesPath) -> Filename:
         """Static constructors to explicitly create a filename that refers to a text
         or binary file.  This is in lieu of calling set_text() or set_binary() or
         set_type().
         """
     @staticmethod
@@ -1224,29 +1233,33 @@
     delimited by spaces or colons, but it can also be built up explicitly.
     """
 
     class Results:
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, copy: DSearchPath.Results = ...) -> None: ...
         def __getitem__(self, n: int) -> Filename: ...
-        def __len__(self) -> int: ...
+        def __len__(self) -> int:
+            """Returns the num of filenames in the set.  This method is defined to make
+            the Results object appear to be a list in Python.
+            """
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[Filename]: ...  # Doesn't actually exist
         def assign(self, copy: DSearchPath.Results) -> Self: ...
         def clear(self) -> None:
             """Removes all the files from the list."""
         def get_num_files(self) -> int:
             """Returns the number of files on the result list."""
         def get_file(self, n: int) -> Filename:
             """Returns the nth file on the result list."""
         def output(self, out: ostream) -> None: ...
         def write(self, out: ostream, indent_level: int = ...) -> None: ...
         getNumFiles = get_num_files
         getFile = get_file
+
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def directories(self) -> Sequence[Filename]: ...
     @overload
     def __init__(self, copy: SearchPathLike = ...) -> None: ...
     @overload
     def __init__(self, directory: StrOrBytesPath) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_dxml.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_dxml.pyi`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,52 +77,14 @@
         can be disabled if TiXmlDocument::SetTabSize() is called with 0 as the value.
 
         @sa TiXmlDocument::SetTabSize()
         """
     def Column(self) -> int:
         """< See Row()"""
 
-class TiXmlDeclaration(TiXmlNode):
-    """In correct XML the declaration is the first entry in the file.
-    @verbatim
-        <?xml version="1.0" standalone="yes"?>
-    @endverbatim
-
-    TinyXml will happily read or write files without a declaration,
-    however. There are 3 possible attributes to the declaration:
-    version, encoding, and standalone.
-
-    Note: In this version of the code, the attributes are
-    handled as special cases, not generic attributes, simply
-    because there can only be at most 3 and they are always the same.
-    """
-
-    @overload
-    def __init__(self, copy: TiXmlDeclaration = ...) -> None:
-        """`(self)`:
-        Construct an empty declaration.
-
-        `(self, _version: str, _encoding: str, _standalone: str)`:
-        Construct.
-
-        `(self, _version: str, _encoding: str, _standalone: str)`:
-        Constructor.
-        """
-    @overload
-    def __init__(self, _version: str, _encoding: str, _standalone: str) -> None: ...
-    def __copy__(self) -> Self: ...
-    def __deepcopy__(self, __memo: object) -> Self: ...
-    def assign(self, copy: Self) -> Self: ...
-    def Version(self) -> str:
-        """Version. Will return an empty string if none was found."""
-    def Encoding(self) -> str:
-        """Encoding. Will return an empty string if none was found."""
-    def Standalone(self) -> str:
-        """Is this a standalone document?"""
-
 class TiXmlNode(TiXmlBase):
     """The parent class for everything in the Document Object Model.
     (Except for attributes).
     Nodes have siblings, a parent, and children. A node can be
     in a document, or stand on its own. The type of a TiXmlNode
     can be queried, and it can be cast to its more defined type.
     """
@@ -341,14 +303,52 @@
         @verbatim
         TiXmlPrinter printer;
         tinyxmlDoc.Accept( &printer );
         const char* xmlcstr = printer.CStr();
         @endverbatim
         """
 
+class TiXmlDeclaration(TiXmlNode):
+    """In correct XML the declaration is the first entry in the file.
+    @verbatim
+        <?xml version="1.0" standalone="yes"?>
+    @endverbatim
+
+    TinyXml will happily read or write files without a declaration,
+    however. There are 3 possible attributes to the declaration:
+    version, encoding, and standalone.
+
+    Note: In this version of the code, the attributes are
+    handled as special cases, not generic attributes, simply
+    because there can only be at most 3 and they are always the same.
+    """
+
+    @overload
+    def __init__(self, copy: TiXmlDeclaration = ...) -> None:
+        """`(self)`:
+        Construct an empty declaration.
+
+        `(self, _version: str, _encoding: str, _standalone: str)`:
+        Construct.
+
+        `(self, _version: str, _encoding: str, _standalone: str)`:
+        Constructor.
+        """
+    @overload
+    def __init__(self, _version: str, _encoding: str, _standalone: str) -> None: ...
+    def __copy__(self) -> Self: ...
+    def __deepcopy__(self, __memo: object) -> Self: ...
+    def assign(self, copy: Self) -> Self: ...
+    def Version(self) -> str:
+        """Version. Will return an empty string if none was found."""
+    def Encoding(self) -> str:
+        """Encoding. Will return an empty string if none was found."""
+    def Standalone(self) -> str:
+        """Is this a standalone document?"""
+
 class TiXmlDocument(TiXmlNode):
     """Always the top level node. A document binds together all the
     XML pieces. It can be saved, loaded, and printed to the screen.
     The 'value' of a document node is the xml file name.
     """
 
     @overload
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_event.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_event.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import Callable, Generator, Iterator, Sequence
 from typing import Any, ClassVar, overload
 from typing_extensions import Final, Literal, Self, TypeAlias, final
 
-from panda3d._typing import TaskCoroutine
+from panda3d._typing import TaskCoroutine, TaskFunction
 from panda3d.core._dtoolbase import TypedObject
 from panda3d.core._dtoolutil import GlobPattern, ostream
 from panda3d.core._express import Namable, TypedReferenceCount
 from panda3d.core._putil import (
     ButtonHandle,
     ClockObject,
     ModifierButtons,
@@ -631,16 +631,22 @@
     query functions.  This also serves to define an AsyncTaskSequence.
 
     TODO: None of this is thread-safe yet.
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: AsyncTaskCollection = ...) -> None: ...
-    def __getitem__(self, index: int) -> AsyncTask: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> AsyncTask:
+        """Returns the nth AsyncTask in the collection.  This is the same as
+        get_task(), but it may be a more convenient way to access it.
+        """
+    def __len__(self) -> int:
+        """Returns the number of tasks in the collection.  This is the same thing as
+        get_num_tasks().
+        """
     def __iadd__(self, other: AsyncTaskCollection) -> Self: ...
     def __add__(self, other: AsyncTaskCollection) -> AsyncTaskCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[AsyncTask]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_task(self, task: AsyncTask) -> None:
@@ -1230,21 +1236,19 @@
         """Alias of wake_time."""
     @property
     def frame(self) -> int:
         """The number of frames that have elapsed since the task was started,
         according to the task manager's clock.
         """
     @overload
-    def __init__(
-        self, function: Callable[..., int | TaskCoroutine[int | None] | None] | TaskCoroutine[Any] | None = ..., name: str = ...
-    ) -> None: ...
+    def __init__(self, function: TaskCoroutine[Any] | TaskFunction | None = ..., name: str = ...) -> None: ...
     @overload
     def __init__(self, __param0: PythonTask) -> None: ...
-    def set_function(self, function: Callable[..., int | TaskCoroutine[int | None] | None] | None) -> None: ...
-    def get_function(self) -> Callable[..., int | TaskCoroutine[int | None] | None] | None:
+    def set_function(self, function: TaskFunction | None) -> None: ...
+    def get_function(self) -> TaskFunction | None:
         """Returns the function that is called when the task runs."""
     def set_args(self, args: Sequence[Any] | None, append_task: bool) -> None: ...
     def get_args(self) -> tuple[Any, ...]: ...
     def set_upon_death(self, upon_death: Callable[[], object] | None) -> None: ...
     def get_upon_death(self) -> Callable[[], object] | None:
         """Returns the function that is called when the task finishes."""
     def set_owner(self, owner) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_express.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_express.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,42 @@
 from panda3d.core._dtoolutil import DSearchPath, Filename, iostream, istream, ostream
 from panda3d.core._prc import ConfigVariableFilename, IStreamWrapper, OStreamWrapper, StreamReader, StreamWrapper, StreamWriter
 
 _ErrorUtilCode: TypeAlias = int
 _WindowsRegistry_RegLevel: TypeAlias = Literal[0, 1]
 _WindowsRegistry_Type: TypeAlias = Literal[0, 1, 2]
 
+class PointerToVoid:
+    """This is the non-template part of the base class for PointerTo and
+    ConstPointerTo.  It is necessary so we can keep a pointer to a non-template
+    class within the ReferenceCount object, to implement weak reference
+    pointers--we need to have something to clean up when the ReferenceCount
+    object destructs.
+
+    This is the base class for PointerToBase<T>.
+    """
+
+    DtoolClassDict: ClassVar[dict[str, Any]]
+    def is_null(self) -> bool:
+        """Returns true if the PointerTo is a NULL pointer, false otherwise.  (Direct
+        comparison to a NULL pointer also works.)
+        """
+    def get_hash(self) -> int: ...
+    isNull = is_null
+    getHash = get_hash
+
+class PointerToBase_ReferenceCountedVector_double(PointerToVoid):
+    def clear(self) -> None: ...
+    def output(self, out: ostream) -> None: ...
+
+class PointerToArrayBase_double(PointerToBase_ReferenceCountedVector_double):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_double(PointerToArrayBase_double):
     def __init__(self, copy: ConstPointerToArray_double | PointerToArray_double) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> float: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_double: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
@@ -28,40 +56,22 @@
     def count(self, __param0: float) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_double(PointerToBase_ReferenceCountedVector_double):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_double(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_float(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
-class PointerToVoid:
-    """This is the non-template part of the base class for PointerTo and
-    ConstPointerTo.  It is necessary so we can keep a pointer to a non-template
-    class within the ReferenceCount object, to implement weak reference
-    pointers--we need to have something to clean up when the ReferenceCount
-    object destructs.
-
-    This is the base class for PointerToBase<T>.
-    """
-
-    DtoolClassDict: ClassVar[dict[str, Any]]
-    def is_null(self) -> bool:
-        """Returns true if the PointerTo is a NULL pointer, false otherwise.  (Direct
-        comparison to a NULL pointer also works.)
-        """
-    def get_hash(self) -> int: ...
-    isNull = is_null
-    getHash = get_hash
+class PointerToArrayBase_float(PointerToBase_ReferenceCountedVector_float):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
 
 class ConstPointerToArray_float(PointerToArrayBase_float):
     def __init__(self, copy: ConstPointerToArray_float | PointerToArray_float) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> float: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_float: ...
     def __copy__(self) -> Self: ...
@@ -74,22 +84,23 @@
     def count(self, __param0: float) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_float(PointerToBase_ReferenceCountedVector_float):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_float(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_int(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_int(PointerToBase_ReferenceCountedVector_int):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_int(PointerToArrayBase_int):
     def __init__(self, copy: ConstPointerToArray_int | PointerToArray_int) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> int: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_int: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
@@ -101,22 +112,23 @@
     def count(self, __param0: int) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_int(PointerToBase_ReferenceCountedVector_int):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_int(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_unsigned_char(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_unsigned_char(PointerToBase_ReferenceCountedVector_unsigned_char):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_unsigned_char(PointerToArrayBase_unsigned_char):
     def __init__(self, copy: ConstPointerToArray_unsigned_char | PointerToArray_unsigned_char) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> str: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_unsigned_char: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[str]: ...  # Doesn't actually exist
@@ -128,22 +140,14 @@
     def count(self, __param0: str) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_unsigned_char(PointerToBase_ReferenceCountedVector_unsigned_char):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_unsigned_char(PointerToVoid):
-    def clear(self) -> None: ...
-    def output(self, out: ostream) -> None: ...
-
 class PointerToArray_double(PointerToArrayBase_double):
     @overload
     def __init__(self, type_handle: TypeHandle | type = ...) -> None: ...
     @overload
     def __init__(self, copy: PointerToArray_double) -> None: ...
     @overload
     def __init__(self, source: Sequence[float]) -> None: ...
@@ -1001,29 +1005,14 @@
     putDatagram = put_datagram
     copyDatagram = copy_datagram
     isError = is_error
     getFilename = get_filename
     getFile = get_file
     getFilePos = get_file_pos
 
-class FileReference(TypedReferenceCount):
-    """Keeps a reference-counted pointer to a file on disk.  As long as the
-    FileReference is held, someone presumably has a use for this file.
-    """
-
-    @overload
-    def __init__(self, __param0: ConfigVariableFilename | FileReference) -> None: ...
-    @overload
-    def __init__(self, filename: StrOrBytesPath) -> None: ...
-    def __copy__(self) -> Self: ...
-    def __deepcopy__(self, __memo: object) -> Self: ...
-    def get_filename(self) -> Filename:
-        """Returns the filename of the reference."""
-    getFilename = get_filename
-
 class TypedReferenceCount(TypedObject, ReferenceCount):  # type: ignore[misc]
     """A base class for things which need to inherit from both TypedObject and
     from ReferenceCount.  It's convenient to define this intermediate base
     class instead of multiply inheriting from the two classes each time they
     are needed, so that we can sensibly pass around pointers to things which
     are both TypedObjects and ReferenceCounters.
 
@@ -1031,14 +1020,29 @@
     """
 
     def upcast_to_TypedObject(self) -> TypedObject: ...
     def upcast_to_ReferenceCount(self) -> ReferenceCount: ...
     upcastToTypedObject = upcast_to_TypedObject
     upcastToReferenceCount = upcast_to_ReferenceCount
 
+class FileReference(TypedReferenceCount):
+    """Keeps a reference-counted pointer to a file on disk.  As long as the
+    FileReference is held, someone presumably has a use for this file.
+    """
+
+    @overload
+    def __init__(self, __param0: ConfigVariableFilename | FileReference) -> None: ...
+    @overload
+    def __init__(self, filename: StrOrBytesPath) -> None: ...
+    def __copy__(self) -> Self: ...
+    def __deepcopy__(self, __memo: object) -> Self: ...
+    def get_filename(self) -> Filename:
+        """Returns the filename of the reference."""
+    getFilename = get_filename
+
 class Ramfile:
     """An in-memory buffer specifically designed for downloading files to memory."""
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, __param0: Ramfile = ...) -> None: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
@@ -2332,16 +2336,18 @@
         unless owns_dest was true.
         """
 
 class VirtualFileList(ReferenceCount):
     """A list of VirtualFiles, as returned by VirtualFile::scan_directory()."""
 
     def __init__(self, __param0: VirtualFileList) -> None: ...
-    def __getitem__(self, n: int) -> VirtualFile: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, n: int) -> VirtualFile:
+        """Returns the nth file in the list."""
+    def __len__(self) -> int:
+        """Returns the number of files in the list."""
     def __iadd__(self, other: VirtualFileList) -> Self: ...
     def __add__(self, other: VirtualFileList) -> VirtualFileList: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[VirtualFile]: ...  # Doesn't actually exist
     def get_num_files(self) -> int:
         """Returns the number of files in the list."""
@@ -2643,14 +2649,18 @@
     openAppendFile = open_append_file
     closeWriteFile = close_write_file
     openReadWriteFile = open_read_write_file
     openReadAppendFile = open_read_append_file
     closeReadWriteFile = close_read_write_file
     getMounts = get_mounts
 
+class PointerToBase_VirtualFileMount(PointerToVoid):
+    def clear(self) -> None: ...
+    def output(self, out: ostream) -> None: ...
+
 class PointerTo_VirtualFileMount(PointerToBase_VirtualFileMount):
     @overload
     def __init__(self, copy: VirtualFileMount = ...) -> None: ...
     @overload
     def __init__(self, ptr: VirtualFileMount) -> None: ...
     @overload
     def __init__(self, __param0: None) -> None: ...
@@ -2663,18 +2673,14 @@
         double-casting, and it can be run-time checked for correctness.
         """
     @overload
     def assign(self, copy: VirtualFileMount) -> Self: ...
     @overload
     def assign(self, ptr: VirtualFileMount) -> Self: ...
 
-class PointerToBase_VirtualFileMount(PointerToVoid):
-    def clear(self) -> None: ...
-    def output(self, out: ostream) -> None: ...
-
 class TrueClock:
     """An interface to whatever real-time clock we might have available in the
     current environment.  There is only one TrueClock in existence, and it
     constructs itself.
 
     The TrueClock returns elapsed real time in seconds since some undefined
     epoch.  Since it is not defined at what time precisely the clock indicates
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_gobj.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_gobj.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4025,24 +4025,24 @@
         pipeline.  This excludes texture stages such as normal mapping and the
         like.
         """
     def set_color(self, color: Vec4Like) -> None:
         """Set the color for this stage"""
     def get_color(self) -> LColor:
         """return the color for this stage"""
-    def set_rgb_scale(self, rgb_scale: Literal[1, 2, 4]) -> None:
+    def set_rgb_scale(self, rgb_scale: int) -> None:
         """Sets an additional factor that will scale all three r, g, b components
         after the texture has been applied.  This is used only when the mode is
         CM_combine.
 
         The only legal values are 1, 2, or 4.
         """
     def get_rgb_scale(self) -> int:
         """See set_rgb_scale()."""
-    def set_alpha_scale(self, alpha_scale: Literal[1, 2, 4]) -> None:
+    def set_alpha_scale(self, alpha_scale: int) -> None:
         """Sets an additional factor that will scale the alpha component after the
         texture has been applied.  This is used only when the mode is CM_combine.
 
         The only legal values are 1, 2, or 4.
         """
     def get_alpha_scale(self) -> int:
         """See set_alpha_scale()."""
@@ -6624,15 +6624,15 @@
         this, its contents may be undefined (or may in fact not be cleared at all).
         """
     def get_clear_data(self) -> bytes:
         """Returns the raw image data for a single pixel if it were set to the clear
         color.
         """
     @overload
-    def read(self, fullpath: StrOrBytesPath, options: LoaderOptions | int = ...) -> bool:
+    def read(self, fullpath: StrOrBytesPath, options: LoaderOptions = ...) -> bool:
         """`(self, fullpath: Filename, alpha_fullpath: Filename, primary_file_num_channels: int, alpha_file_channel: int, options: LoaderOptions = ...)`:
         Combine a 3-component image with a grayscale image to get a 4-component
         image.
 
         See the description of the full-parameter read() method for the meaning of
         the primary_file_num_channels and alpha_file_channel parameters.
 
@@ -6701,33 +6701,33 @@
     @overload
     def read(
         self,
         fullpath: StrOrBytesPath,
         alpha_fullpath: StrOrBytesPath,
         primary_file_num_channels: int,
         alpha_file_channel: int,
-        options: LoaderOptions | int = ...,
+        options: LoaderOptions = ...,
     ) -> bool: ...
     @overload
     def read(
-        self, fullpath: StrOrBytesPath, z: int, n: int, read_pages: bool, read_mipmaps: bool, options: LoaderOptions | int = ...
+        self, fullpath: StrOrBytesPath, z: int, n: int, read_pages: bool, read_mipmaps: bool, options: LoaderOptions = ...
     ) -> bool: ...
     @overload
     def read(
         self,
         fullpath: StrOrBytesPath,
         alpha_fullpath: StrOrBytesPath,
         primary_file_num_channels: int,
         alpha_file_channel: int,
         z: int,
         n: int,
         read_pages: bool,
         read_mipmaps: bool,
         record: BamCacheRecord = ...,
-        options: LoaderOptions | int = ...,
+        options: LoaderOptions = ...,
     ) -> bool: ...
     @overload
     def write(self, fullpath: StrOrBytesPath) -> bool:
         """`(self, fullpath: Filename)`:
         Writes the texture to the named filename.
 
         `(self, fullpath: Filename, z: int, n: int, write_pages: bool, write_mipmaps: bool)`:
@@ -6817,27 +6817,27 @@
         to contain the texture image in a form as similar as possible to its
         runtime image, and it can contain mipmaps, pre-compressed textures, and so
         on.
 
         As with read_dds, the filename is just for reference.
         """
     @overload
-    def load(self, pnmimage: PNMImage, options: LoaderOptions | int = ...) -> bool:
+    def load(self, pnmimage: PNMImage, options: LoaderOptions = ...) -> bool:
         """`(self, pnmimage: PNMImage, options: LoaderOptions = ...)`; `(self, pfm: PfmFile, options: LoaderOptions = ...)`:
         Replaces the texture with the indicated image.
 
         `(self, pnmimage: PNMImage, z: int, n: int, options: LoaderOptions = ...)`; `(self, pfm: PfmFile, z: int, n: int, options: LoaderOptions = ...)`:
         Stores the indicated image in the given page and mipmap level.  See read().
         """
     @overload
-    def load(self, pfm: PfmFile, options: LoaderOptions | int = ...) -> bool: ...
+    def load(self, pfm: PfmFile, options: LoaderOptions = ...) -> bool: ...
     @overload
-    def load(self, pnmimage: PNMImage, z: int, n: int, options: LoaderOptions | int = ...) -> bool: ...
+    def load(self, pnmimage: PNMImage, z: int, n: int, options: LoaderOptions = ...) -> bool: ...
     @overload
-    def load(self, pfm: PfmFile, z: int, n: int, options: LoaderOptions | int = ...) -> bool: ...
+    def load(self, pfm: PfmFile, z: int, n: int, options: LoaderOptions = ...) -> bool: ...
     def load_sub_image(self, pnmimage: PNMImage, x: int, y: int, z: int = ..., n: int = ...) -> bool:
         """Stores the indicated image in a region of the texture.  The texture
         properties remain unchanged.  This can be more efficient than updating an
         entire texture, but has a few restrictions: for one, you must ensure that
         the texture is still in RAM (eg.  using set_keep_ram_image) and it may not
         be compressed.
         """
@@ -10104,16 +10104,22 @@
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     @overload
     def __init__(self, copy: TextureCollection = ...) -> None: ...
     @overload
     def __init__(self, sequence) -> None: ...
-    def __getitem__(self, index: int) -> Texture: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> Texture:
+        """Returns the nth Texture in the collection.  This is the same as
+        get_texture(), but it may be a more convenient way to access it.
+        """
+    def __len__(self) -> int:
+        """Returns the number of textures in the collection.  This is the same thing
+        as get_num_textures().
+        """
     def __iadd__(self, other: TextureCollection) -> Self: ...
     def __add__(self, other: TextureCollection) -> TextureCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[Texture]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_texture(self, texture: Texture) -> None:
@@ -10214,18 +10220,15 @@
         primary_file_num_channels: int = ...,
         alpha_file_channel: int = ...,
         read_mipmaps: bool = ...,
     ) -> Texture: ...
     @overload
     @staticmethod
     def load_texture(
-        filename: StrOrBytesPath,
-        primary_file_num_channels: int = ...,
-        read_mipmaps: bool = ...,
-        options: LoaderOptions | int = ...,
+        filename: StrOrBytesPath, primary_file_num_channels: int = ..., read_mipmaps: bool = ..., options: LoaderOptions = ...
     ) -> Texture:
         """`(filename: Filename, alpha_filename: Filename, primary_file_num_channels: int = ..., alpha_file_channel: int = ..., read_mipmaps: bool = ..., options: LoaderOptions = ...)`:
         Loads the given filename up into a texture, if it has not already been
         loaded, and returns the new texture.  If a texture with the same filename
         was previously loaded, returns that one instead.  If the texture file
         cannot be found, returns NULL.
 
@@ -10247,44 +10250,42 @@
     @staticmethod
     def load_texture(
         filename: StrOrBytesPath,
         alpha_filename: StrOrBytesPath,
         primary_file_num_channels: int = ...,
         alpha_file_channel: int = ...,
         read_mipmaps: bool = ...,
-        options: LoaderOptions | int = ...,
+        options: LoaderOptions = ...,
     ) -> Texture: ...
     @staticmethod
-    def load_3d_texture(
-        filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions | int = ...
-    ) -> Texture:
+    def load_3d_texture(filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions = ...) -> Texture:
         """Loads a 3-D texture that is specified with a series of n pages, all
         numbered in sequence, and beginning with index 0.  The filename should
         include a sequence of one or more hash characters ("#") which will be
         filled in with the index number of each level.
 
         If read_mipmaps is true, the filename should contain an additional hash
         mark.  The first hash mark will be filled in with the mipmap level number,
         and the second with the index number of each 3-d level.
         """
     @staticmethod
     def load_2d_texture_array(
-        filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions | int = ...
+        filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions = ...
     ) -> Texture:
         """Loads a 2-D texture array that is specified with a series of n pages, all
         numbered in sequence, and beginning with index 0.  The filename should
         include a sequence of one or more hash characters ("#") which will be
         filled in with the index number of each level.
 
         If read_mipmaps is true, the filename should contain an additional hash
         mark.  The first hash mark will be filled in with the mipmap level number,
         and the second with the index number of each 2-d level.
         """
     @staticmethod
-    def load_cube_map(filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions | int = ...) -> Texture:
+    def load_cube_map(filename_pattern: StrOrBytesPath, read_mipmaps: bool = ..., options: LoaderOptions = ...) -> Texture:
         """Loads a cube map texture that is specified with a series of 6 pages,
         numbered 0 through 5.  The filename should include a sequence of one or
         more hash characters ("#") which will be filled in with the index number of
         each pagee.
 
         If read_mipmaps is true, the filename should contain an additional hash
         mark.  The first hash mark will be filled in with the mipmap level number,
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_grutil.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_grutil.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from panda3d.core._audio import AudioSound
 from panda3d.core._display import DisplayRegion, GraphicsOutput
 from panda3d.core._dtoolbase import TypedObject
 from panda3d.core._express import Namable
 from panda3d.core._gobj import InternalName, Lens, Texture, TextureStage, VertexTransform
 from panda3d.core._linmath import LColor, LPoint3, LVecBase2, LVector3, LVertex
 from panda3d.core._movies import MovieVideo, MovieVideoCursor
-from panda3d.core._pgraph import CullTraverser, GeomNode, NodePath, PandaNode, RenderAttrib, RenderState, TransformState
+from panda3d.core._pgraph import CullTraverser, GeomNode, NodePath, PandaNode, RenderState, TransformState
 from panda3d.core._pnmimage import PfmFile, PNMFileType, PNMImage
 from panda3d.core._putil import ClockObject, DrawMask
 from panda3d.core._text import TextNode
 
 _ClockObject_Mode: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7]
 _PfmVizzer_ColumnType: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
 _PfmVizzer_MeshFace: TypeAlias = Literal[1, 2, 3]
@@ -1035,15 +1035,15 @@
         some other node here in order to not consider nodes above that as
         contributing to the state to be flattened.  This is particularly useful if
         you have some texture stage which is applied globally to a scene (for
         instance, a caustics effect), which you don't want to be considered for
         flattening by the MultitexReducer.
         """
     @overload
-    def scan(self, node: PandaNode, state: RenderAttrib | RenderState, transform: TransformState) -> None: ...
+    def scan(self, node: PandaNode, state: RenderState, transform: TransformState) -> None: ...
     def set_target(self, stage: TextureStage) -> None: ...
     def set_use_geom(self, use_geom: bool) -> None: ...
     def set_allow_tex_mat(self, allow_tex_mat: bool) -> None: ...
     def flatten(self, window: GraphicsOutput) -> None: ...
     setTarget = set_target
     setUseGeom = set_use_geom
     setAllowTexMat = set_allow_tex_mat
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_gsgbase.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_gsgbase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_linmath.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_linmath.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def __init__(self, __param0: Vec2Like = ...) -> None: ...
     @overload
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[2]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: Vec2Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: Vec2Like) -> LVecBase2f: ...
     def __sub__(self, other: Vec2Like) -> LVecBase2f: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -94,15 +94,15 @@
         """These next functions add to an existing value.  i.e.
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[2]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float) -> None: ...
     def dot(self, other: Vec2Like) -> float: ...
     def length_squared(self) -> float:
@@ -208,15 +208,15 @@
     def __init__(self, __param0: DoubleVec2Like = ...) -> None: ...
     @overload
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[2]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: DoubleVec2Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: DoubleVec2Like) -> LVecBase2d: ...
     def __sub__(self, other: DoubleVec2Like) -> LVecBase2d: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -262,15 +262,15 @@
         """These next functions add to an existing value.  i.e.
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[2]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float) -> None: ...
     def dot(self, other: DoubleVec2Like) -> float: ...
     def length_squared(self) -> float:
@@ -376,15 +376,15 @@
     def __init__(self, __param0: IntVec2Like = ...) -> None: ...
     @overload
     def __init__(self, fill_value: int) -> None: ...
     @overload
     def __init__(self, x: int, y: int) -> None: ...
     def __getitem__(self, i: int) -> int: ...
     def __setitem__(self, i: int, assign_val: int) -> None: ...
-    def __len__(self) -> Literal[2]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: IntVec2Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: IntVec2Like) -> LVecBase2i: ...
     def __sub__(self, other: IntVec2Like) -> LVecBase2i: ...
     def __mul__(self, scalar: int) -> Self: ...
@@ -428,15 +428,15 @@
         """These next functions add to an existing value.  i.e.
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: int) -> None: ...
     def add_y(self, value: int) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[2]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: int) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: int, y: int) -> None: ...
     def dot(self, other: IntVec2Like) -> int: ...
     def length_squared(self) -> int:
@@ -776,15 +776,15 @@
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, copy: Vec2Like, z: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: Vec3Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: Vec3Like) -> LVecBase3f: ...
     def __sub__(self, other: Vec3Like) -> LVecBase3f: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -848,15 +848,15 @@
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     def add_z(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[3]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float) -> None: ...
     def dot(self, other: Vec3Like) -> float: ...
     def length_squared(self) -> float:
@@ -994,15 +994,15 @@
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, copy: DoubleVec2Like, z: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: DoubleVec3Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: DoubleVec3Like) -> LVecBase3d: ...
     def __sub__(self, other: DoubleVec3Like) -> LVecBase3d: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -1066,15 +1066,15 @@
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     def add_z(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[3]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float) -> None: ...
     def dot(self, other: DoubleVec3Like) -> float: ...
     def length_squared(self) -> float:
@@ -1212,15 +1212,15 @@
     def __init__(self, fill_value: int) -> None: ...
     @overload
     def __init__(self, copy: IntVec2Like, z: int) -> None: ...
     @overload
     def __init__(self, x: int, y: int, z: int) -> None: ...
     def __getitem__(self, i: int) -> int: ...
     def __setitem__(self, i: int, assign_val: int) -> None: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: IntVec3Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: IntVec3Like) -> LVecBase3i: ...
     def __sub__(self, other: IntVec3Like) -> LVecBase3i: ...
     def __mul__(self, scalar: int) -> Self: ...
@@ -1282,15 +1282,15 @@
         foo.set_x(foo.get_x() + value) These are useful to reduce overhead in
         scripting languages:
         """
     def add_x(self, value: int) -> None: ...
     def add_y(self, value: int) -> None: ...
     def add_z(self, value: int) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[3]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: int) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: int, y: int, z: int) -> None: ...
     def dot(self, other: IntVec3Like) -> int: ...
     def length_squared(self) -> int:
@@ -1947,15 +1947,15 @@
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, copy: Vec3Like, w: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float, w: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: Vec4Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: Vec4Like) -> LVecBase4f: ...
     def __sub__(self, other: Vec4Like) -> LVecBase4f: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -2017,15 +2017,15 @@
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     def add_z(self, value: float) -> None: ...
     def add_w(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float, w: float) -> None: ...
     def dot(self, other: Vec4Like) -> float: ...
     def length_squared(self) -> float:
@@ -2148,27 +2148,27 @@
     def __init__(self, __param0: UnalignedLVecBase4f | Vec4Like) -> None: ...
     @overload
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float, w: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float, w: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     @staticmethod
     def get_class_type() -> TypeHandle: ...
     getNumComponents = get_num_components
     getClassType = get_class_type
 
 class LVecBase4d:
     """This is the base class for all three-component vectors and points."""
@@ -2199,15 +2199,15 @@
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, copy: DoubleVec3Like, w: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float, w: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: DoubleVec4Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: DoubleVec4Like) -> LVecBase4d: ...
     def __sub__(self, other: DoubleVec4Like) -> LVecBase4d: ...
     def __mul__(self, scalar: float) -> Self: ...
@@ -2269,15 +2269,15 @@
         scripting languages:
         """
     def add_x(self, value: float) -> None: ...
     def add_y(self, value: float) -> None: ...
     def add_z(self, value: float) -> None: ...
     def add_w(self, value: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float, w: float) -> None: ...
     def dot(self, other: DoubleVec4Like) -> float: ...
     def length_squared(self) -> float:
@@ -2400,27 +2400,27 @@
     def __init__(self, __param0: DoubleVec4Like | UnalignedLVecBase4d) -> None: ...
     @overload
     def __init__(self, fill_value: float) -> None: ...
     @overload
     def __init__(self, x: float, y: float, z: float, w: float) -> None: ...
     def __getitem__(self, i: int) -> float: ...
     def __setitem__(self, i: int, assign_val: float) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
     def fill(self, fill_value: float) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: float, y: float, z: float, w: float) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     @staticmethod
     def get_class_type() -> TypeHandle: ...
     getNumComponents = get_num_components
     getClassType = get_class_type
 
 class LVecBase4i:
     """This is the base class for all three-component vectors and points."""
@@ -2451,15 +2451,15 @@
     def __init__(self, fill_value: int) -> None: ...
     @overload
     def __init__(self, copy: IntVec3Like, w: int) -> None: ...
     @overload
     def __init__(self, x: int, y: int, z: int, w: int) -> None: ...
     def __getitem__(self, i: int) -> int: ...
     def __setitem__(self, i: int, assign_val: int) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __lt__(self, other: IntVec4Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __neg__(self) -> Self: ...
     def __add__(self, other: IntVec4Like) -> LVecBase4i: ...
     def __sub__(self, other: IntVec4Like) -> LVecBase4i: ...
     def __mul__(self, scalar: int) -> Self: ...
@@ -2519,15 +2519,15 @@
         scripting languages:
         """
     def add_x(self, value: int) -> None: ...
     def add_y(self, value: int) -> None: ...
     def add_z(self, value: int) -> None: ...
     def add_w(self, value: int) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     def fill(self, fill_value: int) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: int, y: int, z: int, w: int) -> None: ...
     def dot(self, other: IntVec4Like) -> int: ...
     def length_squared(self) -> int:
@@ -2630,27 +2630,27 @@
     def __init__(self, __param0: UnalignedLVecBase4i | tuple[int, int, int, int]) -> None: ...
     @overload
     def __init__(self, fill_value: int) -> None: ...
     @overload
     def __init__(self, x: int, y: int, z: int, w: int) -> None: ...
     def __getitem__(self, i: int) -> int: ...
     def __setitem__(self, i: int, assign_val: int) -> None: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
     def fill(self, fill_value: int) -> None:
         """Sets each element of the vector to the indicated fill_value.  This is
         particularly useful for initializing to zero.
         """
     def set(self, x: int, y: int, z: int, w: int) -> None: ...
     @staticmethod
-    def get_num_components() -> Literal[4]: ...
+    def get_num_components() -> int: ...
     @staticmethod
     def get_class_type() -> TypeHandle: ...
     getNumComponents = get_num_components
     getClassType = get_class_type
 
 class LVector4f(LVecBase4f):
     """This is a four-component vector distance."""
@@ -2961,31 +2961,34 @@
     class Row:
         """These helper classes are used to support two-level operator []."""
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix3f.Row) -> None: ...
         def __getitem__(self, i: int) -> float: ...
         def __setitem__(self, i: int, assign_val: float) -> None: ...
-        def __len__(self) -> Literal[3]: ...
+        def __len__(self) -> int:
+            """Returns 3: the number of columns of a LMatrix3."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase3f: ...
         operatorTypecast = operator_typecast
 
     class CRow:
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix3f.CRow) -> None: ...
         def __getitem__(self, i: int) -> float: ...
-        def __len__(self) -> Literal[3]: ...
+        def __len__(self) -> int:
+            """Returns 3: the number of columns of a LMatrix3."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase3f: ...
         operatorTypecast = operator_typecast
+
     num_components: Final = 9
     is_int: Final = 0
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def rows(self) -> MutableSequence[LVecBase3f]: ...
     @property
     def cols(self) -> MutableSequence[LVecBase3f]: ...
@@ -3004,31 +3007,36 @@
         __param4: float,
         __param5: float,
         __param6: float,
         __param7: float,
         __param8: float,
     ) -> None: ...
     def __getitem__(self, i: int) -> LMatrix3f.CRow | LMatrix3f.Row: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int:
+        """Returns 3: the number of rows of a LMatrix3."""
     def __call__(self, row: int, col: int) -> float | None: ...
     def __lt__(self, other: LMatrix3f) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     @overload
     def __mul__(self, other: LMatrix3f) -> LMatrix3f: ...
     @overload
     def __mul__(self, scalar: float) -> LMatrix3f: ...
     def __truediv__(self, scalar: float) -> LMatrix3f: ...
-    def __iadd__(self, other: LMatrix3f) -> Self: ...
-    def __isub__(self, other: LMatrix3f) -> Self: ...
+    def __iadd__(self, other: LMatrix3f) -> Self:
+        """Performs a memberwise addition between two matrices."""
+    def __isub__(self, other: LMatrix3f) -> Self:
+        """Performs a memberwise subtraction between two matrices."""
     @overload
-    def __imul__(self, other: LMatrix3f) -> Self: ...
+    def __imul__(self, other: LMatrix3f) -> Self:
+        """Performs a memberwise scale."""
     @overload
     def __imul__(self, scalar: float) -> Self: ...
-    def __itruediv__(self, scalar: float) -> Self: ...
+    def __itruediv__(self, scalar: float) -> Self:
+        """Performs a memberwise scale."""
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[LMatrix3f.CRow | LMatrix3f.Row]: ...  # Doesn't actually exist
     @overload
     def assign(self, other: LMatrix3f) -> Self: ...
     @overload
     def assign(self, fill_value: float) -> Self: ...
@@ -3371,31 +3379,34 @@
     class Row:
         """These helper classes are used to support two-level operator []."""
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix4f.Row) -> None: ...
         def __getitem__(self, i: int) -> float: ...
         def __setitem__(self, i: int, assign_val: float) -> None: ...
-        def __len__(self) -> Literal[4]: ...
+        def __len__(self) -> int:
+            """Returns 4: the number of columns of a LMatrix4."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase4f: ...
         operatorTypecast = operator_typecast
 
     class CRow:
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix4f.CRow) -> None: ...
         def __getitem__(self, i: int) -> float: ...
-        def __len__(self) -> Literal[4]: ...
+        def __len__(self) -> int:
+            """Returns 4: the number of columns of a LMatrix4."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase4f: ...
         operatorTypecast = operator_typecast
+
     num_components: Final = 16
     is_int: Final = 0
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def rows(self) -> MutableSequence[LVecBase4f]: ...
     @property
     def cols(self) -> MutableSequence[LVecBase4f]: ...
@@ -3431,26 +3442,29 @@
         __param11: float,
         __param12: float,
         __param13: float,
         __param14: float,
         __param15: float,
     ) -> None: ...
     def __getitem__(self, i: int) -> LMatrix4f.CRow | LMatrix4f.Row: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int:
+        """Returns 4: the number of rows of a LMatrix4."""
     def __call__(self, row: int, col: int) -> float | None: ...
     def __lt__(self, other: Mat4Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     @overload
     def __mul__(self, other: Mat4Like) -> LMatrix4f: ...
     @overload
     def __mul__(self, scalar: float) -> LMatrix4f: ...
     def __truediv__(self, scalar: float) -> LMatrix4f: ...
-    def __iadd__(self, other: Mat4Like) -> Self: ...
-    def __isub__(self, other: Mat4Like) -> Self: ...
+    def __iadd__(self, other: Mat4Like) -> Self:
+        """Performs a memberwise addition between two matrices."""
+    def __isub__(self, other: Mat4Like) -> Self:
+        """Performs a memberwise subtraction between two matrices."""
     @overload
     def __imul__(self, other: Mat4Like) -> Self: ...
     @overload
     def __imul__(self, scalar: float) -> Self: ...
     def __itruediv__(self, scalar: float) -> Self: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
@@ -3891,31 +3905,34 @@
     class Row:
         """These helper classes are used to support two-level operator []."""
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix3d.Row) -> None: ...
         def __getitem__(self, i: int) -> float: ...
         def __setitem__(self, i: int, assign_val: float) -> None: ...
-        def __len__(self) -> Literal[3]: ...
+        def __len__(self) -> int:
+            """Returns 3: the number of columns of a LMatrix3."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase3d: ...
         operatorTypecast = operator_typecast
 
     class CRow:
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix3d.CRow) -> None: ...
         def __getitem__(self, i: int) -> float: ...
-        def __len__(self) -> Literal[3]: ...
+        def __len__(self) -> int:
+            """Returns 3: the number of columns of a LMatrix3."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase3d: ...
         operatorTypecast = operator_typecast
+
     num_components: Final = 9
     is_int: Final = 0
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def rows(self) -> MutableSequence[LVecBase3d]: ...
     @property
     def cols(self) -> MutableSequence[LVecBase3d]: ...
@@ -3934,31 +3951,36 @@
         __param4: float,
         __param5: float,
         __param6: float,
         __param7: float,
         __param8: float,
     ) -> None: ...
     def __getitem__(self, i: int) -> LMatrix3d.CRow | LMatrix3d.Row: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int:
+        """Returns 3: the number of rows of a LMatrix3."""
     def __call__(self, row: int, col: int) -> float | None: ...
     def __lt__(self, other: LMatrix3d) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     @overload
     def __mul__(self, other: LMatrix3d) -> LMatrix3d: ...
     @overload
     def __mul__(self, scalar: float) -> LMatrix3d: ...
     def __truediv__(self, scalar: float) -> LMatrix3d: ...
-    def __iadd__(self, other: LMatrix3d) -> Self: ...
-    def __isub__(self, other: LMatrix3d) -> Self: ...
+    def __iadd__(self, other: LMatrix3d) -> Self:
+        """Performs a memberwise addition between two matrices."""
+    def __isub__(self, other: LMatrix3d) -> Self:
+        """Performs a memberwise subtraction between two matrices."""
     @overload
-    def __imul__(self, other: LMatrix3d) -> Self: ...
+    def __imul__(self, other: LMatrix3d) -> Self:
+        """Performs a memberwise scale."""
     @overload
     def __imul__(self, scalar: float) -> Self: ...
-    def __itruediv__(self, scalar: float) -> Self: ...
+    def __itruediv__(self, scalar: float) -> Self:
+        """Performs a memberwise scale."""
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[LMatrix3d.CRow | LMatrix3d.Row]: ...  # Doesn't actually exist
     @overload
     def assign(self, other: LMatrix3d) -> Self: ...
     @overload
     def assign(self, fill_value: float) -> Self: ...
@@ -4301,31 +4323,34 @@
     class Row:
         """These helper classes are used to support two-level operator []."""
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix4d.Row) -> None: ...
         def __getitem__(self, i: int) -> float: ...
         def __setitem__(self, i: int, assign_val: float) -> None: ...
-        def __len__(self) -> Literal[4]: ...
+        def __len__(self) -> int:
+            """Returns 4: the number of columns of a LMatrix4."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase4d: ...
         operatorTypecast = operator_typecast
 
     class CRow:
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: LMatrix4d.CRow) -> None: ...
         def __getitem__(self, i: int) -> float: ...
-        def __len__(self) -> Literal[4]: ...
+        def __len__(self) -> int:
+            """Returns 4: the number of columns of a LMatrix4."""
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
         def operator_typecast(self) -> LVecBase4d: ...
         operatorTypecast = operator_typecast
+
     num_components: Final = 16
     is_int: Final = 0
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def rows(self) -> MutableSequence[LVecBase4d]: ...
     @property
     def cols(self) -> MutableSequence[LVecBase4d]: ...
@@ -4363,26 +4388,29 @@
         __param11: float,
         __param12: float,
         __param13: float,
         __param14: float,
         __param15: float,
     ) -> None: ...
     def __getitem__(self, i: int) -> LMatrix4d.CRow | LMatrix4d.Row: ...
-    def __len__(self) -> Literal[4]: ...
+    def __len__(self) -> int:
+        """Returns 4: the number of rows of a LMatrix4."""
     def __call__(self, row: int, col: int) -> float | None: ...
     def __lt__(self, other: DoubleMat4Like) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     @overload
     def __mul__(self, other: DoubleMat4Like) -> LMatrix4d: ...
     @overload
     def __mul__(self, scalar: float) -> LMatrix4d: ...
     def __truediv__(self, scalar: float) -> LMatrix4d: ...
-    def __iadd__(self, other: DoubleMat4Like) -> Self: ...
-    def __isub__(self, other: DoubleMat4Like) -> Self: ...
+    def __iadd__(self, other: DoubleMat4Like) -> Self:
+        """Performs a memberwise addition between two matrices."""
+    def __isub__(self, other: DoubleMat4Like) -> Self:
+        """Performs a memberwise subtraction between two matrices."""
     @overload
     def __imul__(self, other: DoubleMat4Like) -> Self: ...
     @overload
     def __imul__(self, scalar: float) -> Self: ...
     def __itruediv__(self, scalar: float) -> Self: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
@@ -4832,15 +4860,18 @@
     def __mul__(self, __param0: LMatrix4f | UnalignedLMatrix4f) -> LMatrix4f: ...
     @overload
     def __mul__(self, __param0: Vec4Like) -> LQuaternionf: ...
     @overload
     def __mul__(self, scalar: float) -> LQuaternionf: ...
     def __truediv__(self, scalar: float) -> LQuaternionf: ...
     def __imul__(self, __param0: Vec4Like) -> Self: ...  # type: ignore[misc, override]
-    def __pow__(self, __param0: float) -> LQuaternionf: ...
+    def __pow__(self, __param0: float) -> LQuaternionf:
+        """Returns a new quaternion that represents this quaternion raised to the
+        given power.
+        """
     @staticmethod
     def pure_imaginary(v: Vec3Like) -> LQuaternionf: ...
     def conjugate(self) -> LQuaternionf:
         """Returns the complex conjugate of this quat."""
     @overload
     def xform(self, v: Vec3Like) -> LVecBase3f:
         """`(self, v: LVecBase3f)`:
@@ -5036,15 +5067,18 @@
     def __mul__(self, __param0: LMatrix4d | UnalignedLMatrix4d) -> LMatrix4d: ...
     @overload
     def __mul__(self, __param0: DoubleVec4Like) -> LQuaterniond: ...
     @overload
     def __mul__(self, scalar: float) -> LQuaterniond: ...
     def __truediv__(self, scalar: float) -> LQuaterniond: ...
     def __imul__(self, __param0: DoubleVec4Like) -> Self: ...  # type: ignore[misc, override]
-    def __pow__(self, __param0: float) -> LQuaterniond: ...
+    def __pow__(self, __param0: float) -> LQuaterniond:
+        """Returns a new quaternion that represents this quaternion raised to the
+        given power.
+        """
     @staticmethod
     def pure_imaginary(v: DoubleVec3Like) -> LQuaterniond: ...
     def conjugate(self) -> LQuaterniond:
         """Returns the complex conjugate of this quat."""
     @overload
     def xform(self, v: DoubleVec3Like) -> LVecBase3d:
         """`(self, v: LVecBase3d)`:
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_mathutil.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_mathutil.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,23 @@
     UnalignedLVecBase4d,
     UnalignedLVecBase4f,
     UnalignedLVecBase4i,
 )
 
 _CoordinateSystem: TypeAlias = Literal[0, 1, 2, 3, 4, 5]
 
+class PointerToBase_ReferenceCountedVector_LMatrix3d(PointerToVoid):
+    def clear(self) -> None: ...
+    def output(self, out: ostream) -> None: ...
+
+class PointerToArrayBase_LMatrix3d(PointerToBase_ReferenceCountedVector_LMatrix3d):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LMatrix3d(PointerToArrayBase_LMatrix3d):
     def __init__(self, copy: ConstPointerToArray_LMatrix3d | PointerToArray_LMatrix3d) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LMatrix3d: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LMatrix3d: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LMatrix3d]: ...  # Doesn't actually exist
@@ -61,22 +70,23 @@
     def count(self, __param0: LMatrix3d) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LMatrix3d(PointerToBase_ReferenceCountedVector_LMatrix3d):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LMatrix3d(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LMatrix3f(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LMatrix3f(PointerToBase_ReferenceCountedVector_LMatrix3f):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LMatrix3f(PointerToArrayBase_LMatrix3f):
     def __init__(self, copy: ConstPointerToArray_LMatrix3f | PointerToArray_LMatrix3f) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LMatrix3f: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LMatrix3f: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LMatrix3f]: ...  # Doesn't actually exist
@@ -88,22 +98,23 @@
     def count(self, __param0: LMatrix3f) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LMatrix3f(PointerToBase_ReferenceCountedVector_LMatrix3f):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LMatrix3f(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase2d(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase2d(PointerToBase_ReferenceCountedVector_LVecBase2d):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase2d(PointerToArrayBase_LVecBase2d):
     def __init__(self, copy: ConstPointerToArray_LVecBase2d | PointerToArray_LVecBase2d) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase2d: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase2d: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase2d]: ...  # Doesn't actually exist
@@ -115,22 +126,23 @@
     def count(self, __param0: DoubleVec2Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase2d(PointerToBase_ReferenceCountedVector_LVecBase2d):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase2d(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase2f(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase2f(PointerToBase_ReferenceCountedVector_LVecBase2f):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase2f(PointerToArrayBase_LVecBase2f):
     def __init__(self, copy: ConstPointerToArray_LVecBase2f | PointerToArray_LVecBase2f) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase2f: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase2f: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase2f]: ...  # Doesn't actually exist
@@ -142,22 +154,23 @@
     def count(self, __param0: Vec2Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase2f(PointerToBase_ReferenceCountedVector_LVecBase2f):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase2f(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase2i(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase2i(PointerToBase_ReferenceCountedVector_LVecBase2i):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase2i(PointerToArrayBase_LVecBase2i):
     def __init__(self, copy: ConstPointerToArray_LVecBase2i | PointerToArray_LVecBase2i) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase2i: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase2i: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase2i]: ...  # Doesn't actually exist
@@ -169,22 +182,23 @@
     def count(self, __param0: IntVec2Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase2i(PointerToBase_ReferenceCountedVector_LVecBase2i):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase2i(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase3d(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase3d(PointerToBase_ReferenceCountedVector_LVecBase3d):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase3d(PointerToArrayBase_LVecBase3d):
     def __init__(self, copy: ConstPointerToArray_LVecBase3d | PointerToArray_LVecBase3d) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase3d: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase3d: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase3d]: ...  # Doesn't actually exist
@@ -196,22 +210,23 @@
     def count(self, __param0: DoubleVec3Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase3d(PointerToBase_ReferenceCountedVector_LVecBase3d):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase3d(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase3f(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase3f(PointerToBase_ReferenceCountedVector_LVecBase3f):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase3f(PointerToArrayBase_LVecBase3f):
     def __init__(self, copy: ConstPointerToArray_LVecBase3f | PointerToArray_LVecBase3f) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase3f: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase3f: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase3f]: ...  # Doesn't actually exist
@@ -223,22 +238,23 @@
     def count(self, __param0: Vec3Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase3f(PointerToBase_ReferenceCountedVector_LVecBase3f):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase3f(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_LVecBase3i(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_LVecBase3i(PointerToBase_ReferenceCountedVector_LVecBase3i):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_LVecBase3i(PointerToArrayBase_LVecBase3i):
     def __init__(self, copy: ConstPointerToArray_LVecBase3i | PointerToArray_LVecBase3i) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> LVecBase3i: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_LVecBase3i: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[LVecBase3i]: ...  # Doesn't actually exist
@@ -250,22 +266,23 @@
     def count(self, __param0: IntVec3Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_LVecBase3i(PointerToBase_ReferenceCountedVector_LVecBase3i):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_LVecBase3i(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_UnalignedLMatrix4d(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_UnalignedLMatrix4d(PointerToBase_ReferenceCountedVector_UnalignedLMatrix4d):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_UnalignedLMatrix4d(PointerToArrayBase_UnalignedLMatrix4d):
     def __init__(self, copy: ConstPointerToArray_UnalignedLMatrix4d | PointerToArray_UnalignedLMatrix4d) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> UnalignedLMatrix4d: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_UnalignedLMatrix4d: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[UnalignedLMatrix4d]: ...  # Doesn't actually exist
@@ -277,22 +294,23 @@
     def count(self, __param0: LMatrix4d | UnalignedLMatrix4d) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_UnalignedLMatrix4d(PointerToBase_ReferenceCountedVector_UnalignedLMatrix4d):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_UnalignedLMatrix4d(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_UnalignedLMatrix4f(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_UnalignedLMatrix4f(PointerToBase_ReferenceCountedVector_UnalignedLMatrix4f):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_UnalignedLMatrix4f(PointerToArrayBase_UnalignedLMatrix4f):
     def __init__(self, copy: ConstPointerToArray_UnalignedLMatrix4f | PointerToArray_UnalignedLMatrix4f) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> UnalignedLMatrix4f: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_UnalignedLMatrix4f: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[UnalignedLMatrix4f]: ...  # Doesn't actually exist
@@ -304,22 +322,23 @@
     def count(self, __param0: LMatrix4f | UnalignedLMatrix4f) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_UnalignedLMatrix4f(PointerToBase_ReferenceCountedVector_UnalignedLMatrix4f):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_UnalignedLMatrix4f(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4d(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_UnalignedLVecBase4d(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4d):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_UnalignedLVecBase4d(PointerToArrayBase_UnalignedLVecBase4d):
     def __init__(self, copy: ConstPointerToArray_UnalignedLVecBase4d | PointerToArray_UnalignedLVecBase4d) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> UnalignedLVecBase4d: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_UnalignedLVecBase4d: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[UnalignedLVecBase4d]: ...  # Doesn't actually exist
@@ -331,22 +350,23 @@
     def count(self, __param0: DoubleVec4Like | UnalignedLVecBase4d) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_UnalignedLVecBase4d(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4d):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4d(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4f(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_UnalignedLVecBase4f(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4f):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_UnalignedLVecBase4f(PointerToArrayBase_UnalignedLVecBase4f):
     def __init__(self, copy: ConstPointerToArray_UnalignedLVecBase4f | PointerToArray_UnalignedLVecBase4f) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> UnalignedLVecBase4f: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_UnalignedLVecBase4f: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[UnalignedLVecBase4f]: ...  # Doesn't actually exist
@@ -358,22 +378,23 @@
     def count(self, __param0: UnalignedLVecBase4f | Vec4Like) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_UnalignedLVecBase4f(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4f):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4f(PointerToVoid):
+class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4i(PointerToVoid):
     def clear(self) -> None: ...
     def output(self, out: ostream) -> None: ...
 
+class PointerToArrayBase_UnalignedLVecBase4i(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4i):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_UnalignedLVecBase4i(PointerToArrayBase_UnalignedLVecBase4i):
     def __init__(self, copy: ConstPointerToArray_UnalignedLVecBase4i | PointerToArray_UnalignedLVecBase4i) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> UnalignedLVecBase4i: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_UnalignedLVecBase4i: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[UnalignedLVecBase4i]: ...  # Doesn't actually exist
@@ -385,22 +406,14 @@
     def count(self, __param0: IntVec4Like | UnalignedLVecBase4i) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_UnalignedLVecBase4i(PointerToBase_ReferenceCountedVector_UnalignedLVecBase4i):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_UnalignedLVecBase4i(PointerToVoid):
-    def clear(self) -> None: ...
-    def output(self, out: ostream) -> None: ...
-
 class PointerToArray_LMatrix3d(PointerToArrayBase_LMatrix3d):
     @overload
     def __init__(self, type_handle: TypeHandle | type = ...) -> None: ...
     @overload
     def __init__(self, copy: PointerToArray_LMatrix3d) -> None: ...
     @overload
     def __init__(self, source: Sequence[LMatrix3d]) -> None: ...
@@ -1338,19 +1351,19 @@
         Constructs an empty box object.
 
         `(self, min: LPoint3, max: LPoint3)`:
         Constructs a specific box object.
         """
     @overload
     def __init__(self, min: Vec3Like, max: Vec3Like) -> None: ...
-    def get_num_points(self) -> Literal[8]:
+    def get_num_points(self) -> int:
         """Returns 8: the number of vertices of a rectangular solid."""
     def get_point(self, n: int) -> LPoint3:
         """Returns the nth vertex of the rectangular solid."""
-    def get_num_planes(self) -> Literal[6]:
+    def get_num_planes(self) -> int:
         """Returns 6: the number of faces of a rectangular solid."""
     def get_plane(self, n: int) -> LPlane:
         """Returns the nth face of the rectangular solid."""
     def set_min_max(self, min: Vec3Like, max: Vec3Like) -> None:
         """Sets the min and max point of the rectangular solid."""
     def get_points(self) -> tuple[LPoint3, ...]: ...
     def get_planes(self) -> tuple[LPlane, ...]: ...
@@ -1433,19 +1446,19 @@
         fur: Vec3Like,
         ful: Vec3Like,
         nll: Vec3Like,
         nlr: Vec3Like,
         nur: Vec3Like,
         nul: Vec3Like,
     ) -> None: ...
-    def get_num_points(self) -> Literal[8]:
+    def get_num_points(self) -> int:
         """Returns 8: the number of vertices of a hexahedron."""
     def get_point(self, n: int) -> LPoint3:
         """Returns the nth vertex of the hexahedron."""
-    def get_num_planes(self) -> Literal[6]:
+    def get_num_planes(self) -> int:
         """Returns 6: the number of faces of a hexahedron."""
     def get_plane(self, n: int) -> LPlane:
         """Returns the nth face of the hexahedron."""
     def get_points(self) -> tuple[LPoint3, ...]: ...
     def get_planes(self) -> tuple[LPlane, ...]: ...
     getNumPoints = get_num_points
     getPoint = get_point
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_movies.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_movies.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,15 @@
             again.  This need be defined only if compare_timestamp() is also defined.
             """
         @staticmethod
         def get_class_type() -> TypeHandle: ...
         compareTimestamp = compare_timestamp
         getTimestamp = get_timestamp
         getClassType = get_class_type
+
     def __init__(self, __param0: MovieVideoCursor) -> None: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def get_source(self) -> MovieVideo:
         """Get the MovieVideo which this cursor references."""
     def size_x(self) -> int:
         """Get the horizontal size of the movie."""
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_nativenet.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_nativenet.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_net.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_net.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from collections.abc import Sequence
 from typing import Any, ClassVar, overload
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 from panda3d.core._dtoolutil import ostream
 from panda3d.core._express import Datagram, DatagramGenerator, DatagramSink, PointerToVoid, ReferenceCount
 from panda3d.core._nativenet import Socket_Address, Socket_IP
 
+class PointerToBase_Connection(PointerToVoid):
+    def clear(self) -> None: ...
+    def output(self, out: ostream) -> None: ...
+
 class PointerTo_Connection(PointerToBase_Connection):
     @overload
     def __init__(self, ptr: Connection = ...) -> None: ...
     @overload
     def __init__(self, copy: Connection) -> None: ...
     @overload
     def __init__(self, __param0: None) -> None: ...
@@ -22,18 +26,14 @@
         double-casting, and it can be run-time checked for correctness.
         """
     @overload
     def assign(self, ptr: Connection) -> Self: ...
     @overload
     def assign(self, copy: Connection) -> Self: ...
 
-class PointerToBase_Connection(PointerToVoid):
-    def clear(self) -> None: ...
-    def output(self, out: ostream) -> None: ...
-
 class NetAddress:
     """Represents a network address to which UDP packets may be sent or to which a
     TCP socket may be bound.
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     @overload
@@ -265,15 +265,15 @@
         the pipe is treated as a single datagram.
 
         This is similar to set_tcp_header_size(0), except that it also turns off
         headers for UDP packets.
         """
     def get_raw_mode(self) -> bool:
         """Returns the current setting of the raw mode flag.  See set_raw_mode()."""
-    def set_tcp_header_size(self, tcp_header_size: Literal[0, 2, 4]) -> None:
+    def set_tcp_header_size(self, tcp_header_size: int) -> None:
         """Sets the header size of TCP packets.  At the present, legal values for this
         are 0, 2, or 4; this specifies the number of bytes to use encode the
         datagram length at the start of each TCP datagram.  Sender and receiver
         must independently agree on this.
         """
     def get_tcp_header_size(self) -> int:
         """Returns the current setting of TCP header size.  See set_tcp_header_size()."""
@@ -361,14 +361,15 @@
         getIp = get_ip
         hasNetmask = has_netmask
         getNetmask = get_netmask
         hasBroadcast = has_broadcast
         getBroadcast = get_broadcast
         hasP2p = has_p2p
         getP2p = get_p2p
+
     DtoolClassDict: ClassVar[dict[str, Any]]
     @property
     def host_name(self) -> str: ...
     @property
     def interfaces(self) -> Sequence[ConnectionManager.Interface]: ...
     def __init__(self) -> None: ...
     @overload
@@ -591,15 +592,15 @@
         Setting the ConnectionWriter to raw mode must be done with care.  This can
         only be done when the matching ConnectionReader is also set to raw mode, or
         when the ConnectionWriter is communicating to a process that does not
         expect datagrams.
         """
     def get_raw_mode(self) -> bool:
         """Returns the current setting of the raw mode flag.  See set_raw_mode()."""
-    def set_tcp_header_size(self, tcp_header_size: Literal[0, 2, 4]) -> None:
+    def set_tcp_header_size(self, tcp_header_size: int) -> None:
         """Sets the header size of TCP packets.  At the present, legal values for this
         are 0, 2, or 4; this specifies the number of bytes to use encode the
         datagram length at the start of each TCP datagram.  Sender and receiver
         must independently agree on this.
         """
     def get_tcp_header_size(self) -> int:
         """Returns the current setting of TCP header size.  See set_tcp_header_size()."""
@@ -615,14 +616,27 @@
     isImmediate = is_immediate
     getNumThreads = get_num_threads
     setRawMode = set_raw_mode
     getRawMode = get_raw_mode
     setTcpHeaderSize = set_tcp_header_size
     getTcpHeaderSize = get_tcp_header_size
 
+class QueuedReturn_Datagram:
+    DtoolClassDict: ClassVar[dict[str, Any]]
+    def set_max_queue_size(self, max_size: int) -> None: ...
+    def get_max_queue_size(self) -> int: ...
+    def get_current_queue_size(self) -> int: ...
+    def get_overflow_flag(self) -> bool: ...
+    def reset_overflow_flag(self) -> None: ...
+    setMaxQueueSize = set_max_queue_size
+    getMaxQueueSize = get_max_queue_size
+    getCurrentQueueSize = get_current_queue_size
+    getOverflowFlag = get_overflow_flag
+    resetOverflowFlag = reset_overflow_flag
+
 class DatagramGeneratorNet(DatagramGenerator, ConnectionReader, QueuedReturn_Datagram):
     """This class provides datagrams one-at-a-time as read directly from the net,
     via a TCP connection.  If a datagram is not available, get_datagram() will
     block until one is.
     """
 
     def __init__(self, manager: ConnectionManager, num_threads: int) -> None:
@@ -646,27 +660,14 @@
     upcastToDatagramGenerator = upcast_to_DatagramGenerator
     upcastToConnectionReader = upcast_to_ConnectionReader
     upcastToQueuedReturnDatagram = upcast_to_QueuedReturn_Datagram
     getDatagram = get_datagram
     isEof = is_eof
     isError = is_error
 
-class QueuedReturn_Datagram:
-    DtoolClassDict: ClassVar[dict[str, Any]]
-    def set_max_queue_size(self, max_size: int) -> None: ...
-    def get_max_queue_size(self) -> int: ...
-    def get_current_queue_size(self) -> int: ...
-    def get_overflow_flag(self) -> bool: ...
-    def reset_overflow_flag(self) -> None: ...
-    setMaxQueueSize = set_max_queue_size
-    getMaxQueueSize = get_max_queue_size
-    getCurrentQueueSize = get_current_queue_size
-    getOverflowFlag = get_overflow_flag
-    resetOverflowFlag = reset_overflow_flag
-
 class DatagramSinkNet(DatagramSink, ConnectionWriter):
     """This class accepts datagrams one-at-a-time and sends them over the net, via
     a TCP connection.
     """
 
     def __init__(self, manager: ConnectionManager, num_threads: int) -> None:
         """Creates a new DatagramSinkNet with the indicated number of threads to
@@ -696,14 +697,27 @@
     upcastToDatagramSink = upcast_to_DatagramSink
     upcastToConnectionWriter = upcast_to_ConnectionWriter
     setTarget = set_target
     getTarget = get_target
     putDatagram = put_datagram
     isError = is_error
 
+class QueuedReturn_ConnectionListenerData:
+    DtoolClassDict: ClassVar[dict[str, Any]]
+    def set_max_queue_size(self, max_size: int) -> None: ...
+    def get_max_queue_size(self) -> int: ...
+    def get_current_queue_size(self) -> int: ...
+    def get_overflow_flag(self) -> bool: ...
+    def reset_overflow_flag(self) -> None: ...
+    setMaxQueueSize = set_max_queue_size
+    getMaxQueueSize = get_max_queue_size
+    getCurrentQueueSize = get_current_queue_size
+    getOverflowFlag = get_overflow_flag
+    resetOverflowFlag = reset_overflow_flag
+
 class QueuedConnectionListener(ConnectionListener, QueuedReturn_ConnectionListenerData):
     """This flavor of ConnectionListener will queue up all of the TCP connections
     it established for later detection by the client code.
     """
 
     def __init__(self, manager: ConnectionManager, num_threads: int) -> None: ...
     def upcast_to_ConnectionListener(self) -> ConnectionListener: ...
@@ -741,15 +755,15 @@
         new_connection: Connection | PointerTo_Connection,
     ) -> bool: ...
     upcastToConnectionListener = upcast_to_ConnectionListener
     upcastToQueuedReturnConnectionListenerData = upcast_to_QueuedReturn_ConnectionListenerData
     newConnectionAvailable = new_connection_available
     getNewConnection = get_new_connection
 
-class QueuedReturn_ConnectionListenerData:
+class QueuedReturn_PointerTo_Connection:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def set_max_queue_size(self, max_size: int) -> None: ...
     def get_max_queue_size(self) -> int: ...
     def get_current_queue_size(self) -> int: ...
     def get_overflow_flag(self) -> bool: ...
     def reset_overflow_flag(self) -> None: ...
     setMaxQueueSize = set_max_queue_size
@@ -799,15 +813,15 @@
         there are multiple threads accessing the QueuedConnectionManager).
         """
     upcastToConnectionManager = upcast_to_ConnectionManager
     upcastToQueuedReturnPointerToConnection = upcast_to_QueuedReturn_PointerTo_Connection
     resetConnectionAvailable = reset_connection_available
     getResetConnection = get_reset_connection
 
-class QueuedReturn_PointerTo_Connection:
+class QueuedReturn_NetDatagram:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def set_max_queue_size(self, max_size: int) -> None: ...
     def get_max_queue_size(self) -> int: ...
     def get_current_queue_size(self) -> int: ...
     def get_overflow_flag(self) -> bool: ...
     def reset_overflow_flag(self) -> None: ...
     setMaxQueueSize = set_max_queue_size
@@ -846,27 +860,14 @@
         are multiple threads accessing the QueuedConnectionReader).
         """
     upcastToConnectionReader = upcast_to_ConnectionReader
     upcastToQueuedReturnNetDatagram = upcast_to_QueuedReturn_NetDatagram
     dataAvailable = data_available
     getData = get_data
 
-class QueuedReturn_NetDatagram:
-    DtoolClassDict: ClassVar[dict[str, Any]]
-    def set_max_queue_size(self, max_size: int) -> None: ...
-    def get_max_queue_size(self) -> int: ...
-    def get_current_queue_size(self) -> int: ...
-    def get_overflow_flag(self) -> bool: ...
-    def reset_overflow_flag(self) -> None: ...
-    setMaxQueueSize = set_max_queue_size
-    getMaxQueueSize = get_max_queue_size
-    getCurrentQueueSize = get_current_queue_size
-    getOverflowFlag = get_overflow_flag
-    resetOverflowFlag = reset_overflow_flag
-
 class RecentConnectionReader(ConnectionReader):
     """This flavor of ConnectionReader will read from its sockets and retain only
     the single most recent datagram for inspection by client code.  It's useful
     particularly for reading telemetry-type data from UDP sockets where you
     don't care about getting every last socket, and in fact if the sockets are
     coming too fast you'd prefer to skip some of them.
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_parametrics.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_parametrics.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pgraph.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pgraph.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     ParamValueBase,
     PortalMask,
     TypedWritable,
     TypedWritableReferenceCount,
     UpdateSeq,
 )
 
-_N = TypeVar('_N', bound=PandaNode, covariant=True)
-_M = TypeVar('_M', bound=PandaNode)
+_N = TypeVar('_N', bound=PandaNode, default=PandaNode, covariant=True)
+_M = TypeVar('_M', bound=PandaNode, default=PandaNode)
 _RenderModeAttrib_Mode: TypeAlias = Literal[0, 1, 2, 3, 4, 5]
 _RenderAttrib_PandaCompareFunc: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8]
 _BoundingVolume_BoundsType: TypeAlias = Literal[0, 1, 2, 3, 4]
 _TransparencyAttrib_Mode: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6]
 _LogicOpAttrib_Operation: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16]
 _NodePath_ErrorType: TypeAlias = Literal[0, 1, 2, 3]
 _RenderAttrib_TexGenMode: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
@@ -1066,30 +1066,30 @@
     You should not attempt to create or modify a RenderState object directly.
     Instead, call one of the make() functions to create one for you.  And
     instead of modifying a RenderState object, create a new one.
     """
 
     @property
     def attribs(self) -> Mapping[TypeHandle, RenderAttrib]: ...
-    def compare_to(self, other: RenderAttrib | RenderState) -> int:
+    def compare_to(self, other: RenderState) -> int:
         """Provides an arbitrary ordering among all unique RenderStates, so we can
         store the essentially different ones in a big set and throw away the rest.
 
         This method is not needed outside of the RenderState class because all
         equivalent RenderState objects are guaranteed to share the same pointer;
         thus, a pointer comparison is always sufficient.
         """
-    def compare_sort(self, other: RenderAttrib | RenderState) -> int:
+    def compare_sort(self, other: RenderState) -> int:
         """Returns -1, 0, or 1 according to the relative sorting of these two
         RenderStates, with regards to rendering performance, so that "heavier"
         RenderAttribs (as defined by RenderAttribRegistry::get_slot_sort()) are
         more likely to be grouped together.  This is not related to the sorting
         order defined by compare_to.
         """
-    def compare_mask(self, other: RenderAttrib | RenderState, compare_mask: BitMask32 | int) -> int:
+    def compare_mask(self, other: RenderState, compare_mask: BitMask32 | int) -> int:
         """This version of compare_to takes a slot mask that indicates which
         attributes to include in the comparison.  Unlike compare_to, this method
         compares the attributes by pointer.
         """
     def get_hash(self) -> int:
         """Returns a suitable hash value for phash_map."""
     def is_empty(self) -> bool:
@@ -1141,24 +1141,24 @@
         attrib1: RenderAttrib,
         attrib2: RenderAttrib,
         attrib3: RenderAttrib,
         attrib4: RenderAttrib,
         attrib5: RenderAttrib,
         override: int = ...,
     ) -> RenderState: ...
-    def compose(self, other: RenderAttrib | RenderState) -> RenderState:
+    def compose(self, other: RenderState) -> RenderState:
         """Returns a new RenderState object that represents the composition of this
         state with the other state.
 
         The result of this operation is cached, and will be retained as long as
         both this RenderState object and the other RenderState object continue to
         exist.  Should one of them destruct, the cached entry will be removed, and
         its pointer will be allowed to destruct as well.
         """
-    def invert_compose(self, other: RenderAttrib | RenderState) -> RenderState:
+    def invert_compose(self, other: RenderState) -> RenderState:
         """Returns a new RenderState object that represents the composition of this
         state's inverse with the other state.
 
         This is similar to compose(), but is particularly useful for computing the
         relative state of a node as viewed from some other node.
         """
     def add_attrib(self, attrib: RenderAttrib, override: int = ...) -> RenderState:
@@ -1624,17 +1624,24 @@
 
     You should not attempt to create or modify a RenderEffects object directly.
     Instead, call one of the make() functions to create one for you.  And
     instead of modifying a RenderEffects object, create a new one.
     """
 
     def __lt__(self, other: RenderEffect | RenderEffects) -> bool: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of separate effects indicated in the state."""
     @overload
-    def __getitem__(self, type: TypeHandle | type) -> RenderEffect: ...
+    def __getitem__(self, type: TypeHandle | type) -> RenderEffect:
+        """`(self, type: TypeHandle)`:
+        Returns the effect in the state with the given type.
+
+        `(self, n: int)`:
+        Returns the nth effect in the state.
+        """
     @overload
     def __getitem__(self, n: int) -> RenderEffect: ...
     def is_empty(self) -> bool:
         """Returns true if the state is empty, false otherwise."""
     def get_num_effects(self) -> int:
         """Returns the number of separate effects indicated in the state.
         @deprecated in Python, use len(effects) instead, or effects.size() in C++.
@@ -2048,15 +2055,15 @@
         """
     def has_effect(self, type: TypeHandle | type) -> bool:
         """Returns true if there is a render effect of the indicated type defined on
         this node, or false if there is not.
         """
     def clear_effect(self, type: TypeHandle | type) -> None:
         """Removes the render effect of the given type from this node."""
-    def set_state(self, state: RenderAttrib | RenderState, current_thread: Thread = ...) -> None:
+    def set_state(self, state: RenderState, current_thread: Thread = ...) -> None:
         """Sets the complete RenderState that will be applied to all nodes at this
         level and below.  (The actual state that will be applied to lower nodes is
         based on the composition of RenderStates from above this node as well).
         This completely replaces whatever has been set on this node via repeated
         calls to set_attrib().
         """
     def get_state(self, current_thread: Thread = ...) -> RenderState:
@@ -2331,15 +2338,15 @@
         """Returns the union of all into_collide_mask() values set at CollisionNodes
         at this level and below.
         """
     def get_off_clip_planes(self, current_thread: Thread = ...) -> RenderAttrib:
         """Returns a ClipPlaneAttrib which represents the union of all of the clip
         planes that have been turned *off* at this level and below.
         """
-    def prepare_scene(self, gsg: GraphicsStateGuardianBase, node_state: RenderAttrib | RenderState) -> None:
+    def prepare_scene(self, gsg: GraphicsStateGuardianBase, node_state: RenderState) -> None:
         """Walks through the scene graph beginning at this node, and does whatever
         initialization is required to render the scene properly with the indicated
         GSG.  It is not strictly necessary to call this, since the GSG will
         initialize itself when the scene is rendered, but this may take some of the
         overhead away from that process.
 
         In particular, this will ensure that textures and vertex buffers within the
@@ -2821,16 +2828,22 @@
     getNodepath = get_nodepath
     getTexture = get_texture
     getSampler = get_sampler
 
 class InternalNameCollection:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: InternalNameCollection = ...) -> None: ...
-    def __getitem__(self, index: int) -> InternalName: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> InternalName:
+        """Returns the nth InternalName in the collection.  This is the same as
+        get_name(), but it may be a more convenient way to access it.
+        """
+    def __len__(self) -> int:
+        """Returns the number of names in the collection.  This is the same thing as
+        get_num_names().
+        """
     def __iadd__(self, other: InternalNameCollection) -> Self: ...
     def __add__(self, other: InternalNameCollection) -> InternalNameCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[InternalName]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_name(self, name: InternalName | str) -> None:
@@ -2881,16 +2894,22 @@
     getNumNames = get_num_names
     getName = get_name
     getNames = get_names
 
 class MaterialCollection:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: MaterialCollection = ...) -> None: ...
-    def __getitem__(self, index: int) -> Material: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> Material:
+        """Returns the nth Material in the collection.  This is the same as
+        get_material(), but it may be a more convenient way to access it.
+        """
+    def __len__(self) -> int:
+        """Returns the number of materials in the collection.  This is the same thing
+        as get_num_materials().
+        """
     def __iadd__(self, other: MaterialCollection) -> Self: ...
     def __add__(self, other: MaterialCollection) -> MaterialCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[Material]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_material(self, node_material: Material) -> None:
@@ -2944,16 +2963,22 @@
     findMaterial = find_material
     getNumMaterials = get_num_materials
     getMaterial = get_material
 
 class TextureStageCollection:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: TextureStageCollection = ...) -> None: ...
-    def __getitem__(self, index: int) -> TextureStage: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> TextureStage:
+        """Returns the nth TextureStage in the collection.  This is the same as
+        get_texture_stage(), but it may be a more convenient way to access it.
+        """
+    def __len__(self) -> int:
+        """Returns the number of texture stages in the collection.  This is the same
+        thing as get_num_texture_stages().
+        """
     def __iadd__(self, other: TextureStageCollection) -> Self: ...
     def __add__(self, other: TextureStageCollection) -> TextureStageCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[TextureStage]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_texture_stage(self, node_texture_stage: TextureStage) -> None:
@@ -3082,22 +3107,23 @@
         PandaNode is created with the indicated name.
         """
     @overload
     def __init__(self, copy: NodePath[_N]) -> None: ...
     @overload
     def __init__(self, node: _N, current_thread: Thread = ...) -> None: ...
     @overload
-    def __init__(self, top_node_name: str, current_thread: Thread = ...) -> None: ...
+    def __init__(self: NodePath[PandaNode], top_node_name: str, current_thread: Thread = ...) -> None: ...
     @overload
     def __init__(self, parent: NodePath, child_node: _N, current_thread: Thread = ...) -> None: ...
     def __bool__(self) -> bool: ...
     def __copy__(self) -> NodePath: ...
     def __deepcopy__(self, memo): ...
     def __reduce_persist__(self, pickler): ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison methods"""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: NodePath | WeakNodePath) -> bool: ...
     @staticmethod
     def any_path(node: _M, current_thread: Thread = ...) -> NodePath[_M]:
         """Returns a new NodePath that represents any arbitrary path from the root to
         the indicated node.  This is the same thing that would be returned by
         NodePath(node), except that no warning is issued if the path is ambiguous.
@@ -3386,25 +3412,25 @@
 
         `(self, current_thread: Thread = ...)`:
         Returns the complete state object set on this node.
         """
     @overload
     def get_state(self, other: NodePath, current_thread: Thread = ...) -> RenderState: ...
     @overload
-    def set_state(self, state: RenderAttrib | RenderState, current_thread: Thread = ...) -> None:
+    def set_state(self, state: RenderState, current_thread: Thread = ...) -> None:
         """`(self, other: NodePath, state: RenderState, current_thread: Thread = ...)`:
         Sets the state object on this node, relative to the other node.  This
         computes a new state object that will have the indicated value when seen
         from the other node.
 
         `(self, state: RenderState, current_thread: Thread = ...)`:
         Changes the complete state object on this node.
         """
     @overload
-    def set_state(self, other: NodePath, state: RenderAttrib | RenderState, current_thread: Thread = ...) -> None: ...
+    def set_state(self, other: NodePath, state: RenderState, current_thread: Thread = ...) -> None: ...
     def get_net_state(self, current_thread: Thread = ...) -> RenderState:
         """Returns the net state on this node from the root."""
     def set_attrib(self, attrib: RenderAttrib, priority: int = ...) -> None:
         """Adds the indicated render attribute to the scene graph on this node.  This
         attribute will now apply to this node and everything below.  If there was
         already an attribute of the same type, it is replaced.
         """
@@ -5918,15 +5944,18 @@
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     @overload
     def __init__(self, __param0: NodePathCollection = ...) -> None: ...
     @overload
     def __init__(self, sequence: Sequence[NodePath]) -> None: ...
     def __getitem__(self, index: int) -> NodePath: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of paths in the collection.  This is the same thing as
+        get_num_paths().
+        """
     def __iadd__(self, other: NodePathCollection) -> Self: ...
     def __add__(self, other: NodePathCollection) -> NodePathCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[NodePath]: ...  # Doesn't actually exist
     def add_path(self, node_path: NodePath) -> None:
         """Adds a new NodePath to the collection."""
@@ -6820,15 +6849,15 @@
         some other viewpoint.  This may be used, for instance, to reduce LOD
         popping when the camera rotates in a small circle about an avatar.
         """
     def get_lod_center(self) -> NodePath:
         """Returns the point from which the LOD distances will be measured, if it was
         set by set_lod_center(), or the empty NodePath otherwise.
         """
-    def set_initial_state(self, state: RenderAttrib | RenderState) -> None:
+    def set_initial_state(self, state: RenderState) -> None:
         """Sets the initial state which is applied to all nodes in the scene, as if it
         were set at the top of the scene graph.
         """
     def get_initial_state(self) -> RenderState:
         """Returns the initial state as set by a previous call to set_initial_state()."""
     def set_tag_state_key(self, tag_state_key: str) -> None:
         """Sets the tag key which, when encountered as a tag on nodes in the scene
@@ -6839,15 +6868,15 @@
         """Returns the tag key as set by a previous call to set_tag_state_key()."""
     def set_lod_scale(self, value: float) -> None:
         """Sets the multiplier for LOD distances.  This value is multiplied with the
         LOD scale set on LodNodes.
         """
     def get_lod_scale(self) -> float:
         """Returns the multiplier for LOD distances."""
-    def set_tag_state(self, tag_state: str, state: RenderAttrib | RenderState) -> None:
+    def set_tag_state(self, tag_state: str, state: RenderState) -> None:
         """Associates a particular state transition with the indicated tag value.
         When a node is encountered during traversal with the tag key specified by
         set_tag_state_key(), if the value of that tag matches tag_state, then the
         indicated state is applied to this node--but only when it is rendered by
         this camera.
 
         This can be used to apply special effects to nodes when they are rendered
@@ -7609,26 +7638,26 @@
         """
     def get_geom_state(self, n: int) -> RenderState:
         """Returns the RenderState associated with the nth geom of the node.  This is
         just the RenderState directly associated with the Geom; the actual state in
         which the Geom is rendered will also be affected by RenderStates that
         appear on the scene graph in nodes above this GeomNode.
         """
-    def set_geom_state(self, n: int, state: RenderAttrib | RenderState) -> None:
+    def set_geom_state(self, n: int, state: RenderState) -> None:
         """Changes the RenderState associated with the nth geom of the node.  This is
         just the RenderState directly associated with the Geom; the actual state in
         which the Geom is rendered will also be affected by RenderStates that
         appear on the scene graph in nodes above this GeomNode.
 
         Note that if this method is called in a downstream stage (for instance,
         during cull or draw), then it will propagate the new list of Geoms upstream
         all the way to pipeline stage 0, which may step on changes that were made
         independently in pipeline stage 0. Use with caution.
         """
-    def add_geom(self, geom: Geom, state: RenderAttrib | RenderState = ...) -> None:
+    def add_geom(self, geom: Geom, state: RenderState = ...) -> None:
         """Adds a new Geom to the node.  The geom is given the indicated state (which
         may be RenderState::make_empty(), to completely inherit its state from the
         scene graph).
         """
     def add_geoms_from(self, other: GeomNode) -> None:
         """Copies the Geoms (and their associated RenderStates) from the indicated
         GeomNode into this one.
@@ -8120,15 +8149,15 @@
         """
     def get_cull_bounds(self) -> BoundingVolume:
         """Returns the bounding volume that should be used to perform view-frustum
         culling (in the space of get_cull_center()).  This is normally the current
         lens' bounding volume, but it may be overridden with
         Camera::set_cull_bounds().
         """
-    def set_initial_state(self, initial_state: RenderAttrib | RenderState) -> None:
+    def set_initial_state(self, initial_state: RenderState) -> None:
         """Sets the initial state which is applied to all nodes in the scene, as if it
         were set at the top of the scene graph.
         """
     def get_initial_state(self) -> RenderState:
         """Returns the initial state as set by a previous call to set_initial_state()."""
     def set_camera_transform(self, camera_transform: TransformState) -> None:
         """Specifies the position of the camera relative to the starting node."""
@@ -9168,14 +9197,15 @@
         def get_files(self) -> tuple[Filename, ...]: ...
         def get_file_types(self) -> tuple[LoaderFileType, ...]: ...
         getNumFiles = get_num_files
         getFile = get_file
         getFileType = get_file_type
         getFiles = get_files
         getFileTypes = get_file_types
+
     @overload
     def __init__(self, name: str = ...) -> None: ...
     @overload
     def __init__(self, __param0: Loader) -> None: ...
     def upcast_to_TypedReferenceCount(self) -> TypedReferenceCount: ...
     def upcast_to_Namable(self) -> Namable: ...
     def set_task_manager(self, task_manager: AsyncTaskManager) -> None:
@@ -9193,21 +9223,21 @@
     def stop_threads(self) -> None:
         """Stop any threads used for asynchronous loads."""
     def remove(self, task: AsyncTask) -> bool:
         """Removes a pending asynchronous load request.  Returns true if successful,
         false otherwise.
         @deprecated use task.cancel() to cancel the request instead.
         """
-    def load_sync(self, filename: StrOrBytesPath, options: LoaderOptions | int = ...) -> PandaNode:
+    def load_sync(self, filename: StrOrBytesPath, options: LoaderOptions = ...) -> PandaNode:
         """Loads the file immediately, waiting for it to complete.
 
         If search is true, the file is searched for along the model path;
         otherwise, only the exact filename is loaded.
         """
-    def make_async_request(self, filename: StrOrBytesPath, options: LoaderOptions | int = ...) -> AsyncTask:
+    def make_async_request(self, filename: StrOrBytesPath, options: LoaderOptions = ...) -> AsyncTask:
         """Returns a new AsyncTask object suitable for adding to load_async() to start
         an asynchronous model load.
         """
     def load_async(self, request: AsyncTask) -> None:
         """Begins an asynchronous load request.  To use this call, first call
         make_async_request() to create a new ModelLoadRequest object with the
         filename you wish to load, and then add that object to the Loader with
@@ -9215,17 +9245,17 @@
         loaded in the background.
 
         To determine when the model has completely loaded, you may poll
         request->is_ready() from time to time, or set the done_event on the request
         object and listen for that event.  When the model is ready, you may
         retrieve it via request->get_model().
         """
-    def save_sync(self, filename: StrOrBytesPath, options: LoaderOptions | int, node: PandaNode) -> bool:
+    def save_sync(self, filename: StrOrBytesPath, options: LoaderOptions, node: PandaNode) -> bool:
         """Saves the file immediately, waiting for it to complete."""
-    def make_async_save_request(self, filename: StrOrBytesPath, options: LoaderOptions | int, node: PandaNode) -> AsyncTask:
+    def make_async_save_request(self, filename: StrOrBytesPath, options: LoaderOptions, node: PandaNode) -> AsyncTask:
         """Returns a new AsyncTask object suitable for adding to save_async() to start
         an asynchronous model save.
         """
     def save_async(self, request: AsyncTask) -> None:
         """Begins an asynchronous save request.  To use this call, first call
         make_async_save_request() to create a new ModelSaveRequest object with the
         filename you wish to load, and then add that object to the Loader with
@@ -9274,19 +9304,19 @@
         """Returns a space-separated list of extension, in addition to the one
         returned by get_extension(), that are recognized by this loader.
         """
     def supports_compressed(self) -> bool:
         """Returns true if this file type can transparently load compressed files
         (with a .pz or .gz extension), false otherwise.
         """
-    def get_allow_disk_cache(self, options: LoaderOptions | int) -> bool:
+    def get_allow_disk_cache(self, options: LoaderOptions) -> bool:
         """Returns true if the loader flags allow retrieving the model from the on-
         disk bam cache (if it is enabled), false otherwise.
         """
-    def get_allow_ram_cache(self, options: LoaderOptions | int) -> bool:
+    def get_allow_ram_cache(self, options: LoaderOptions) -> bool:
         """Returns true if the loader flags allow retrieving the model from the in-
         memory ModelPool cache, false otherwise.
         """
     def supports_load(self) -> bool:
         """Returns true if the file type can be used to load files, and load_file() is
         supported.  Returns false if load_file() is unimplemented and will always
         fail.
@@ -9431,15 +9461,15 @@
     def loader(self) -> Loader: ...
     @overload
     def __init__(self, __param0: ModelLoadRequest) -> None:
         """Create a new ModelLoadRequest, and add it to the loader via load_async(),
         to begin an asynchronous load.
         """
     @overload
-    def __init__(self, name: str, filename: StrOrBytesPath, options: LoaderOptions | int, loader: Loader) -> None: ...
+    def __init__(self, name: str, filename: StrOrBytesPath, options: LoaderOptions, loader: Loader) -> None: ...
     def get_filename(self) -> Filename:
         """Returns the filename associated with this asynchronous ModelLoadRequest."""
     def get_options(self) -> LoaderOptions:
         """Returns the LoaderOptions associated with this asynchronous
         ModelLoadRequest.
         """
     def get_loader(self) -> Loader:
@@ -9647,15 +9677,15 @@
     def get_model(filename: StrOrBytesPath, verify: bool) -> ModelRoot:
         """Returns the model that has already been previously loaded, or NULL
         otherwise.  If verify is true, it will check if the file is still up-to-
         date (and hasn't been modified in the meantime), and if not, will still
         return NULL.
         """
     @staticmethod
-    def load_model(filename: StrOrBytesPath, options: LoaderOptions | int = ...) -> ModelRoot:
+    def load_model(filename: StrOrBytesPath, options: LoaderOptions = ...) -> ModelRoot:
         """Loads the given filename up as a model, if it has not already been loaded,
         and returns the new model.  If a model with the same filename was
         previously loaded, returns that one instead (unless cache-check-timestamps
         is true and the file has recently changed).  If the model file cannot be
         found, or cannot be loaded for some reason, returns NULL.
         """
     @overload
@@ -9745,17 +9775,15 @@
     def loader(self) -> Loader: ...
     @overload
     def __init__(self, __param0: ModelSaveRequest) -> None:
         """Create a new ModelSaveRequest, and add it to the loader via save_async(),
         to begin an asynchronous save.
         """
     @overload
-    def __init__(
-        self, name: str, filename: StrOrBytesPath, options: LoaderOptions | int, node: PandaNode, loader: Loader
-    ) -> None: ...
+    def __init__(self, name: str, filename: StrOrBytesPath, options: LoaderOptions, node: PandaNode, loader: Loader) -> None: ...
     def get_filename(self) -> Filename:
         """Returns the filename associated with this asynchronous ModelSaveRequest."""
     def get_options(self) -> LoaderOptions:
         """Returns the LoaderOptions associated with this asynchronous
         ModelSaveRequest.
         """
     def get_node(self) -> PandaNode:
@@ -10077,15 +10105,15 @@
     def get_min_coverage(self) -> float:
         """Returns the minimum screen coverage."""
     def set_vertices(self, v0: Vec3Like, v1: Vec3Like, v2: Vec3Like, v3: Vec3Like) -> None:
         """Replaces the four vertices of the occluder polygon.  The vertices should be
         defined in a counterclockwise orientation when looking at the face of the
         occluder.
         """
-    def get_num_vertices(self) -> Literal[4]:
+    def get_num_vertices(self) -> int:
         """Returns the number of vertices in the occluder polygon.  This should always
         return 4.
         """
     def get_vertex(self, n: int) -> LPoint3:
         """Returns the nth vertex of the occluder polygon."""
     def set_vertex(self, n: int, v: Vec3Like) -> None:
         """Sets the nth vertex of the occluder polygon."""
@@ -10149,15 +10177,16 @@
     ALINEAR: Final = 0
     AQUADRATIC: Final = 1
     @overload
     def __init__(self, __param0: PolylightNode) -> None:
         """Use PolylightNode() to construct a new PolylightNode object."""
     @overload
     def __init__(self, name: str) -> None: ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison methods"""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: PolylightNode) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def enable(self) -> None:
         """Enable this light"""
     def disable(self) -> None:
@@ -10860,15 +10889,15 @@
         """
     def remove_unused_vertices(self, root: PandaNode) -> None:
         """Removes any vertices in GeomVertexDatas that are no longer used at this
         level and below.  This requires remapping vertex indices in all of the
         GeomPrimitives, to remove holes in the GeomVertexDatas.  It is normally not
         necessary to call this explicitly.
         """
-    def premunge(self, root: PandaNode, initial_state: RenderAttrib | RenderState) -> None:
+    def premunge(self, root: PandaNode, initial_state: RenderState) -> None:
         """Walks the scene graph rooted at this node and below, and uses the indicated
         GSG to premunge every Geom found to optimize it for eventual rendering on
         the indicated GSG.  If there is no GSG indicated for the SceneGraphReducer,
         this is a no-op.
 
         This operation will also apply to stashed children.
         """
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pgraphnodes.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pgraphnodes.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,15 @@
 
 from panda3d._typing import IntVec2Like, IntVec3Like, Vec3Like, Vec4Like
 from panda3d.core._dtoolutil import ostream
 from panda3d.core._express import TypedReferenceCount
 from panda3d.core._gobj import GeomVertexAnimationSpec, Texture
 from panda3d.core._gsgbase import GraphicsOutputBase, GraphicsStateGuardianBase
 from panda3d.core._linmath import LColor, LPoint3, LVecBase2i, LVecBase3, LVecBase3i, LVector3
-from panda3d.core._pgraph import (
-    Camera,
-    CullTraverser,
-    CullTraverserData,
-    Light,
-    PandaNode,
-    RenderAttrib,
-    RenderState,
-    ShaderAttrib,
-)
+from panda3d.core._pgraph import Camera, CullTraverser, CullTraverserData, Light, PandaNode, RenderState, ShaderAttrib
 from panda3d.core._putil import AnimInterface, CallbackData, CallbackObject
 
 _SceneGraphAnalyzer_LodMode: TypeAlias = Literal[0, 1, 2, 3]
 
 class LightNode(Light, PandaNode):  # type: ignore[misc]
     """A derivative of Light and of PandaNode.  All kinds of Light except
     Spotlight (which must inherit from LensNode instead) inherit from this
@@ -561,15 +552,15 @@
         certain results.  The parameter that must be passed is the GSG to which the
         shader generator belongs.
         """
     @overload
     def __init__(self, __param0: ShaderGenerator) -> None: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
-    def synthesize_shader(self, rs: RenderAttrib | RenderState, anim: GeomVertexAnimationSpec) -> ShaderAttrib:
+    def synthesize_shader(self, rs: RenderState, anim: GeomVertexAnimationSpec) -> ShaderAttrib:
         """This is the routine that implements the next-gen fixed function pipeline by
         synthesizing a shader.  It also takes care of setting up any buffers needed
         to produce the requested effects.
 
         Currently supports:
         - flat colors
         - vertex colors
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pgui.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pgui.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -324,25 +324,25 @@
         """Returns the event name that will be thrown when the item gets the keyboard
         focus.
         """
     def get_focus_out_event(self) -> str:
         """Returns the event name that will be thrown when the item loses the keyboard
         focus.
         """
-    def get_press_event(self, button: ButtonHandle | int | str) -> str:
+    def get_press_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the item is active and the
         indicated mouse or keyboard button is depressed while the mouse is within
         the frame.
         """
-    def get_repeat_event(self, button: ButtonHandle | int | str) -> str:
+    def get_repeat_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the item is active and the
         indicated mouse or keyboard button is continuously held down while the
         mouse is within the frame.
         """
-    def get_release_event(self, button: ButtonHandle | int | str) -> str:
+    def get_release_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the item is active and the
         indicated mouse or keyboard button, formerly clicked down is within the
         frame, is released.
         """
     def get_keystroke_event(self) -> str:
         """Returns the event name that will be thrown when the item is active and any
         key is pressed by the user.
@@ -460,40 +460,40 @@
         create the label geometry.  This automatically sets up the frame according
         to the size of the text.
         """
     @overload
     def setup(self, label: str, bevel: float = ...) -> None: ...
     @overload
     def setup(self, ready: NodePath, depressed: NodePath, rollover: NodePath, inactive: NodePath = ...) -> None: ...
-    def add_click_button(self, button: ButtonHandle | int | str) -> bool:
+    def add_click_button(self, button: ButtonHandle | str) -> bool:
         """Adds the indicated button to the set of buttons that can effectively
         "click" the PGButton.  Normally, this is just MouseButton::one().  Returns
         true if the button was added, or false if it was already there.
         """
-    def remove_click_button(self, button: ButtonHandle | int | str) -> bool:
+    def remove_click_button(self, button: ButtonHandle | str) -> bool:
         """Removes the indicated button from the set of buttons that can effectively
         "click" the PGButton.  Normally, this is just MouseButton::one().  Returns
         true if the button was removed, or false if it was not in the set.
         """
-    def has_click_button(self, button: ButtonHandle | int | str) -> bool:
+    def has_click_button(self, button: ButtonHandle | str) -> bool:
         """Returns true if the indicated button is on the set of buttons that can
         effectively "click" the PGButton.  Normally, this is just
         MouseButton::one().
         """
     def is_button_down(self) -> bool:
         """Returns true if the user is currently holding the mouse button down on the
         button, false otherwise.
         """
     @staticmethod
     def get_click_prefix() -> str:
         """Returns the prefix that is used to define the click event for all
         PGButtons.  The click event is the concatenation of this string followed by
         get_id().
         """
-    def get_click_event(self, button: ButtonHandle | int | str) -> str:
+    def get_click_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the button is clicked
         normally.
         """
     addClickButton = add_click_button
     removeClickButton = remove_click_button
     hasClickButton = has_click_button
     isButtonDown = is_button_down
@@ -772,19 +772,19 @@
         """
     @staticmethod
     def get_cursormove_prefix() -> str:
         """Returns the prefix that is used to define the cursor event for all
         PGEntries.  The cursor event is the concatenation of this string followed
         by get_id().
         """
-    def get_accept_event(self, button: ButtonHandle | int | str) -> str:
+    def get_accept_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the entry is accepted
         normally.
         """
-    def get_accept_failed_event(self, button: ButtonHandle | int | str) -> str:
+    def get_accept_failed_event(self, button: ButtonHandle | str) -> str:
         """Returns the event name that will be thrown when the entry cannot accept an
         input
         """
     def get_overflow_event(self) -> str:
         """Returns the event name that will be thrown when too much text is attempted
         to be entered into the PGEntry, exceeding either the limit set via
         set_max_chars() or via set_max_width().
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pipeline.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pipeline.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pnmimage.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pnmimage.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def __mul__(self, mult: float) -> pixel: ...
     def __iadd__(self, other: pixel) -> Self: ...
     def __isub__(self, other: pixel) -> Self: ...
     def __imul__(self, mult: float) -> Self: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: pixel) -> bool: ...
-    def __len__(self) -> Literal[3]: ...
+    def __len__(self) -> int: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
     def output(self, out: ostream) -> None: ...
 
 class PNMFileType(TypedWritable):
     """This is the base class of a family of classes that represent particular
@@ -142,15 +142,18 @@
         def __init__(self, gray_value: int, alpha: int = ...) -> None: ...
         @overload
         def __init__(self, red: int, green: int, blue: int, alpha: int = ...) -> None: ...
         def __lt__(self, other: PNMImageHeader.PixelSpec | pixel) -> bool: ...
         def __eq__(self, __other: object) -> bool: ...
         def __ne__(self, __other: object) -> bool: ...
         def __getitem__(self, n: int) -> int: ...
-        def __len__(self) -> Literal[4]: ...
+        def __len__(self) -> int:
+            """Specifies the number of components in the PixelSpec; this is always 4,
+            regardless of the type of image it was taken from.
+            """
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
         def compare_to(self, other: PNMImageHeader.PixelSpec | pixel) -> int: ...
         def get_red(self) -> int: ...
         def get_green(self) -> int: ...
         def get_blue(self) -> int: ...
@@ -207,14 +210,15 @@
         def get_count(self, n: int) -> int: ...
         def write(self, out: ostream) -> None: ...
         def get_pixels(self) -> tuple[PNMImageHeader.PixelSpec, ...]: ...
         getNumPixels = get_num_pixels
         getPixel = get_pixel
         getCount = get_count
         getPixels = get_pixels
+
     CT_invalid: Final = 0
     CTInvalid: Final = 0
     CT_grayscale: Final = 1
     CTGrayscale: Final = 1
     CT_two_channel: Final = 2
     CTTwoChannel: Final = 2
     CT_color: Final = 3
@@ -952,17 +956,21 @@
     class Row:
         """Provides an accessor for reading or writing the contents of one row of
         the image in-place.
         """
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: PNMImage.Row) -> None: ...
-        def __len__(self) -> int: ...
+        def __len__(self) -> int:
+            """Get the number of pixels in the row."""
         def __getitem__(self, x: int) -> LColorf: ...
-        def __setitem__(self, x: int, v: Vec4Like) -> None: ...
+        def __setitem__(self, x: int, v: Vec4Like) -> None:
+            """Set the pixel at the given column in the row.  If the image has no alpha
+            channel, the alpha component is ignored.
+            """
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[LColorf]: ...  # Doesn't actually exist
         def get_xel_val(self, x: int) -> xel:
             """Fetch the pixel at the given column in the row."""
         def set_xel_val(self, x: int, v: xel) -> None:
             """Set the pixel at the given column in the row."""
@@ -978,25 +986,27 @@
     class CRow:
         """Provides an accessor for reading the contents of one row of the image in-
         place.
         """
 
         DtoolClassDict: ClassVar[dict[str, Any]]
         def __init__(self, __param0: PNMImage.CRow) -> None: ...
-        def __len__(self) -> int: ...
+        def __len__(self) -> int:
+            """Get the number of pixels in the row."""
         def __getitem__(self, x: int) -> LColorf: ...
         def __copy__(self) -> Self: ...
         def __deepcopy__(self, __memo: object) -> Self: ...
         def __iter__(self) -> Iterator[LColorf]: ...  # Doesn't actually exist
         def get_xel_val(self, x: int) -> xel:
             """Fetch the pixel at the given column in the row."""
         def get_alpha_val(self, x: int) -> int:
             """Fetch the alpha value at the given column in the row."""
         getXelVal = get_xel_val
         getAlphaVal = get_alpha_val
+
     @overload
     def __init__(self, copy: PNMImage = ...) -> None: ...
     @overload
     def __init__(self, filename: StrOrBytesPath, type: PNMFileType = ...) -> None: ...
     @overload
     def __init__(
         self,
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pnmtext.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pnmtext.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_prc.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_prc.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -980,15 +980,16 @@
     @overload
     def __init__(self, __param0: ConfigVariableBool) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: bool | str, description: str = ..., flags: int = ...) -> None: ...
     def __bool__(self) -> bool: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of unique words in the variable."""
     def __getitem__(self, n: int) -> bool: ...
     def __iter__(self) -> Iterator[bool]: ...  # Doesn't actually exist
     def assign(self, value: bool) -> Self: ...
     def set_value(self, value: bool) -> None:
         """Reassigns the variable's local value."""
     def get_value(self) -> bool:
         """Returns the variable's value."""
@@ -1017,15 +1018,16 @@
     @overload
     def __init__(self, __param0: ConfigVariableDouble) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: float | str, description: str = ..., flags: int = ...) -> None: ...
     def __float__(self) -> float: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of unique words in the variable."""
     def __getitem__(self, n: int) -> float: ...
     def __iter__(self) -> Iterator[float]: ...  # Doesn't actually exist
     def assign(self, value: float) -> Self: ...
     def set_value(self, value: float) -> None:
         """Reassigns the variable's local value."""
     def get_value(self) -> float:
         """Returns the variable's value."""
@@ -1057,18 +1059,24 @@
     @overload
     def __init__(self, __param0: ConfigVariableFilename) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: StrOrBytesPath, description: str = ..., flags: int = ...) -> None: ...
     def __getitem__(self, n: int) -> str: ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison operators are handy."""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: StrOrBytesPath) -> bool: ...
-    def __fspath__(self) -> str: ...
+    def __fspath__(self) -> str:
+        """Allows a ConfigVariableFilename object to be passed to any Python function
+        that accepts an os.PathLike object.
+
+        @since 1.10.13
+        """
     def operator_typecast(self) -> Filename: ...
     def assign(self, value: StrOrBytesPath) -> Self: ...
     def c_str(self) -> str:
         """These methods help the ConfigVariableFilename act like a Filename object."""
     def empty(self) -> bool: ...
     def length(self) -> int: ...
     def get_fullpath(self) -> str:
@@ -1132,15 +1140,16 @@
     @overload
     def __init__(self, __param0: ConfigVariableInt) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: int | str, description: str = ..., flags: int = ...) -> None: ...
     def __int__(self) -> int: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of unique words in the variable."""
     def __getitem__(self, n: int) -> int: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
     def assign(self, value: int) -> Self: ...
     def set_value(self, value: int) -> None:
         """Reassigns the variable's local value."""
     def get_value(self) -> int:
         """Returns the variable's value."""
@@ -1169,15 +1178,16 @@
     @overload
     def __init__(self, __param0: ConfigVariableInt64) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: int | str, description: str = ..., flags: int = ...) -> None: ...
     def __int__(self) -> int: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of unique words in the variable."""
     def __getitem__(self, n: int) -> int: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
     def assign(self, value: int) -> Self: ...
     def set_value(self, value: int) -> None:
         """Reassigns the variable's local value."""
     def get_value(self) -> int:
         """Returns the variable's value."""
@@ -1207,15 +1217,16 @@
     A ConfigVariableList cannot be modified locally.
     """
 
     @overload
     def __init__(self, __param0: ConfigVariableList) -> None: ...
     @overload
     def __init__(self, name: str, description: str = ..., flags: int = ...) -> None: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of unique values of the variable."""
     def __getitem__(self, n: int) -> str: ...
     def __iter__(self) -> Iterator[str]: ...  # Doesn't actually exist
     def get_num_values(self) -> int:
         """Returns the number of values in the variable."""
     def get_string_value(self, n: int) -> str:
         """Returns the nth value of the variable."""
     def get_num_unique_values(self) -> int:
@@ -1332,15 +1343,16 @@
     @overload
     def __init__(self, __param0: ConfigVariableString) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     @overload
     def __init__(self, name: str, default_value: str, description: str = ..., flags: int = ...) -> None: ...
     def __getitem__(self, n: int) -> str: ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison operators are handy."""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: str) -> bool: ...
     def assign(self, value: str) -> Self: ...
     def c_str(self) -> str:
         """These methods help the ConfigVariableString act like a C++ string object."""
     def empty(self) -> bool: ...
     def length(self) -> int: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_pstatclient.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_pstatclient.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_putil.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_putil.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 
 _ColorSpace: TypeAlias = Literal[0, 1, 2, 3]
 _AutoTextureScale: TypeAlias = Literal[0, 1, 2, 3, 4]
 _BamEnums_BamEndian: TypeAlias = Literal[0, 1, 1]
 _BamEnums_BamTextureMode: TypeAlias = Literal[0, 1, 2, 3, 4]
 _ClockObject_Mode: TypeAlias = Literal[0, 1, 2, 3, 4, 5, 6, 7]
 
+class PointerToBase_ReferenceCountedVector_ushort(PointerToVoid):
+    def clear(self) -> None: ...
+    def output(self, out: ostream) -> None: ...
+
+class PointerToArrayBase_ushort(PointerToBase_ReferenceCountedVector_ushort):
+    def __eq__(self, __other: object) -> bool:
+        """These are implemented in PointerToVoid, but expose them here."""
+    def __ne__(self, __other: object) -> bool: ...
+
 class ConstPointerToArray_ushort(PointerToArrayBase_ushort):
     def __init__(self, copy: ConstPointerToArray_ushort | PointerToArray_ushort) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, n: int) -> int: ...
     def __deepcopy__(self, memo) -> ConstPointerToArray_ushort: ...
     def __copy__(self) -> Self: ...
     def __iter__(self) -> Iterator[int]: ...  # Doesn't actually exist
@@ -70,22 +79,14 @@
     def count(self, __param0: int) -> int: ...
     getElement = get_element
     getData = get_data
     getSubdata = get_subdata
     getRefCount = get_ref_count
     getNodeRefCount = get_node_ref_count
 
-class PointerToArrayBase_ushort(PointerToBase_ReferenceCountedVector_ushort):
-    def __eq__(self, __other: object) -> bool: ...
-    def __ne__(self, __other: object) -> bool: ...
-
-class PointerToBase_ReferenceCountedVector_ushort(PointerToVoid):
-    def clear(self) -> None: ...
-    def output(self, out: ostream) -> None: ...
-
 class PointerToArray_ushort(PointerToArrayBase_ushort):
     @overload
     def __init__(self, type_handle: TypeHandle | type = ...) -> None: ...
     @overload
     def __init__(self, copy: PointerToArray_ushort) -> None: ...
     @overload
     def __init__(self, source: Sequence[int]) -> None: ...
@@ -907,15 +908,15 @@
         This enables the reader to interpret pathnames in the BAM as relative to
         the directory containing the BAM.
         """
     def get_loader_options(self) -> LoaderOptions:
         """Returns the LoaderOptions passed to the loader when the model was
         requested, if any.
         """
-    def set_loader_options(self, options: LoaderOptions | int) -> None:
+    def set_loader_options(self, options: LoaderOptions) -> None:
         """Specifies the LoaderOptions for this BamReader."""
     def read_object(self) -> TypedWritable:
         """Reads a single object from the Bam file.  If the object type is known, a
         new object of the appropriate type is created and returned; otherwise, NULL
         is returned.  NULL is also returned when the end of the file is reached.
         is_eof() may be called to differentiate between these two cases.
 
@@ -1762,21 +1763,21 @@
     @overload
     def __init__(self, index: int) -> None: ...
     @overload
     def __init__(self, name: str) -> None: ...
     def __bool__(self) -> bool: ...
     def __eq__(self, __other: object) -> bool: ...
     def __ne__(self, __other: object) -> bool: ...
-    def __lt__(self, other: ButtonHandle | int | str) -> bool: ...
-    def __le__(self, other: ButtonHandle | int | str) -> bool: ...
-    def __gt__(self, other: ButtonHandle | int | str) -> bool: ...
-    def __ge__(self, other: ButtonHandle | int | str) -> bool: ...
+    def __lt__(self, other: ButtonHandle | str) -> bool: ...
+    def __le__(self, other: ButtonHandle | str) -> bool: ...
+    def __gt__(self, other: ButtonHandle | str) -> bool: ...
+    def __ge__(self, other: ButtonHandle | str) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
-    def compare_to(self, other: ButtonHandle | int | str) -> int:
+    def compare_to(self, other: ButtonHandle | str) -> int:
         """Sorts ButtonHandles arbitrarily (according to <, >, etc.).  Returns a
         number less than 0 if this type sorts before the other one, greater than
         zero if it sorts after, 0 if they are equivalent.
         """
     def get_hash(self) -> int:
         """Returns a hash code suitable for phash_map."""
     def get_name(self) -> str:
@@ -1793,15 +1794,15 @@
         """Returns the alias (alternate name) associated with the button, if any, or
         ButtonHandle::none() if the button has no alias.
 
         Each button is allowed to have one alias, and multiple different buttons
         can refer to the same alias.  The alias should be the more general name for
         the button, for instance, shift is an alias for lshift, but not vice-versa.
         """
-    def matches(self, other: ButtonHandle | int | str) -> bool:
+    def matches(self, other: ButtonHandle | str) -> bool:
         """Returns true if this ButtonHandle is the same as the other one, or if the
         other one is an alias for this one.  (Does not return true if this button
         is an alias for the other one, however.)
 
         This is a more general comparison than operator ==.
         """
     def get_index(self) -> int:
@@ -2848,25 +2849,25 @@
         """
     def matches(self, other: ModifierButtons) -> bool:
         """Returns true if the set of buttons indicated as down by this
         ModifierButtons object is the same set of buttons indicated as down by the
         other ModifierButtons object.  The buttons indicated as up are not
         relevant.
         """
-    def add_button(self, button: ButtonHandle | int | str) -> bool:
+    def add_button(self, button: ButtonHandle | str) -> bool:
         """Adds the indicated button to the set of buttons that will be monitored for
         upness and downness.  Returns true if the button was added, false if it was
         already being monitored or if too many buttons are currently being
         monitored.
         """
-    def has_button(self, button: ButtonHandle | int | str) -> bool:
+    def has_button(self, button: ButtonHandle | str) -> bool:
         """Returns true if the indicated button is in the set of buttons being
         monitored, false otherwise.
         """
-    def remove_button(self, button: ButtonHandle | int | str) -> bool:
+    def remove_button(self, button: ButtonHandle | str) -> bool:
         """Removes the indicated button from the set of buttons being monitored.
         Returns true if the button was removed, false if it was not being monitored
         in the first place.
 
         Unlike the other methods, you cannot remove a button by removing its alias;
         you have to remove exactly the button itself.
         """
@@ -2875,21 +2876,21 @@
         (e.g.  the number of buttons passed to add_button()).
         """
     def get_button(self, index: int) -> ButtonHandle:
         """Returns the nth button that the ModifierButtons object is monitoring (the
         nth button passed to add_button()).  This must be in the range 0 <= index <
         get_num_buttons().
         """
-    def button_down(self, button: ButtonHandle | int | str) -> bool:
+    def button_down(self, button: ButtonHandle | str) -> bool:
         """Records that a particular button has been pressed.  If the given button is
         one of the buttons that is currently being monitored, this will update the
         internal state appropriately; otherwise, it will do nothing.  Returns true
         if the button is one that was monitored, or false otherwise.
         """
-    def button_up(self, button: ButtonHandle | int | str) -> bool:
+    def button_up(self, button: ButtonHandle | str) -> bool:
         """Records that a particular button has been released.  If the given button is
         one of the buttons that is currently being monitored, this will update the
         internal state appropriately; otherwise, it will do nothing.  Returns true
         if the button is one that was monitored, or false otherwise.
         """
     def all_buttons_up(self) -> None:
         """Marks all monitored buttons as being in the "up" state."""
@@ -2981,15 +2982,15 @@
         """
     @staticmethod
     def wheel_right() -> ButtonHandle:
         """Returns the ButtonHandle generated when the mouse is scrolled to the right.
         Usually, you'll only find the horizontal scroll on laptops.
         """
     @staticmethod
-    def is_mouse_button(button: ButtonHandle | int | str) -> bool:
+    def is_mouse_button(button: ButtonHandle | str) -> bool:
         """Returns true if the indicated ButtonHandle is a mouse button, false if it
         is some other kind of button.
         """
     wheelUp = wheel_up
     wheelDown = wheel_down
     wheelLeft = wheel_left
     wheelRight = wheel_right
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_recorder.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_recorder.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_text.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_text.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/core/_tform.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/core/_tform.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -225,51 +225,51 @@
         buttons should be processed.  See add_throw_button().
         """
     def get_throw_buttons_active(self) -> bool:
         """Returns the flag that indicates whether the ButtonThrower will only process
         events for the explicitly named buttons or not.  See
         set_throw_buttons_active().
         """
-    def add_throw_button(self, mods: ModifierButtons, button: ButtonHandle | int | str) -> bool:
+    def add_throw_button(self, mods: ModifierButtons, button: ButtonHandle | str) -> bool:
         """Adds a new button to the set of buttons that the ButtonThrower explicitly
         processes.
 
         If set_throw_buttons_active is false (which is the default), the
         ButtonThrower will process all buttons.  Otherwise, the ButtonThrower will
         only process events for the button(s) explicitly named by this function;
         buttons not on the list will be ignored by this object and passed on
         downstream to the child node(s) in the data graph.  A button that *is* on
         the list will be processed by the ButtonThrower and not passed on to the
         child node(s).
 
         The return value is true if the button is added, or false if it was already
         in the set.
         """
-    def remove_throw_button(self, mods: ModifierButtons, button: ButtonHandle | int | str) -> bool:
+    def remove_throw_button(self, mods: ModifierButtons, button: ButtonHandle | str) -> bool:
         """Removes the indicated button from the set of buttons that the ButtonThrower
         explicitly processes.  See add_throw_button().
 
         The return value is true if the button is removed, or false if it was not
         on the set.
         """
     @overload
-    def has_throw_button(self, button: ButtonHandle | int | str) -> bool:
+    def has_throw_button(self, button: ButtonHandle | str) -> bool:
         """`(self, button: ButtonHandle)`:
         Returns true if the indicated button, in conjunction with any nonspecified
         modifier buttons, is on the set of buttons that will be processed by the
         ButtonThrower.  That is to say, returns true if this button was ever passed
         as the second parameter add_throw_button(), regardless of what the first
         parameter was.
 
         `(self, mods: ModifierButtons, button: ButtonHandle)`:
         Returns true if the indicated button is on the set of buttons that will be
         processed by the ButtonThrower, false otherwise.  See add_throw_button().
         """
     @overload
-    def has_throw_button(self, mods: ModifierButtons, button: ButtonHandle | int | str) -> bool: ...
+    def has_throw_button(self, mods: ModifierButtons, button: ButtonHandle | str) -> bool: ...
     def clear_throw_buttons(self) -> None:
         """Empties the set of buttons that were added via add_throw_button().  See
         add_throw_button().
         """
     def get_parameters(self) -> tuple[EventParameter, ...]: ...
     setButtonDownEvent = set_button_down_event
     getButtonDownEvent = get_button_down_event
@@ -313,21 +313,21 @@
     It collects together some common interface; in particular, the
     require_button() and related methods.
     """
 
     def __init__(self, __param0: MouseInterfaceNode) -> None: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
-    def require_button(self, button: ButtonHandle | int | str, is_down: bool) -> None:
+    def require_button(self, button: ButtonHandle | str, is_down: bool) -> None:
         """Indicates that the indicated button must be in the required state (either
         up or down) in order for this particular MouseInterfaceNode to do anything.
         For instance, this may be called to make a Trackball object respect mouse
         input only when the control key is held down.
         """
-    def clear_button(self, button: ButtonHandle | int | str) -> None:
+    def clear_button(self, button: ButtonHandle | str) -> None:
         """Removes any requirement on the indicated button set by an earlier call to
         require_button().
         """
     def clear_all_buttons(self) -> None:
         """Removes all requirements on buttons set by an earlier call to
         require_button().
         """
@@ -854,15 +854,15 @@
 
         `(self, x: float, y: float)`:
         Returns the smallest region the indicated point is over, or NULL if it is
         over no region.
         """
     @overload
     def get_over_region(self, x: float, y: float) -> MouseWatcherRegion: ...
-    def is_button_down(self, button: ButtonHandle | int | str) -> bool:
+    def is_button_down(self, button: ButtonHandle | str) -> bool:
         """Returns true if the indicated button is currently being held down, false
         otherwise.
         """
     def set_button_down_pattern(self, pattern: str) -> None:
         """Sets the pattern string that indicates how the event names are generated
         when a button is depressed.  This is a string that may contain any of the
         following:
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_dcparser.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_dcparser.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_deadrec.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_deadrec.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_distributed.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_distributed.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, ClassVar
-from typing_extensions import Literal, Self
+from typing_extensions import Self
 
 from panda3d._typing import URL
 from panda3d.core._downloader import HTTPChannel, SocketStream
 from panda3d.core._express import Datagram, DatagramIterator
 from panda3d.core._nativenet import Buffered_DatagramConnection
 from panda3d.core._net import ConnectionWriter, QueuedConnectionManager, QueuedConnectionReader
 from panda3d.core._pgraph import NodePath
@@ -51,15 +51,15 @@
         datagrams, regardless of message type, are passed up to Python for
         processing.
 
         The CMU distributed-object implementation requires this to be set false.
         """
     def get_handle_datagrams_internally(self) -> bool:
         """Returns the handle_datagrams_internally flag."""
-    def set_tcp_header_size(self, tcp_header_size: Literal[0, 2, 4]) -> None:
+    def set_tcp_header_size(self, tcp_header_size: int) -> None:
         """Sets the header size of TCP packets.  At the present, legal values for this
         are 0, 2, or 4; this specifies the number of bytes to use encode the
         datagram length at the start of each TCP datagram.  Sender and receiver
         must independently agree on this.
         """
     def get_tcp_header_size(self) -> int:
         """Returns the current setting of TCP header size.  See set_tcp_header_size()."""
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_interval.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_interval.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_motiontrail.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_motiontrail.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/direct/_showbase.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/direct/_showbase.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/egg/_egg.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/egg/_egg.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1219,16 +1219,20 @@
     def __init__(self, copy: EggVertexPool) -> None:
         """Copying a vertex pool is of questionable value, since it will copy all of
         the vertices and assign new pointers to them all.  There will be no
         polygons referring to the new vertices.
         """
     @overload
     def __init__(self, name: str) -> None: ...
-    def __getitem__(self, index: int) -> EggVertex: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, index: int) -> EggVertex:
+        """Returns the vertex in the pool with the indicated index number, or NULL if
+        no vertices have that index number.
+        """
+    def __len__(self) -> int:
+        """Returns the number of vertices in the pool."""
     def __iter__(self) -> Iterator[EggVertex]: ...  # Doesn't actually exist
     def has_vertex(self, index: int) -> bool:
         """Returns true if the indicated vertex has been defined in the vertex pool,
         false otherwise.  This does not include forward references.
         """
     def has_forward_vertices(self) -> bool:
         """Returns true if any vertices in the pool are undefined forward-reference
@@ -1413,15 +1417,16 @@
     VMUnspecified: Final = 0
     VM_hidden: Final = 1
     VMHidden: Final = 1
     VM_normal: Final = 2
     VMNormal: Final = 2
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: EggRenderMode = ...) -> None: ...
-    def __eq__(self, __other: object) -> bool: ...
+    def __eq__(self, __other: object) -> bool:
+        """Comparison operators are handy."""
     def __ne__(self, __other: object) -> bool: ...
     def __lt__(self, other: EggRenderMode) -> bool: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def assign(self, copy: Self) -> Self: ...
     def write(self, out: ostream, indent_level: int) -> None:
         """Writes the attributes to the indicated output stream in Egg format."""
@@ -2977,15 +2982,15 @@
         """Returns true if a texcoord name has been explicitly specified for this
         texture, false otherwise.
         """
     def get_uv_name(self) -> str:
         """Returns the texcoord name that has been specified for this texture, or the
         empty string if no texcoord name has explicitly been specified.
         """
-    def set_rgb_scale(self, rgb_scale: Literal[1, 2, 4]) -> None:
+    def set_rgb_scale(self, rgb_scale: int) -> None:
         """Sets an additional factor that will scale all three r, g, b components
         after the texture has been applied.  This is used only when a combine mode
         is in effect.
 
         The only legal values are 1, 2, or 4.
         """
     def clear_rgb_scale(self) -> None:
@@ -2996,15 +3001,15 @@
         """Returns true if an rgb_scale has been specified for the texture, false
         otherwise.
         """
     def get_rgb_scale(self) -> int:
         """Returns the rgb_scale value that has been specified for the texture, or 1
         if no rgb_scale value has been specified.
         """
-    def set_alpha_scale(self, alpha_scale: Literal[1, 2, 4]) -> None:
+    def set_alpha_scale(self, alpha_scale: int) -> None:
         """Sets an additional factor that will scale the alpha component after the
         texture has been applied.  This is used only when a combine mode is in
         effect.
 
         The only legal values are 1, 2, or 4.
         """
     def clear_alpha_scale(self) -> None:
@@ -4750,16 +4755,18 @@
     """This is a collection of textures by TRef name.  It can extract the textures
     from an egg file and sort them all together; it can also manage the
     creation of unique textures and the assignment of unique TRef names.
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: EggTextureCollection = ...) -> None: ...
-    def __getitem__(self, n: int) -> EggTexture: ...
-    def __len__(self) -> int: ...
+    def __getitem__(self, n: int) -> EggTexture:
+        """Returns the nth EggTexture in the collection."""
+    def __len__(self) -> int:
+        """Returns the number of EggTextures in the collection."""
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[EggTexture]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def clear(self) -> None:
         """Removes all textures from the collection."""
     def extract_textures(self, node: EggGroupNode) -> int:
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/egg/_egg2pg.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/egg/_egg2pg.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/fx.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/fx.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/interrogatedb.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/interrogatedb.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/ode.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/ode.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1167,15 +1167,18 @@
     getParamStopERP = get_param_stop_ERP
     getParamStopCFM = get_param_stop_CFM
 
 class OdeJointCollection:
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: OdeJointCollection = ...) -> None: ...
     def __getitem__(self, index: int) -> OdeJoint: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of joints in the collection.  This is the same thing as
+        get_num_joints().
+        """
     def __iadd__(self, other: OdeJointCollection) -> Self: ...
     def __add__(self, other: OdeJointCollection) -> OdeJointCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[OdeJoint]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_joint(self, joint: OdeJoint) -> None: ...
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/physics/_particlesystem.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/physics/_particlesystem.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/physics/_physics.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/physics/_physics.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,18 @@
     """This is a set of zero or more PhysicsObjects.  It's handy for returning
     from functions that need to return multiple PhysicsObjects.
     """
 
     DtoolClassDict: ClassVar[dict[str, Any]]
     def __init__(self, copy: PhysicsObjectCollection = ...) -> None: ...
     def __getitem__(self, index: int) -> PhysicsObject: ...
-    def __len__(self) -> int: ...
+    def __len__(self) -> int:
+        """Returns the number of physics objects in the collection.  This is the same
+        thing as get_num_physics_objects().
+        """
     def __iadd__(self, other: PhysicsObjectCollection) -> Self: ...
     def __add__(self, other: PhysicsObjectCollection) -> PhysicsObjectCollection: ...
     def __copy__(self) -> Self: ...
     def __deepcopy__(self, __memo: object) -> Self: ...
     def __iter__(self) -> Iterator[PhysicsObject]: ...  # Doesn't actually exist
     def assign(self, copy: Self) -> Self: ...
     def add_physics_object(self, physics_object: PhysicsObject) -> None:
```

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/skel.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/skel.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/vision.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/vision.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/panda3d-stubs/vrpn.pyi` & `types-panda3d-0.3.3/src/panda3d-stubs/vrpn.pyi`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/src/types_panda3d.egg-info/PKG-INFO` & `types-panda3d-0.3.3/src/types_panda3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-panda3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: Type stubs for the Panda3D Python bindings
 Author: W. M. Okiishi
 License: Copyright (c) 2022 W. M. Okiishi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `types-panda3d-0.3.2/src/types_panda3d.egg-info/SOURCES.txt` & `types-panda3d-0.3.3/src/types_panda3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `types-panda3d-0.3.2/tests/test_stubtest.py` & `types-panda3d-0.3.3/tests/test_stubtest.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,74 +4,66 @@
 from collections.abc import Container, Sequence
 from importlib.abc import Loader, MetaPathFinder
 from importlib.machinery import ModuleSpec
 from importlib.util import spec_from_loader
 from pathlib import Path
 from types import ModuleType
 
+import attrs
 import mypy.stubtest
 
 
+@attrs.define
 class NonExecutingLoader(Loader):
     """This `Loader` skips execution of the module's contents."""
-    __slots__ = ()
 
     def exec_module(self, module: ModuleType) -> None:
         pass
 
 
+@attrs.define
 class PathFilter(MetaPathFinder):
     """This `MetaPathFinder` can be used to prevent
     certain scripts from running when loaded.
     """
-    __slots__ = 'modules'
     modules: Container[str]
 
-    def __init__(self, modules: Container[str]) -> None:
-        self.modules = modules
-
     def find_spec(
             self,
             fullname: str,
-            path: Sequence[str | bytes] | None,
+            path: Sequence[str] | None,
             target: ModuleType | None = None) -> ModuleSpec | None:
         if fullname in self.modules:
             return spec_from_loader(fullname, NonExecutingLoader())
         else:
             return None
 
 
-def prevent_running(names: Container[str], *, index: int = 2) -> None:
-    """Prevent scripts with names in `names` from running when imported."""
-    sys.meta_path.insert(index, PathFilter(names))
-
-
 def main() -> int:
-    allowlists = [Path('allowlists', 'common.txt')]
-    version_allowlist = Path(
-        'allowlists',
-        f'py{sys.version_info.major}{sys.version_info.minor}.txt'
-    )
-    platform_allowlist = Path('allowlists', f'{sys.platform}.txt')
-    if version_allowlist.exists():
-        allowlists.append(version_allowlist)
-    if platform_allowlist.exists():
-        allowlists.append(platform_allowlist)
-    args = ['panda3d', 'direct', '--mypy-config-file', '../pyproject.toml']
-    for allowlist in allowlists:
-        args += [
-            '--allowlist',
-            str(allowlist),
-        ]
-    print('Stubtest arguments:', ' '.join(args), file=sys.stderr)
+    root = Path(__file__).parent.parent
+    allowlist_names = [
+        'common',
+        f'py{sys.version_info.major}{sys.version_info.minor}',
+        sys.platform,
+    ]
+    args = [
+        'panda3d', 'direct',
+        '--mypy-config-file',
+        str(root / 'pyproject.toml'),
+    ]
+    for name in allowlist_names:
+        path = root / 'tests' / 'allowlists' / f'{name}.txt'
+        if path.exists():
+            args += ['--allowlist', str(path)]
+            print('Using allowlist', repr(str(path)), file=sys.stderr)
     # These scripts run on import, interfering with the tests
-    prevent_running({
+    sys.meta_path.insert(2, PathFilter({
         'direct.directbase.ThreeUpStart',
         'direct.directbase.TestStart',
         'direct.directutil.MemoryLeakHelpers',
-    })
+    }))
     sys.argv += args
     return mypy.stubtest.main()
 
 
 if __name__ == '__main__':
     sys.exit(main())
```

