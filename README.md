## archinstall
Used archinstall script  
Set media server to pipewire  
Set Profile to Minimal  

## hyprland
### Laptop with external monitors via USB-C/Thunderbolt dock  
See: https://wiki.hyprland.org/FAQ/#my-external-monitor-is-blank--doesnt-render--receives-no-signal-laptop  
See: https://github.com/hyprwm/Hyprland/issues/7825  
env = AQ_NO_MODIFIERS,1  


### Laptop with intel 9th gen CPU and built in GPU
See: https://wiki.archlinux.org/title/Intel_graphics     
See: https://wiki.archlinux.org/title/Hardware_video_acceleration  
env = ANV_VIDEO_DECODE,1  
mesa
vulkan-intel
vulkan-tools -> vulkaninfo | grep VK_KHR_video_   
libav-utils -> vainfo:w
intel-media-driver

### Chrome
See: https://wiki.archlinux.org/title/Chromium#Hardware_video_acceleration  
$browser = google-chrome-stable --enable-features=AcceleratedVideoDecodeLinuxGL  
intel-gpu-tools -> intel_gpu_top
