# USBTO3DO-FZ1
这是Francois CARON的SATATO3DO项目https://github.com/FCare/SataTo3DO的拓展，使用了集成电路来缩小体积，具体使用方法请参考其方案

BOM:

最小系统：

U1 RP2040 MODULE

U2/U3 TXS0108

U4 74LVC4245

R2 4.7K

1.25MM 12P

1.25MM 30P

如果你要在模块上建立一个换盘功能（同主机EJECT按钮功能）：

你需要增加一个6X6mm的按钮开关

如果你要在模块上建立一个读盘灯（同主机面板绿色读盘灯）：

你需要增加：
R1：470欧姆
LED：3MM

如果你需要在模块上建立一个USB-A口：

你需要增加一个USB-A母口，并按照图示将D+，D-连接到RP2040模块，但注意，这里并没有HUB功能，只能使用其中的一个，其意义是省去一根TYPE-C的转换线

预留了电容的位置，可以不需要安装
C1/C2：220uf-470uf/10V
C3/C4/C5/C6：0.1uf
