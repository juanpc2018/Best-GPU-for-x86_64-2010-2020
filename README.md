### Best GPU for x86_64 (2010-2020) </br>

### The title of this Repo is "Best GPU for.."
The goal is to find 1x GPU that works in all OS, or most OS from 2010 to 2020. </br>

most important OS from x86_64 era: </br>
[OSX SnowLeopard 10.6.8](https://en.wikipedia.org/wiki/Mac_OS_X_Snow_Leopard) [Server](https://en.wikipedia.org/wiki/Mac_OS_X_Server#Mac_OS_X_Server_10.6_(Snow_Leopard)) </br>
[OSX Mavericks 10.9.5](https://en.wikipedia.org/wiki/OS_X_Mavericks) </br>
[OSX HighSierra 10.13.6](https://en.wikipedia.org/wiki/MacOS_High_Sierra)  </br>
[OSX Catalina 10.15.7](https://en.wikipedia.org/wiki/MacOS_Catalina) </br>
[Windows 8.1 (2013-2023)](https://en.wikipedia.org/wiki/Windows_8.1) </br>
Ubuntu / Kubuntu 10.04 LTS to 22.04.4 LTS x86_64 or similar .deb </br>

many Reasons: </br>
OSX SnowLeopard 10.6.8 has [Rosetta](https://en.wikipedia.org/wiki/Rosetta_(software)) PowerPC G4 "emulator" Binary Translation, removed / deleted in OSX Lion 10.7 </br>
OSX Mavericks 10.9.5 is the last OS that works with ProTools HD10.3.10 also has 3rd party USB3.0 drivers for VL800 chip, and old Renesas 200 Firmware, drivers are Not compatible in next OSX </br>
OSX HighSierra 10.13.6 is the Peak of 32-Bit & 64-Bit , .3 has Thunderbolt2 eGPU support, .4 removed TB2 eGPU support and added TB3 eGPU support, requires a patch to reactivate TB2 eGPU in .6 </br>
HighSierra Read/Writes & Format APFS drives, Detects & Boots from M.2 NVMe drives. </br>
OSX Mavericks 10.9.5 Only works with M.2 AHCI, Not M.2 NVMe. </br>
[OSX Mojave 10.14](https://en.wikipedia.org/wiki/MacOS_Mojave) removes 32-Bit driver support, still runs some 32-Bit sw like QuickTime, required for ProTools & Media composer Video Engine. </br> 
OSX Catalina 10.15.7 is the last 100% intel, 100% 64-Bit, removed 32-Bit completely, preparing for the transition to ARM CPU's </br>
OSX BigSur 11, using a RAM drive of 2GB, and a test file of 1GB in [Black Magic Speed Test](https://apps.apple.com/us/app/blackmagic-disk-speed-test/id425264550?mt=12) or [AJA Speed Test](https://www.aja.com/products/aja-system-test), </br>
BigSur Hybrid Kernel Runs slower on x86_64 vs. OSX Catalina pure x86_64 kernel. </br>
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

but still Win8.1 is important for other "Win Only" software like [Microchip Studio for AVR & SAM Devices 7.0.2594 (2022)](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio) and [older](https://www.microchip.com/en-us/tools-resources/archives/avr-sam-mcus),
for programmers like [STK 600](https://www.microchip.com/en-us/development-tool/ATSTK600), STK500, etc... that require USB drivers. </br>
but if Only requires USB drivers, is better to install Win8.1x64 on a 2-core Virtual Machine with USB pass-through. </br>
[VirtualBox6](https://www.virtualbox.org/wiki/Download_Old_Builds) works well, VirtualBox7 is designed for UEFI, Virtual GPU driver v7 has issues. </br>

### GPU candidates:

AMD latest driver that supports Win8.1 officially was Rx 480, forcing W7x64 driver for Rx 580 may work, but untested, Unofficial. </br>
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

OSX Cata 10.15.7 is limited to intel 8th Gen CPU's on MacMini 2018 [i7-8700B](https://www.cpu-monkey.com/en/compare_cpu-intel_core_i7_8700b-vs-intel_core_i5_12400) or [MacPro 2019](https://www.cpu-monkey.com/en/compare_cpu-intel_xeon_w_3275m-vs-intel_core_i9_12900ks) </br>
Macs are limited to run [T2 Linux](https://wiki.t2linux.org/) Not to be confused with [T2 SDE](https://t2sde.org/)
same as M1/2/3 Macs are limited to [Asahi Linux](https://asahilinux.org/)

having a powerful GPU for Win8.1 is almost pointless because Modern 3D Gaming is Dead in Win8.1 unless its DRM Free like [GOG](https://www.gog.com/en/) </br>
better to game in Linux using Wine, Codeweavers, Bottles, Proton, PlayOnLinux </br>
but Not everything works on Linux, </br>
for example: </br>
ProTools Ultimate [2020.12](https://avidtech.my.salesforce-sites.com/pkb/articles/en_US/Compatibility/Pro-Tools-Operating-System-Compatibility-Chart) + HDX PCIe + [Razer Core X Chroma](https://egpu.io/best-egpu-buyers-guide/) or similar. </br>
ProTools HD10.3.10 + HD PCI-x or PCI-e + Magma expansion chassis </br>
Matrox MXO2 MAX + Adobe CS6 Media Encoder / Avid Video Engine </br>
imacon Photo / 343 / 646 / 848 / 949 SCSI Async scanner + FlexColor v4.0 software </br>
Lynx AES16, RME hdsp 9632 </br>
[Autodesk DWG Trueview (2015-2020)](https://www.filehorse.com/download-autodesk-dwg-trueview/old-versions/) </br>
[Rhino 3D 7](https://www.rhino3d.com/7/system-requirements/)/[6](https://www.rhino3d.com/6/system-requirements/)/[5](https://www.rhino3d.com/5/system-requirements/) </br>
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
Recomended to install [CUDA-Z](https://cuda-z.sourceforge.net/) to test if driver has CUDA 64-Bit working </br>
for example: GTX Titan 6GB requires [driver 388.71](https://www.nvidia.com/en-us/drivers/details/128447/), Newer driver install, but does Not have CUDA 64-Bit, its Disabled in Newer drivers. </br>

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
most NVIDIA GPU's are Metal Compatible but OSX deleted driver support for most NVIDIA GPU's in OSX Mojave & Catalina. </br>
most NVIDIA GPU's only go up to OSX HighSierra 10.13.6 </br>
AMD works better on OSX Catalina and older. </br>
OSX deleted all AMD & NVIDIA GPU support / drivers for [M2 Mac Pro 2023](https://en.wikipedia.org/wiki/Mac_Pro#Apple_silicon_(2023)) with [OSX Ventura 13.4](https://www.youtube.com/watch?v=OtcSNiU9Zb8&t=799s) </br>

P5000 is +20% faster vs. M6000 but slower vs. Titan X "Maxwell" and slower vs. Titan X "pascal", and slower vs. Titan Xp </br>
the fastest Titan Xp is slower vs. RTX 3070 or newer. </br>
for modern gaming only: purchasing a Non-RayTracing capable GPU is wasting money. </br>
M6000 is older "more compatible" but there is 12GB and 24GB versions, 24GB is Newer "less wide compatible between multiple OS". </br>
RTX 8000 is a Good option for Modern Gaming on Linux & Dual Boot on Windows8.1 but incompatible with older OSX </br>
GTX Titan 6GB is older "more compatible" but.. </br>
Titan Xp has Newer drivers for Windows8.1 vs. RTX 8000, P6000 & M6000, is compatible with OSX HighSierra 10.13.6, OSX eGPU, but is useless for modern gaming, Untested with older OSX, probably Not compatible. </br>

using a GPU compatible with Win8.1 + Linux + OSX does Not allow to play modern RayTracing Games like Indiana Jones - The Great Circle (2024) unless its a RTX 8000 </br>
RTX 8000 wont work in OSX + Mac Pro 5,1 2010 or a MacPro 6,1 2013 or MacMini 2014 + TB2 eGPU + Apple TB2 to TB3 converter. </br> 
Max GPU for OSX HighSierra 10.13.6 is Titan Xp or P6000 </br>
OSX Catalina 10.15.7 [list](http://www.macvidcards.com/store/c19/OS_10.15_Catalina_Compatible.html) is reduced, </br>
GTX Titan 6GB works in OSX but has issues, for OSX is better HD 7950 but HD 7950 does Not work eGPU in OSX </br>
Best AMD GPU for OSX Catalina is Vega 56, "64 & Frontier Untested" </br>
Radeon VII was the best for OSX but many failed with Error 32 "Broken Memory" cannot be repaired, its SMB on the same GPU die. </br>
MacPro 5,1 2010 requires a cable from TeamProfit that converts 2x mini 6-pin GPU to standard 8-pin GPU, some GPU's also require a 1 or 2x SATA ports to 6-pin GPU. </br>

### so far:  </br>
1x GPU that does all is complicated. </br>
2x GPU's: 
RTX 8000 + Radeon HD 7950 gives broad compatibility between different OS. </br>
3x or more GPU's allows to optimize individually for each OS case/scenario. </br>
[Thunderbolt](https://egpu.io/best-egpu-buyers-guide/) allows to swap GPU's much faster on any machine, </br>
but HD 7950 does Not work eGPU in OSX HighSierra 10.13.1-3 </br>
Thunderbolt1 is available since [OSX Lion 10.7 / 2011 Macs](https://en.wikipedia.org/wiki/Mac_Mini#Technical_specifications_3) </br>
Thunderbolt2 is available since MacMini 2014 or [MacPro 6,1 2013](https://en.wikipedia.org/wiki/Mac_Pro#Specifications_2) </br>
Thunderbolt3/4 "Alpine/Titan/Maple Ridge" add-on card with Intel DSL6540 / DSL7540 / JHL8540 controller won't work in older OSX Mavericks 10.9.5 </br>
MacPro 5,1 2010 would require a [Thunderbolt2](https://www.asrock.com/mb/spec/card.asp?Model=Thunderbolt%202%20AIC) "Falcon Ridge" card with Intel DSL5320 Controller + Hacks, Untested. </br>

#### OSX SnowLeopard 10.6.8 requires: </br>

clean install: [Mac 2008-2011](https://en.wikipedia.org/wiki/Mac_OS_X_Snow_Leopard#64-bit_architecture) + [GPU's](https://web.archive.org/web/20090831083420/http://www.apple.com/macosx/specs.html): </br>
    NVIDIA GeForce 9400M / 9600M GT / 8600M GT, GT 120 / GT 130, GTX 285, 8800 GT / GS, Quadro FX 4800 / FX5600, Radeon 4850 / 4870 / 5770 / 5870 </br>
HD 7950 does Not require drivers in OSX 10.6.8 but clean install OSX 10.6.3 / 10.6.4 DVD Untested </br>
VM or OSX 10.6.7 iso DVD with more modern GPU drivers. </br>
NVIDIA Quadro 4000 works in OSX SnowLeopard with optional Drivers in PCIe "eGPU untested", K5000, GTX Titan 6GB, GTX 780 Untested. </br>
R9 290 / 290x / 280 / 280x / 270x / 270 could be an alternative to HD 7950, Untested. </br>

#### OSX Mavericks 10.9.5 requires: </br>

[Quadro 4000](https://www.nvidia.com/content/dam/en-zz/Solutions/design-visualization/quadro-product-literature/NV_DS_QUADRO_4000_forMac_A4_NV_LR.pdf) </br>
HD 5770* </br>
Quadro K620 </br>
HD 5870 </br>
R9 270x </br>
HD 7950 </br>
R9 280x some work flashed </br>
HD 7970 some work flashed </br>
GTX Titan 6GB° Non-Black </br>
GTX 970 </br>
[Quadro M6000 12GB (2015)](https://www.nvidia.com/content/dam/en-zz/Solutions/design-visualization/quadro-product-literature/11305_NV_DS_Quadro_M6000_FEB15_NV_US_FNL_HR.pdf) </br>
[Quadro M6000 24GB (2016)](https://www.nvidia.com/content/dam/en-zz/Solutions/design-visualization/quadro-product-literature/NV-DS-Quadro-M6000-24GB-US-NV-fnl-HR.pdf) Unknown </br>

*Radeon HD 5770 stops working in OSX HighSierra 10.13.6 </br>
does Not work at 60fps has issues / glitches, only works at 30fps or older OSX. </br>
°GTX Titan 6GB does Not work well on OSX, has issues with some 32-Bit aps, and some 64-bit in OSX Catalina 10.15.7 </br>
**The Few Reasons to buy a GPU like M6000 or better for OSX 10.13.6 is FinalCutPro 10.4.3 + Compressor 4.4.1 </br>
[Rhino3D v6](https://www.rhino3d.com/6/system-requirements/)/[v5](https://www.rhino3d.com/5/system-requirements/) </br>

#### OSX HighSierra 10.13.6: </br>

AMD Rx 480 works in OSX HighSierra, Windows8.1 and most Linux </br>
does Not work in older OSX SnowLeopard, OSX Mavericks. </br>
it's a balanced option for Dual & Triple Boot. </br>

Nvidia Quadro 4000 has support from OSX 10.6.8 upto OSX 10.13.6 </br>
works in Windows8.1 and most Linux. </br>
has less 3D power, but has wider compatibility. </br>

K5000 is faster vs. Quadro 4000 but has limited OSX support. </br>
Rx 480 is faster vs. K5000 but also has limited OSX support. </br>

GTX 970 has support from OSX 10.9.5 upto OSX 10.13.6 </br>
Windows8.1 & Linux, same as M2000/M4000/M5000/M6000 </br>
its 5% faster vs. Rx 480 </br>
70% faster vs. HD 7950 </br>

P5000 is +20% faster vs. M6000-12 </br>
P6000 is +65% faster vs. M6000-12 </br>
P6000 is +60% faster vs. M6000-24 but... </br>
M6000-12 works in OSX Mavericks 10.9.5 </br>
Quadro Pascal have limited OSX support. </br> 

OSX prefers AMD for PCIe, Nvidia for eGPU. </br>

#### Nvidia Official Mac support: </br>
GeForce GTX 680 | GTX 285 | GT 120 | 8800 GT </br>
Quadro K5000 for Mac, Quadro 4000 for Mac </br>
Quadro FX 4800, Quadro FX 5600 </br>
but others also work with some issues. </br>

K5000 is +260% vs. Quadro FX 5600 </br>
K5000 is +200% vs. Quadro 4000 </br>
K5000 is +150% vs. Quadro FX 5800 </br>
K5000 is +127% vs. GTX 285 </br>
K5000 is +100% vs. Quadro K620 </br>
K5000 is +40% vs. Quadro 6000 </br>
R9 270x is +30% vs. K5000 </br>
Quadro K2200 is +30% vs. K5000 </br>
HD 7950 is +35% vs. K5000 </br>
K5200 is +50% vs. Quadro K5000 </br>
GTX 680 is +50% vs. Quadro K5000 </br>
R9 280x is +66% vs. K5000 </br>
K6000 is +100% vs. K5000 </br>
GTX 780 is +110% vs. K5000 </br>
RX 480 is +115% vs. K5000 </br>
Titan 6GB is +120% vs. K5000 </br>
R9 290 is +120% vs. K5000 </br>
GTX 970 is +130% vs. K5000 </br>
R9 290x is +140% vs. K5000 </br>
RX 580 is +140% vs. K5000 </br>
Titan Black +140% vs. K5000 </br>
GTX 780 Ti +150% vs. K5000 </br>
GTX 980 +180% vs. K5000 </br>
M6000-12GB +240% vs. K5000 </br>
M6000-24GB +250% vs. K5000 </br>
Titan X Maxwell +250% vs. K5000 </br>
GTX 980 Ti +270% vs. K5000 </br>
Vega-56 +270% vs. K5000 </br>
Vega Frontier Ed. +310% vs. K5000 </br>
Vega-64 +310% vs. K5000 </br>
Quadro P5000 +320% vs. K5000 </br>
Radeon VII +370% vs. K5000 </br>
Quadro P6000 +470% vs. K5000 </br>
Titan X pascal +470% vs. K5000 </br>
Titan Xp +500% vs. K5000 </br>
