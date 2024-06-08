## HTC Vive Pro Eye 2 Unity Connection Guide

Guide to running Unity projects on HTC Vive Pro Eye 2 using the OpenXR (to access Unity's XR GameObjects (such as XRRig).

1. Download the [UltimateXR Package](https://www.ultimatexr.io/) and SteamVR Plugin from the Unity Package Manager (in the project).

2. Add the UltimateXR Package to the Unity project (Drag the .unitypackage file or Assets -> Import Package -> Custom Package)

3.  In Unity project go to Tools -> UltimateXR -> SDK Manager.

4.  SDK Manager should give an error as "SteamVR actions have not been set up..." if the SteamVR Plugin is installed".

5.  Go to Windows -> SteamVR Input. If you see a warning message as "It looks like your project is missing an actions.json." click "Yes".

6.  Go to the SDK Manager (follow the same path in step 3) and select "Create Actions".

7.  Go to Edit -> Project Settings -> XR Plug-in Management.

8.  Uncheck the "OpenVR Loader" and make sure that "OpenXR" is checked. There may be a warning icon next to it, it will be fixed in the next steps)

9.  Go to the OpenXR section underneath the XR Plug-in Management (Edit -> Project Settings -> XR Plug-in Management -> OpenXR)

10.  On the "Enabled Interaction Profiles" delete all profiles (using the '-' on the bottom right) except the "HTC Vive Controller Profile"

11.  Make sure that all features are unchecked (such as "D-Pad Binding" or "Hand Interaction Poses")

12.  The project should run on the VR headset when it is played from the Unity Editor.

## HTC Vive Pro Eye 2 Eye Tracker Unity Connection Guide

 1. Use [this link](https://developer.vive.com/resources/vive-sense/eye-and-facial-tracking-sdk/download/latest/) to download the SDK for the Eye Tracking.

 2. Go to SDK -> 02_Unity and extract the "Vive-SRanipal-Unity-Plugin.unitypackage" and import to the Unity project (as in the 2nd step of HTC Vive Pro Eye 2 Unity Connection Guide).

 3. Add the prefabs "Gaze Ray Sample" and "SRanipal Eye Framework" in the folder ViveSR -> Prefabs to the hierarchy.

 4. You should see a line that follows the gaze in play mode.

## Additional Notes

* To run the headset on a 120 Hz refresh rate, the computer's graphics card should be DSC capable according to [this link](https://www.vive.com/us/support/vive-pro2/category_howto/how-to-enable-full-resolution.html).
