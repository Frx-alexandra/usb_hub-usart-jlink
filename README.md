# usb_hub-usart-jlink

usb_hub包含两个usb口一个串口一个jlink_ob程序下载口

## jilink驱动程序在```Firmware```中可以通过```keil```直接下载芯片中

* 首先需要复制一个跟主控同型号的可用的工程，然后将其编译
* 之后需要将```Firmware```文件夹中的```ob-stm32.hex```文件复制到本工程生成的```.hex```文件夹中
* 打开keil的```options for target```界面，选择output，修改```name of executable```内容为```ob-stm32.hex```
* 直接进行下载，不要再进行编译

## 如果你的KEIL显示```jlink is defective```说明KEIL的jlink版本过高，可以将```.\keil\ARM\Segger```文件夹整个替换掉
