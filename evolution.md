# 16-May-2024

Source:-
- Initial update for EvolutionX v9.0 based on lineage.

Device:-
- Introduced Xiaomi parts 
- dropped oneplus Dolby and Introduce Dolby Atmos as part
- Shipped with Leica camera as default camera 
- Fixed audio distortion issue completely
- audio: Imported SpatialAudio support
- audio: Use QCOM implementation for audio effects
- audio: Enable 24-bit support for wired headphones
- overlay: Optimize statusbar paddings  
- overlay: Disable alpha compositing in WM
- props: better RAM management
- props: Disable QTI perf lock usage in camera HAL
- props: Enable adb on boot
- sepolicy: addressed various denials 
-  Import powerhint.json from coral and adapted it for yupi
- Upsteamed kernelSU to the latest version, download<a href="https://github.com/tiann/KernelSU/releases/download/v0.9.2/KernelSU_v0.9.2_11682-release.apk"> kernelSU</a> manager.
- There are more device side changes but most of you will not understand those changes terms so i am not mentioning those changes.