## archinstall
Used archinstall script  
Set media server to pipewire  
Set Profile to Minimal  

## hyprland
Laptop with external monitors via USB-C/Thunderbolt dock  
See: https://wiki.hyprland.org/FAQ/#my-external-monitor-is-blank--doesnt-render--receives-no-signal-laptop  
See: https://github.com/hyprwm/Hyprland/issues/7825  
env = AQ_NO_MODIFIERS,1  


Laptop with intel 9th gen CPU and built in GPU  
env = ANV_VIDEO_DECODE,1  
mesa
vulkan-intel
vulkan-tools -> vulkaninfo
intel-media-driver

$browser = google-chrome-stable --enable-features=AcceleratedVideoDecodeLinuxGL
