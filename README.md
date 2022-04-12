# UE4 plugin and sample project to receive data from MocapForAll

# How to use

- [How to use in English](https://github.com/Akiya-Research-Institute/MocapForAll-Receiver-Plugin-for-UE4/wiki/How-to-use)  
- [日本語版つかいかた](https://github.com/Akiya-Research-Institute/MocapForAll-Receiver-Plugin-for-UE4/wiki/%E4%BD%BF%E3%81%84%E6%96%B9)

# Quick start

In MocapForAll,
- turn on "Settings > Data export > VMT protocol > Send tracking positions"
- turn off "Settings > Data export > VMT protocol > Send tracking positions > As relative position to HMD"

Make sure
- the port numbers match between MocapForAll and this receiver
- no other application uses the same port

See "Plugins\MocapForAllReceiver\Content\Sample" for exaplmes:
- "BP_Sample1_TransformCubes" shows how to get transforms of tracking points from the OSC messages.
- "BP_Sample2_TrackerToControlRig_MetaHumanPreview" shows how to animate a MetaHuman using the transforms of tracking points. Note that you need to import MetaHuman to use this.
- "BP_Sample3_TrackerToControlRig_VRM" is an example to show how to animate a VRM using the transforms of tracking points. Note that you need to install [VRM4U](https://github.com/ruyo/VRM4U) plugin to use this.
- "BP_Sample4_TrackerToControlRig_Mannequin" shows how to animate UE Mannequin using the transforms of tracking points. Note that you need to import UE Mannequin from Third-person template to use this.

# Third party license notice

This repository uses the following open source software:

- [VRM4U](https://github.com/ruyo/VRM4U) created by ruyo
