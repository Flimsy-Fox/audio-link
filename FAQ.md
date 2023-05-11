## **Question**:
Will the AudioLink-enabled shaders on my avatars continue to work in worlds using AudioLink 0.3.0
### **Answer**:
Yes.

## **Question**:
Are shaders written for previous versions of AudioLink usable in projects that use AudioLink 0.3.0?
### **Answer**:
It depends:
- Shaders that include the AudioLink.cginc file to support AudioLink will have to be upgraded. We have included a tool that can do this for you automatically, you can access it via the "Update AudioLink compatible shaders" button in the new AudioLink dropdown in the top menu bar of the Unity editor.
- Shaders that use their own custom code to sample data provided by AudioLink will not have to be changed at all.
If you are unsure which of these applies to a specific shader, ask the author, they should know.

## **Question**:
Are shaders written for AudioLink 0.3.0+ usable in projects that use older versions of AudioLink?
### **Answer**:
No.

## **Question**:
I want to use AudioLink 0.3.0+, but am not interested in VRChat nor ChilloutVR at all. How do I install the standalone version?
### **Answer**:
Download the latest **UnityPackage** AudioLink Release at https://github.com/llealloo/vrc-udon-audio-link/releases, and import as any other unitypackage.

## **Question**:
I am seeing a bunch of errors in the console after installing AudioLink 0.3.0. What do I do?
### **Answer**:
There is known issue where, when first importing AudioLink, error messages will be spammed in the console window. This is harmless and should automatically fix itself. Simply clear the console and proceed as normal.

## **Question**:
I'm having trouble using VR Stage Lighting (VRSL) with AudioLink. Where should I ask for help?
### **Answer**:
https://vrsl.dev/
