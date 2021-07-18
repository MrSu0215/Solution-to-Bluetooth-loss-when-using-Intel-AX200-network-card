Solution to Bluetooth loss when using Intel AX200 network card

因特尔AX200网卡使用时蓝牙丢失的解决办法

Install and use AX200 network card, Wi-Fi is normal but the Bluetooth control panel disappears or the Bluetooth switch cannot be used.

安装使用AX200网卡，Wi-Fi正常但蓝牙控制面板消失不见或者蓝牙开关无法使用。

To make Intel Bluetooth work in Big Sur, the following are required:

1. The latest version of Lilu (from source code)

2. The latest version of BrcmPatchRAM (from source code), this package only needs
BlueToolFixup.kext

3. Download and install the following files in the author's Bluetooth driver package

IntelBluetoothFirmware.kext

IntelBluetoolInjector.kext.

4. Turn off XhciPortLimit in OpenCore Configurator

5. Save the config file

6. Shut down and restart the machine instead of restarting it.

要使英特尔蓝牙在Big Sur工作，需要以下内容：

1.最新版的Lilu（来自源码）

2.最新版本的 BrcmPatchRAM（来自源码），这个包中只需要

BlueToolFixup.kext

3.下载安装作者蓝牙驱动包中的以下文件

IntelBluetoothFirmware.kext

IntelBluetoolInjector.kext。

4.在OpenCore Configurator中关闭 XhciPortLimit

5.保存config文件

6.关闭并重新启动机器而不是重新启动。

![image](https://user-images.githubusercontent.com/55876369/126084793-e3a8ac82-2b72-4618-b65f-8c5f06614241.png)

After booting, you can see the Bluetooth hardware information in the hackintool and system reports. During use, Bluetooth is normal and the system's Bluetooth switch is operating normally.

开机后，便可以在hackintool和系统报告中看到蓝牙的硬件信息。在使用过程中，蓝牙正常且系统蓝牙开关正常操作。
![image](https://user-images.githubusercontent.com/55876369/126084842-5181aaae-f0a0-4ad3-8893-b16f801f144c.png)
![image](https://user-images.githubusercontent.com/55876369/126084874-c07c76c8-987f-4c2f-b429-95db7317b535.png)
