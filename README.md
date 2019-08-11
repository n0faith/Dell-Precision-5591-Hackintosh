

# macOS Mojave 10.14.6 - Dell Precision 5591 (August 10, 2019)
![Dell Precision 5591](https://i.dell.com/sites/imagecontent/products/PublishingImages/latitude-15-5591-laptop/laptop-latitude-15-5591-mlk-nontouch-notebook-pdp-2.jpg)

## Specs 
- Model : Dell Precision 5591
- Bios: 1.9.0 
- CPU: Intel® Core™ i7-8850H (6 Core - 12 Thread) ~ 2,6 - 4,3Ghz
- GPU: Intel UHD630 1536MB  + NVIDIA GeForce MX130 ( Optimus )
- RAM: 1 x 2667MHz Samsung 16GB Single Channel LPDDR4  
- Display: 15.6 inch 16:9, 1920 x 1080 pixel 141 PPI, multitouch, AU Optronics B156HW03, IPS , glossy 
- Storage: NVME PCIE 3.0 x4 Toshiba XG5 KXG50ZNV512G 512 GB 
- LAN : Intel Ethernet Connection I219-LM (10/100/1000/2500/5000MBit/s) 
- Wireless :  DW1560 
- Bootloader :  Clover_v2.5k_r5033
##  OS 
- Dual boot macOS 10.14.6 + win10 1903 
## What Works
- CPU + IGPU Power Management . 
- Native NVRAM  
- Battery status  
- HDMI 1.4 working on LS mode 
- Sleep and Wake with Lid Open and Close  
- Audio ALC256 ( Speaker + Internal Microphone )
- Combo Jack :  Headphone/Headset with microphone ( Line-in )
- Keyboard with Brightness Audio funtion keys   
- Trackpad / Touchscreen with native gestures  
- WiFi and Bluetooth ( Handoff , Airdrop , Continuity , Instant Hot Spot )
## What Doesn't Work 
- Finger Print Sensor 
- HDMI audio 
- VGA port 
- Nvidia MX130 --> disable via ssdt-ddgpu or -wegnoegpu   
- Trackpad buttons 
- SD Card Reader --> disable in BIOS for save  battery 
## Not tested 
- Combo Thunderbolt + displayport over usb-c + usb-c  
- HDMI 2.0 output 
- Imess , Facetime 
## Bugs  
- Hot plug VGA port reboot  --> don't use 
- Sometime audio not working after sleep/wake --> restart 
- Slow or stuck while booting --> shutdown by press power button , disable  TRIM kext patch in KextsToPatch  (  3rd party nvme, sata ssd TRIM maybe not compatible with native mac TRIM ) 
- Power button led not blink when sleep -->  no solution . 
## Misc  
- Combo jack fix for ALC255/256 --> [hackintosh-stuff](https://github.com/hackintosh-stuff/ComboJack) 
- Modify macOS CPU Performance if your CPU isn't 8870H with [one-key-cpufriend](https://github.com/stevezhengshiqi/one-key-cpufriend/blob/master/README.md)
## Credits
- @Apple for macOS 
- @Acidanthera vit9696 lvs1974 vandroiy2013 PMheart ... for Lilu, AppleALC, VirtualSMC, WhateverGreen, AirportBrcmFixup, BT4LEContinuityFixup 
- @Alexandred and his team for VoodooI2C
- Special thanks: @RehabMan
