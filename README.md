# <p align="center">项目说明</p>

- 原本是想写一个OLED屏幕的驱动程序，但是后来项目打开错误，在原本的OLED项目中写了一个用于调试无刷电机的PWM串口调试
- 串口波特率`9600`，通讯起始符`$`终止符`!`，控制示例:更改Compare为900 `$900!`
- TB上的海凌科电调要求一开始输出频宽0.2ms的PWM终止信号，即Compare为`900`，等待2s后再输出大于频宽0.2ms的PWM信号，最高转速为2ms的PWM信号，即Compare为`2000`
- 项目开发环境: `VSCode、EIDE(VSCode扩展插件)、Keil uVision5`
- 烧录工具: `ST-Link V2`
