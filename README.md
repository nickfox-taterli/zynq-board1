# 咸鱼新发现的矿板

------

| 信号 | 接口 | 备注 |
| :--------: | :-----: | :----: |
| PSCLK | - | 33.33MHz |
| MIO0 | D2 LED ||
| MIO1 - MIO6 | S25FL512 | 可启动 |
| MIO8 - MIO8 | SP3232 - J10 - GND/TX/RX | | 
| MIO10 - MIO15 | J6 | 不可启动 |
| MIO16 - MIO27 / MIO52 - MIO53 | RTL8211F - J4 | 似乎只能协商10Mbps |
| MIO28 - MIO39 / MIO52 - MIO53 | RTL8211F - J5 | 似乎只能协商10Mbps |
| MIO40 - MIO51 / MIO7(RESETB) | USB3320 - J9 - VBUS/D-/D+/GND ||
| DDR3 | U3 / U4 | |
| PROG_B | K1 | ? |
| PL_G14 | K2 | |
| PL_DONE | D1 | |
| PL_LED1 | D29 | |
| PL_LED2 | D31 | |
| PL_LED3 | D32 | |
| JTAG | J1 - GND/TDI/TDO/TCK/TMS/3V3 | |
| PL_SD | J7 - CLK(D20)/CMD(E17)/D0(D18)/D1(B19)/D2(C20)/D3(D19)/CD(B20)| |
| EMIO | J13 - GND/U20/N20 | |
| PL_GPIO | J12 - K19/F20/J18/GND/L20/L17/M17/K18/L16/5V | |
| PL_EEPROM | U18 - SCL(P16)/SDA(P15)| |

##启动模式(纯逆向可能不对)

| 开关 | 1 | 2 |
| :-----: | :-----: | :-----: |
| QSPI | 1 | 0 |
| JTAG | 0 | 0 |

![成色不错的板子图][1]


  [1]: board.jpg
