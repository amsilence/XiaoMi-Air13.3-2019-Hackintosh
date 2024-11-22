# XiaoMi-Air13.3-2019-Hackintosh

此版本EFI支持版本为：macOS 11.x/macOS 12.x/macOS 13.x/macOS 14.x/macOS 15.1.x

## 电脑配置信息/Computer configuration

|        型号         | 小米Air13.3 2019款 |
| :-------------------------: | :----------: |
|     CPU   | i7 8550U |
|     内存     | 8G DDR4 |
| 固态 | 三星NVME MZVLW256 (256G固态硬盘) |
|     集成显卡  | Intel(R) UHD Graphics 620  (1 GB) |
|     独立显卡     | MX250 (2GB) |
| 无线网卡 | 英特尔AC8265 |
|     蓝牙      | 英特尔AC8265 |
|     显示器     |    13.3寸 1080P    |
| 声卡 |    ---    |

## 仿造APPLE型号

- SMBIOS: MacBookPro16,3


## 注意/attention

1.修复AX201蓝牙在macOS 15.1.x无法驱动的问题

- 涉及的kext驱动

|          kext name          | kext version |           download link            |
| :-------------------------: | :----------: | :--------------------------------: |
|     BlueToolFixup.kext      |    2.6.9     | https://dortania.github.io/builds/ |
|     IntelBTPatcher.kext     |    2.5.0     | https://dortania.github.io/builds/ |
| IntelBluetoothFirmware.kext |    2.5.0     | https://dortania.github.io/builds/ |


- NVRAM配置的参数

|               key               | Data Type |            Value             |
| :-----------------------------: | :-------: | :--------------------------: |
|  bluetoothExternalDongleFailed  |   Data    |              00              |
| bluetoothInternalControllerInfo |   Data    | 0000000000000000000000000000 |

2.修复AX201 WIFI在macOS 15.1.x无法驱动的问题

- 需要添加 IOSkywalkFamily.kext、IO80211FamilyLegacy.kext、AirportItlwm_v2.3.0_stable_Ventura.kext
- OpenCore-Patcher需要安装1.6.0版本的，才能安装补丁



## 对这台电脑的评价

1. 感觉是最像MacBook Air 13.3的电脑
2. 这台电脑板载的内存8GB，可玩性被缩小了
3. 有两个硬盘位，存储空间可以进行扩容
4. 板载的无线网卡和蓝牙性能较差



