[![Discord - AudioLink Discord](https://img.shields.io/badge/Discord-AudioLink_Discord-7289da?logo=discord&logoColor=7289da)](https://discord.gg/d5wjNwZBR3) [![Website - AudioLink Website](https://img.shields.io/badge/Website-AudioLink_Website-7289da)](https://audiolink.dev/)

# Unity AudioLink

AudioLink is a system that analyzes and processes in-world audio into many different highly reactive data streams and exposes the data to VRChat Udon, world shaders, and avatar shaders. This fork works universally for avatar shaders.

The per-frequency audio amplitude data is first read briefly into Udon using Unity's GetOutputData. It is then sent to the GPU for signal processing and buffered into a CustomRenderTexture. Then, the CustomRenderTexture is broadcast globally (called `_AudioTexture`) which can be picked up by shaders both in-world and across all avatars.

Should work across all Unity-based games for which AudioLink is developed. Includes avatar shader files only.

### [AudioLink for VRChat worlds](https://github.com/llealloo/vrc-udon-audio-link/releases)
### [AudioLink for ChilloutVR worlds](https://github.com/zLucPlayZ/audio-link-for-cvr/releases)

### [Frequently Asked Questions](FAQ.md)
### [Documentation for shader creators](https://github.com/llealloo/vrc-udon-audio-link/tree/master/Docs)

### For non-game uses
1. Download and Import the latest **UnityPackage** AudioLink Release at https://github.com/llealloo/vrc-udon-audio-link/releases.
2. Open the AudioLink folder and drag the AudioLink prefab into your scene's hierarchy. It should work out of the box.

## Compatible tools / assets
- [Silent Cel Shading Shader](https://gitlab.com/s-ilent/SCSS) by Silent
- [Mochies Unity Shaders](https://github.com/MochiesCode/Mochies-Unity-Shaders/releases) by Mochie
- [Fire Lite](https://discord.gg/24W435s) by Rollthered
- [VR Stage Lighting](https://github.com/AcChosen/VR-Stage-Lighting) by AcChosen
- [Poiyomi Shader](https://poiyomi.com/) by Poiyomi
- [orels1 AudioLink Shader](https://github.com/orels1/orels1-AudioLink-Shader) by orels1
- [VRC Things](https://github.com/PiMaker/VRChatUnityThings) by \_pi\_
- [June Screen FX](https://luka.moe/june.html) by luka
- [ShaderForge-AudioLink](https://github.com/lethanan/ShaderForge-AudioLink) by lethanan
- [AudioLink-USharpVideo-Adapter](https://github.com/Blabzillaweasel/AudioLink-USharpVideo-Adapter/) by Blabz
- [ProTV](https://gitlab.com/techanon/protv) by ArchiTechAnon

## Thank you
- phosphenolic for the math wizardry, conceptual programming, debugging, design help and emotional support!!!
- cnlohr for the help with the new DFT spectrogram and helping to port AudioLink to 100% shader code
- lox9973 for autocorrelator functionality and the inspirational & tangential math help with signal processing
- Texelsaur for the AudioLinkMiniPlayer and support!
- Pema for the help with strengthening the codebase and inspiration!
- 3 for joining the AudioLink team, helping maintain the codebase, and being instrumental in getting version 0.3.0 out.
- Merlin for making UdonSharp and offering many many pointers along the way. Thank you Merlin!
- Orels1 for all of the great help with MaterialPropertyBlocks & shaders and the auto configurator script for easy AV3 local testing
- Xiexe for the help developing and testing
- Thryrallo for the help setting up local AV3 testing functionality
- CyanLaser for making CyanEmu
- Lyuma for helping in many ways and being super nice!
- ACIIL for the named texture check in AudioLink.cginc
- fuopy for being awesome and reflecting great vibes back into this project
- Colonel Cthulu for incepting the idea to make the audio data visible to avatars
- jackiepi for math wizardry, emotional support and inspiration
- Barry and OM3 for stoking my fire!
- Lamp for the awesome example music and inspiration. Follow them!! https://soundcloud.com/lampdx
- Shelter, Loner, Rizumu, and all of the other dance communities in VRChat for making this
- rrazgriz for coming up with and implementing yt-dlp support for editor testing
