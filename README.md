# HTC Vive Pro Eye 2 Connection Guide

Guide to run Unity projects on HTC Vive Pro Eye 2 using the OpenXR (to access Unity's XR GameObjects (such as XRRig).

1. Download the [UltimateXR Package](https://www.ultimatexr.io/) and SteamVR Plugin from the Unity Package Manager (in project).

2. Add the UltimateXR Package to Unity project (Drag the .unitypackage file or Assets -> Import Package -> Custom Package)

3.  In Unity project go to Tools -> UltimateXR -> SDK Manager.

4.  SDK Manager should give an error as "SteamVR actions have not been set up..." if the SteamVR Plugin is installed".

5.  Go to Windows -> SteamVR Input. If you see a warning message as "It looks like your project is missing an actions.json." click "Yes".

6.  Go to the SDK Manager (follow the same path in the step 3) and select "Create Actions".

7.  Go to Edit -> Project Settings -> XR Plug-in Management.

8.  Uncheck the "OpenVR Loader" and make sure that "OpenXR" is checked. There may be a warning icon next to it, it will be fixed in next steps)

9.  Go to the OpenXR section underneath the XR Plug-in Management (Edit -> Project Settings -> XR Plug-in Management -> OpenXR)

10.  On the "Enabled Interaction Profiles" delete all profiles (using the '-' on bottom right) except the "HTC Vive Controller Profile"

11.  Make sure that all features are unchecked (such as "D-Pad Binding" or "Hand Interaction Poses")

12.  Project should run on the VR headset when it is played from the Unity Editor.
