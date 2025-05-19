# ASUS-PRIME-B660M-K-D4-WiFi-AX210-RX570-Mac15.5

# The overall configuration list of my black Apple host is as follows:

| Part Type     | Part Model 
|---------------|----------------------------------------------|
| Opencore      |  1.0.5                                       |
| Version       |  macOS Sequoia15.5                           |
| Motherboard   |  ASUS-PRIME-B660M-K-D4                       |
| Hard disk     |  Coiorful CN600 1T M2                        |
| Graphics      |  Radeon RX570  8G                            |
| CPU           |  Intel Core i5-12490F                        |
| Memory        |  ADATA 3000MHz 16G*2 DDR4    32G             |
| Wireless      |  Realtek RTL8111 LAN                         |
| Realtek Audio |  Realtek ALC897                              |
| WiFi          |  Intel AX210                                 |
|               |                                              |

# ASUS-PRIME-B660M-K-D Motherboards MacOS 15.5 Completeness:

Onboard audio is normal

The graphics card supports HDMI/DP display output

The front and rear 3.5 audio outputs are normal

Sleep wake-up is normal

Realtek RTL8111 LAN normal use

Solution 1: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-car. MacOS 15 requires the HELIPORT APP to use the WIFI function

Solution 2: The onboard intel AX210 Bluetooth and WIFi can be driven, and the network speed is very good, but it does not support air-carry; MacOS 15 requires OCLP patching here using option 2

If you want to achieve the additional function of air carry, you need to buy a NVME M.2 SSD to connect to the Heiguo wireless network card

The boot can support independent graphics (RX560/570/590/5500/5600/5700/6600 and other series) by default.

I won't talk about them one by one

# OpenCore Configuration

# ACPI

| ACPIs                    |
|--------------------------|
|  SSDT-PLUG-ALT           |
|  SSDT-AWAC-DISABLE       |
|  SSDT-EC-USBX            | 
|  SSDT-GPRW               |

# Drivers

| Driver Name     |
|-----------------|
| HfsPlus         |
| CrScreenshotDxe | 
| AudioDxe        | 
| OpenCanopy      |
| OpenRuntime     |
| ResetNvramEntry |
| ToggleSipEntry  |

# Kexts

| Kext Name                             |
|---------------------------------------|
| AppleALC.kext                         |
| CPUFriend.kext                        |
| CPUFriendDataProvider.kext            |
| CpuTopologyRebuild.kext               |
| CpuTscSync.kext                       |
| FeatureUnlock.kext                    |
| USBXHCIFixup.kext                     |
| RealtekRTL8111.kext                   |
| NVMeFix.kext                          |
| Lilu.kext                             | 
| SMCProcessor.kext                     | 
| SMCSuperIO.kext                       | 
| WhateverGreen.kext                    | 
| VirtualSMC.kext                       | 
| RestrictEvents.kext                   | 
| RadeonBoost.kext                      | 
| RadeonSensor.kext                     |
| USBPorts.kext                         | 
| USBWakeFixup.kext                     |
| AMFIPass.kext                         | 
| IOSkywalkFamily.kext                  |  
| IO80211FamilyLegacy.kext              | 
| AirportItlwm-15.5Sequoia.kext         |             
| IntelBTPatcher.kext                   |       
| IntelBluetoothFirmware.kext           |
| BlueToolFixup.kext                    |
|                                       | 
|                                       |
| I won't talk about them one by one    |

# BIOS Setup Reference:

Secure Boot 关闭

CSM         关闭

Resizable BAR  关闭

Above 4G Decoding 开启

AHCI  开启

## 关于打赏

如果您认可我的工作，请通过打赏支持我后续的更新(自觉打赏的人真少啊，免费的东西长久不了,现已改为需要密码解压，需微信或支付宝打赏入群。打赏记得留言备注你的qq号，然后申请入群时，填写你的留言为验证答案就是，我确认后会通过你的验证的。PS:之所以设置打赏，并不是为了赚大钱，当然大家打赏的多是有一些零花钱。主要是维护更新不易，每次系统一更新，有问题的话，就要工作时间之外花时间去调试，解决问题。普通群最多500人，无门槛的入群，不够用，有些机友对无门槛进入还不珍惜，进退群很随意，不看相关说明，上来就问问题的又多。不多说了，理解不理解的，就这样吧。

|  微信                                                                                 |
|---------------------------------------------------------------------------------------|
| ![1](https://github.com/user-attachments/assets/06d87fea-0d11-4bf4-b9ed-034dc7f53d06) |
|                                                                                       |
| ![1](https://github.com/user-attachments/assets/b99e75b4-69d3-450a-aae4-1a610760372d) |                                              |                                                                                       |
