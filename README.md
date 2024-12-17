### Best GPU for x86_64 (2010-2020) </br>

### The title of this Repo is "Best GPU for.."
The goal is to find 1x GPU that works in all OS, or most from 2010 to 2020. </br>

most important OS from x86_64 era: </br>
[OSX SnowLeopard 10.6.8](https://en.wikipedia.org/wiki/Mac_OS_X_Snow_Leopard) Server</br>
[OSX Mavericks 10.9.5](https://en.wikipedia.org/wiki/OS_X_Mavericks) </br>
[OSX HighSierra 10.13.6](https://en.wikipedia.org/wiki/MacOS_High_Sierra)  </br>
[OSX Catalina 10.15.7](https://en.wikipedia.org/wiki/MacOS_Catalina) </br>
[Windows 8.1 (2013-2023)](https://en.wikipedia.org/wiki/Windows_8.1) </br>
Ubuntu / Kubuntu 10.04 LTS to 22.04.4 LTS x86_64 or similar .deb </br>

for many Reasons: </br>
OSX SnowLeopard 10.6.8 has [Rosetta](https://en.wikipedia.org/wiki/Rosetta_(software)) PowerPC G4 "emulator" Binary Translation, removed / deleted in OSX Lion 10.7 </br>
OSX Mavericks 10.9.5 is the last OS that works with ProTools HD10.3.10 also has 3rd party USB3.0 drivers for VL800 chip, and old Renesas 200 Firmware, Not compatible in following OSX </br>
OSX HighSierra 10.13.6 is the Peak of 32-Bit & 64-Bit , .3 has Thunderbolt2 eGPU support, .4 removed TB2 eGPU support and added TB3 eGPU support, requires a patch to reactivate TB2 eGPU in .6 </br>
HighSierra also Read/Writes & Format APFS drives, Detects & Boots from M.2 NVMe drives. </br>
[OSX Mojave 10.14](https://en.wikipedia.org/wiki/MacOS_Mojave) removes 32-Bit driver support, still runs some 32-Bit sw like QuickTime required for ProTools & Media composer Video Engine. </br> 
OSX Catalina 10.15.7 is the last 100% intel, 100% 64-Bit, removed 32-Bit completely, preparing for the transition to ARM CPU's </br>
OSX BigSur 11, using a RAM drive of 2GB, and a test file of 1GB in [Black Magic Speed Test](https://apps.apple.com/us/app/blackmagic-disk-speed-test/id425264550?mt=12) or [AJA Speed Test](https://www.aja.com/products/aja-system-test), </br>
BigSur 11 Hybrid Kernel Runs slower on x86_64 vs. OSX Catalina pure x86_64 kernel. </br>
BigSur 11 takes too much time to update from OSX Catalina, and does Not allow to Downgrade. </br>

OSX SnowLeopard 10.6.8 cannot be installed on a Mac newer than 2010 </br>
unless using a Virtual Machine like VMWare Fusion Player 10.2.1 on OSX Catalina </br>

VM does Not have FireWire support, Nor Firewire Pass-through, Nor PCIe Pass-through. </br>
OSX SnowLeopard 10.6.8 cannot be installed on a VM, requires [OSX Server 10.6.8](https://en.wikipedia.org/wiki/Mac_OS_X_Server#Mac_OS_X_Server_10.6_(Snow_Leopard)) </br>
OSX SnowLeopard 10.6.8 is designed for MacPro 5,1 2010 with AMD Radeon HD 5770, HD 5870, HD 7950, GTX Titan 6GB*, K5000*, Quadro 4000* with Optional Drivers. </br>
Runs on MacMini 2010, maybe 2011, 2012 or recent does Not. </br>
MacPro 5,1 2012 requires Firmware downgrade to 2010. </br>
Running a more recent VMWare than >10.2.1 requires OSX BigSur 11 or Newer, but OSX Hybrid Kernel becomes -30% slower on x86_64 </br>

Windows8.1 is similar to OSX HighSierra, the Peak of 32-Bit & 64-Bit. </br>
but Steem, Origin, Ubisoft re-compliled Launchers so it does Not run on Windows8.1 anymore = Gaming on Win8.1x64 is dead, unless its retro gaming like Eduke32 & Free DRM. </br>
games like [Need For Speed - The Run (2011)](https://en.wikipedia.org/wiki/Need_for_Speed%3A_The_Run) wont work, because requires Origin app account, Discontinued and Replaced by EA app, but EA requires W10 or later, in a few years EA will stop working on W10 & will only work in W11. </br>

but still Win8.1 is important for other Win Only software like [Microchip Studio for AVR & SAM Devices 7.0.2594 (2022)](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio) and [older](https://www.microchip.com/en-us/tools-resources/archives/avr-sam-mcus),
for programmers like [STK 600](https://www.microchip.com/en-us/development-tool/ATSTK600), STK500, etc... that require USB drivers. </br>
but if Only requires USB drivers, is better to install Win8.1x64 on a 2-core Virtual Machine with USB pass-through. </br>
[VirtualBox6](https://www.virtualbox.org/wiki/Download_Old_Builds) works well, VirtualBox7 is designed for UEFI, Virtual GPU driver v7 has issues. </br>

## GPU candidates:

AMD latest driver that supports Win8.1 officially was Rx 480, forcing W7x64 driver for Rx 580 may work, but untested, Unofficial. </br>
basically AMD is discarded for Win8.1x64 if want modern 3D Games on Linux. </br>
Rx480 is +50% vs. 1050 Ti, but modern gaming in Windows8.1 is Dead. </br>
Only software like [Unigine Tropics](https://benchmark.unigine.com/tropics) </br>

Nvidia latest GPU that has drivers for Win8.1x64 is RTX 8000, P6000, Titan Xp, M6000 </br>
but... RTX 8000, P6000, Titan Xp does Not work in OSX Mavericks 10.9.5 requires to buy 2x GPUs </br>
or another GPU more compatible. </br>

Windows 8.1 works in [ASRock Z790 LiveMixer](https://www.asrock.com/mb/Intel/Z790%20LiveMixer/Specification.asp) UEFI v9.03 + [ASRock Thunderbolt 4 v1](https://www.asrock.com/mb/spec/product.asp?Model=Thunderbolt%204%20AIC) </br>
Dual Boot: Linux 22.04 LTS & Win8.1 on separate SSD/M.2 </br>
requires a GPU compatible with Windows8.1 </br>
intel iGPU removed Legacy Boot in 12th Gen CPU's, 11th untested, 10th Gen iGPU and older Boot Legacy OS FAT32 500MB partition with BIOS or UEFI, </br>
Win8.1x64 does Not Boot if has Both BIOS & UEFI at same time on the Boot Partition. </br>

having a powerful GPU for Win8.1 is almost pointless because Modern 3D Gaming is Dead in Win8.1 unless its DRM Free like GOG </br>
better to game in Linux using Wine, Codeweavers, Bottles, Proton, PlayOnLinux </br>
but Not everything works in Linux, </br>
for example: </br>
ProTools Ultimate 2020.12 + HDX PCIe + [Razer Core X Chroma](https://egpu.io/best-egpu-buyers-guide/) or similar. </br>
ProTools HD10.3.10 + HD PCI-x or PCI-e + Magma expansion chassis </br>
Matrox MXO2 MAX + Adobe CS6 Media Encoder / Avid Video Engine </br>
imacon Photo / 343 / 646 / 848 / 949 SCSI A-sync scanner + FlexColor v4.0 software </br>
Lynx AES16, RME hdsp 9632 </br>
and others... </br>

some things work 50/50 </br>
example: </br>
ilok VST2 plugins work in Linux IF plugin allows to store license on the Machine, Not USB,</br>
because ilok-USB requires propietary drivers Not available for Linux, but ilok PC licence works on Wine. </br>

Best GPU for Dual Boot: </br>
Low Cost: GT 1050 Ti  </br>
perfect option, has DisplayPort for New Monitors like LG 34GP63A that require DP to run at 160fps, Low power consumption. </br>
Fastest GPU: RTX 8000, P6000, Titan Xp, M6000, </br>
Dual Boot: Win8.1x64 + Linux </br>
to Game on Linux, in Win8.1 a Fast GPU will be overkill, very few software will use it. </br>
Modern / Faster GPU like 4070 or 4070 Super "The best in 200w category for 2024" works on Linux but Not on Win8.1 </br>
requires to turn-off, open the PC, change GPU's & boot in other OS, </br>
or install 2x different GPU's at same time in the same machine,</br>
or purchase Twin machines to have different GPU's & different OS. </br>

OSX SnowLeopard 10.6.8 works with Quadro 4000, K5000, HD 7950, HD 5770, HD 5870, Radeon 6000 series has issues on OSX </br>
OSX Mavericks 10.9.5 works with GTX Titan 6GB / GTX 780 "the same" and M6000 "+50% faster" </br>
GTX Titan Black requires OSX 10.11 or newer </br>
GTX Titan 6GB / GTX 780 are the true sucessor of Nvidia GTX 580 </br> 
GTX 680 series were a dissapointment in my opinion, a cut down version with higher clock to compensate, did Not feel an improvement on games like NFS The Run. </br>
but GTX 680 can be flahsed easy to have EFI and Boot on MAC OSX, same as Radeon HD 7950 </br>
but Radeon HD 7950 does Not work eGPU in OSX, even it works directly on PCIe </br>
OSX Mojave 10.14 and Newer OSX Cata 10.15.7 requires a [Metal Compatible GPU](https://blog.greggant.com/posts/2018/05/07/definitive-mac-pro-upgrade-guide.html#gpuupgrades) </br>

P5000 is +20% faster vs. M6000 but slower vs. Titan X "Maxwell" and slower vs. Titan X "pascal", and slower vs. Titan Xp </br>
the fastest Titan Xp is slower vs. RTX 3070 or newer. </br>

using a GPU compatible with Win8.1 & Linux will Not allow to play modern RayTracing Games like Indiana Jones - The Great Circle (2024) unless its a RTX 8000 </br>
but RTX 8000 wont work in OSX, if also have a Mac Pro 5,1 2010 or a MacPro 6,1 2013 or MacMini 2014 with TB2 eGPU </br> 
Max GPU for OSX HighSierra 10.13.6 is Titan Xp or P6000 </br>
for OSX Catalina 10.15.7 [the list](http://www.macvidcards.com/store/c19/OS_10.15_Catalina_Compatible.html) is reduced, GTX Titan 6GB works but has some issues, better HD 7950 </br>
Best AMD GPU for OSX Catalina is Vega 56. </br>
MacPro 5,1 2010 requires a cable from TeamProfit that converts 2x mini 6-pin GPU to standard 8-pin GPU, some GPU's also require a 1 or 2x SATA ports to 6-pin GPU. </br>
