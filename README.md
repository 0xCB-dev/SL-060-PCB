# Synth Labs 060 PCB
## 60% Keyboard

Licence | OSHWA
:-------------------------:|:-------------------------:
![](https://github.com/0xCB-dev/sl-060-pcb/blob/main/LICENSE.svg) | [![](https://github.com/0xCB-dev/SL-060-PCB/blob/main/rev1.0/OSHWA.svg)](https://certification.oshwa.org/de000116.html)

### PCB:
KiCad version 5.99

Top | Bottom
:-------------------------:|:-------------------------:
![](https://github.com/0xCB-dev/SL-060-PCB/blob/main/rev1.0/pcb-hotswap.top.png)  |  ![](https://github.com/0xCB-dev/SL-060-PCB/blob/main/rev1.0/pcb-hotswap.bottom.png)

#### BOM:

[ibom daughterboard](https://files.0xcb.dev/0xCB/SL-060-PCB/daughterboard.html)

[ibom hotswap pcb](https://files.0xcb.dev/0xCB/SL-060-PCB/pcb-hotswap.html)

[ibom soldered pcb](https://files.0xcb.dev/0xCB/SL-060-PCB/pcb-solder.html)

##### Daughterboard

| References | Value        | Footprint             | Quantity | Mouser                 |
|------------|--------------|-----------------------|----------|------------------------|
| J1         | USB4120-03-C | GCT_USB4120-03-C_REVA | 1        |  640-USB4120-03-C      |
| J2         | Conn_01x04   | JST-SR-4              | 1        |  485-4208              |
| R1, R2     | 5.1k         | R_0603_1608Metric     | 2        |  667-ERA-3AED512V      |
| R3, R4     | 22           | R_0603_1608Metric     | 2        |  754-RG1608Q-220DT5    |
| U1         | USBLC6-2SC6  | SOT-23-6              | 1        |  511-USBLC6-2SC6       |
| C1         | 10u          | C_0603_1608Metric     | 1        |  80-C0603C106M8PLR     |
| C2         | 1u           | C_0603_1608Metric     | 1        |  81-GCG188L8EE105KA7D  |
| F1         | 3A           | Fuse_0805_2012Metric  | 1        |  652-MF-PSML150/6-2    |
| D1         | SMF5.0CA     | D_SOD-123F            | 1        |  576-SMF5.0CA          |
| FB1, FB2   | 600R         | Ferrite_Bead_0603     | 2        |  81-BLM18KN601EH1D     |

##### Soldered PCB

| References     | Value      | Footprint                                       | Quantity | Mouser                 |
|----------------|------------|-------------------------------------------------|----------|------------------------|
| J2             | Conn_01x04 | JST-SR-4                                        | 1        | 485-4208               |
| R1, R2         | 10k        | R_0603_1608Metric                               | 2        | 754-RG1608N-103-BT5    |
| U1             | ATMEGA32U4 | QFN-44-1EP_7x7mm_P0.5mm_EP5.2x5.2mm_ThermalVias | 1        | 556-ATMEGA32U4-MU      |
| Y1             | 16MHz      | Crystal_SMD_3225-4Pin_3.2x2.5mm                 | 1        | 581-CX3225SB16H0PST    |
| C2, C3, C4, C5 | 100n       | C_0603_1608Metric                               | 4        | 80-C603C104K5RAC3121   |
| C1, C8         | 1u         | C_0603_1608Metric                               | 2        | 81-GCG188L8EE105KA7D   |
| C6, C7         | 22p        | C_0603_1608Metric                               | 2        | 80-C0603C220J5G7411    |
| SW1            | SW_Push    | SW_SPST_TL3342                                  | 1        | 611-PTS526SM15SMTR2L   |
| D1, ..., D34   | BAV70      | SOT-23                                          | 34       | 241-BAV70_R1_00001     |

##### Hotswap PCB

| References                             | Value        | Footprint                                       | Quantity | Mouser                                                                                                              |
|----------------------------------------|--------------|-------------------------------------------------|----------|---------------------------------------------------------------------------------------------------------------------|
| J2                                     | Conn_01x04   | JST-SR-4                                        | 1        | 485-4208                                                                                                            |
| R3, R4                                 | 10k          | R_0603_1608Metric                               | 2        | 754-RG1608N-103-BT5                                                                                                 |
| U1                                     | ATMEGA32U4   | QFN-44-1EP_7x7mm_P0.5mm_EP5.2x5.2mm_ThermalVias | 1        | 556-ATMEGA32U4-MU                                                                                                   |
| Y1                                     | 16MHz        | Crystal_SMD_3225-4Pin_3.2x2.5mm                 | 1        | 581-CX3225SB16H0PST                                                                                                 |
| C2, C3, C4, C5, C9, C10, C11, C12, C13 | 100n         | C_0603_1608Metric                               | 9        | 80-C603C104K5RAC3121                                                                                                |
| C1, C8                                 | 1u           | C_0603_1608Metric                               | 2        | 81-GCG188L8EE105KA7D                                                                                                |
| C6, C7                                 | 22p          | C_0603_1608Metric                               | 2        | 80-C0603C220J5G7411                                                                                                 |
| SW1                                    | SW_Push      | SW_SPST_TL3342                                  | 1        | 611-PTS526SM15SMTR2L                                                                                                |
| D1, ..., D63                           | SK6812MINI-E | MX_SK6812MINI-E                                 | 63       | https://cdn-shop.adafruit.com/product-files/4960/4960_SK6812MINI-E_REV02_EN.pdf                                     |
| D64, ..., D96                          | BAV70        | SOT-23                                          | 33       | 241-BAV70_R1_00001                                                                                                  |
| MX*                                    | MX           | SW_Hotswap_Kailh_*                              | 61       | https://www.kailhswitch.com/mechanical-keyboard-switches/box-switches/kailh-rainbow-mx-hot-swapping-pcb-socket.html |
