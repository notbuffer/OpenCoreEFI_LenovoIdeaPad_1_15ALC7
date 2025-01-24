# OpenCoreEFI of my Lenovo IdeaPad 1 15ALC7 (type 82R4)
## Notes
- Please make your own ProductInfo... info.
- Please do not make issues regarding the EFI folder! This is what works for me, and what works for me, might not work for you. Use Yahoo and Dortania/ChefKissInc guide.
- Please do make issues if you see any issues with the README, or suggestions about kexts, I will update this repository once I edit something.
- Please update the time zone manually using terminal if no Location Services through Terminal.
## Things I MIGHT have to do with this repository
- [ ] Make multiple branches, each for Broadcom, one for Realtek and one for Intel because why not.
      > Probably will only update which one I am currently using though.
## My Laptop Variant (type 82R4)
- AMD Ryzen 5 5500U
- Radeon Vega 7
- 8 GB of RAM (2 GB are dedicated to iGPU)
- Realtek WiFi + Bluetooth RTL8852BE (Unsupported, soon-to-be-replaced with a BCM94352Z)
 > Included fixes for old Broadcom cards, so just use OpenCore Legacy Patcher and you're good to go if you use one of those.
 > Also included the updated HoRNDIS kernel extension for USB Tethering with Android.
- 256 GB M.2 KIOXIA SSD
- 1080p TN 15.6" Display
 > Drivers work fine thanks to NootedRed, except some graphical glitches in AutoCAD and no Chromium/Brave/React/Whatever-other-project-based-on-Blink-and-V8 for sure.
- 42Wh Battery
 > Lasts about 6-7 hours on Windows/Linux, no estimate for macOS as USB Tethering is extremely draining
 > The number might not be accurate, but doesn't really care
- Left side of ports: 1 AC Port, 1 USB-A SuperSpeed port, 1 USB-C SuperSpeed port, 3.5 mm Jack
 > USB-C port only supports being, well, a USB-C port and doesn't charge nor supports displays.
 > 3.5 mm Jack should work but didn't bother testing.
- Right side of ports: 1 USB-A 2.0 port, 1 Realtek SD Card reader, Novo Button
 > The SD Card reader should work fine, added kernel extension for it, didn't test yet.
- Realtek ALC257 and AMD Microphone
 > Realtek Audio uses Layout ID 11 in my case, and I added AMD Microphone kext which seems to work fine.
