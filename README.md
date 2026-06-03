# CAN-Shield for STM32F469I-DISCO

STM32F469I-DISCO board compatible CAN shield.

<p float="left">
  <img src="img/glr-pcb-display-can-shield-front.png" width="49%" />
  <img src="img/glr-pcb-display-can-shield-back.png" width="49%" />
</p>

## Overview

Provides 8V for the discovery board, from 24V car voltage.

Acts as can transciever for the discovery board.

Accessible screw terminals for buttons signals to the discovery board.

Can be directly slotted on to the board.

## Used parts

Exported from KiCad BOM. View there for more details.

| DigiKey                   | WuerthElektronik | Reference         | Footprint                                                  | Qty |
|---------------------------|------------------|-------------------|------------------------------------------------------------|-----|
| 541-60.4HCT-ND            |                  | R4,R5             | Resistor_SMD:R_0603_1608Metric                             | 2   |
| 311-22.1KHRCT-ND          |                  | R3                | Resistor_SMD:R_0603_1608Metric                             | 1   |
| P200KDBCT-ND              |                  | R2                | Resistor_SMD:R_0603_1608Metric                             | 1   |
| 311-10.0KHRCT-ND          |                  | R1                | Resistor_SMD:R_0603_1608Metric                             | 1   |
| 732-74479889310CT-ND      | 74479889310      | L1                | Inductor_SMD:L_1008_2520Metric                             | 1   |
| 732-61802525023-ND        | 61802525023      | J2                | Connector_Dsub:DSUB-25_Socket_Vertical_P2.77x2.84mm        | 1   |
| 732-643250100304-ND       | 643250100304     | J1                | GLR_KiCad_Library:M12A-04P                                 | 1   |
| ATA6561-GAQW-NCT-ND       |                  | IC2               | SamacSys_Parts:SOIC127P600X175-8N                          | 1   |
| 31-AP64060QWU-7CT-ND      |                  | IC1               | SamacSys_Parts:SOT95P280X100-6N                            | 1   |
| 732-7290-1-ND             | 744235510        | FL1               | SamacSys_Parts:744235510                                   | 1   |
| 497-15333-1-ND            |                  | D1                | SamacSys_Parts:SOT95P255X125-3N                            | 1   |
| 732-5299-ND               | 61301621121      | CN12              | Connector_PinSocket_2.54mm:PinSocket_2x08_P2.54mm_Vertical | 1   |
| 732-5319-ND               | 61300611121      | CN8               | Connector_PinHeader_2.54mm:PinHeader_1x06_P2.54mm_Vertical | 1   |
| 732-5321-ND               | 61300811121      | CN6,CN7           | Connector_PinHeader_2.54mm:PinHeader_1x08_P2.54mm_Vertical | 2   |
| 732-2670-ND               | 61301011121      | CN5               | Connector_PinHeader_2.54mm:PinHeader_1x10_P2.54mm_Vertical | 1   |
| 490-1427-1-ND             |                  | C9,C10,C11,C12    | Capacitor_SMD:C_0603_1608Metric                            | 4   |
| 399-C0603C105K4RACTUCT-ND |                  | C4                | Capacitor_SMD:C_0603_1608Metric                            | 1   |
| 399-C0603C104K3RACTUCT-ND |                  | C2,C3,C5,C6,C7,C8 | Capacitor_SMD:C_0603_1608Metric                            | 6   |
| 1276-1040-1-ND            |                  | C1                | Capacitor_SMD:C_0603_1608Metric                            | 1   |

## Used pins and their connector

| Element | Chip Pin | Connector Pin |
| ------- | -------- | ------------- |
| 5V      | -        | CN6 Pin 5     |
| GND     | -        | CN6 Pin 6,7   |
| 8V IN   | -        | CN6 Pin 8     |

### Button 1-6

| Element  | Chip Pin | Connector Pin |
| -------- | -------- | ------------- |
| Button 1 | PB1      | CN8 Pin 1     |
| Button 2 | PC4      | CN8 Pin 4     |
| Button 3 | PC5      | CN8 Pin 5     |
| Button 4 | PA4      | CN8 Pin 6     |
| Button 5 | PD3      | CN5 Pin 6     |
| Button 6 | PB14     | CN5 Pin 5     |

### Incremental Rotary Encoder 1-2

| Element                   | Chip Pin | Connector Pin |
| ------------------------- | -------- | ------------- |
| Incremental Encoder 1 CLK | PB15     | CN5 Pin 4     |
| Incremental Encoder 1 DT  | PH6      | CN5 Pin 3     |
| Incremental Encoder 1 SW  | PA7      | CN5 Pin 2     |
| Incremental Encoder 2 CLK | PG13     | CN7 Pin 3     |
| Incremental Encoder 2 DT  | PG14     | CN7 Pin 2     |
| Incremental Encoder 2 SW  | PG9      | CN7 Pin 1     |

### Absolute Rotary Encoder 1-3

| Element               | Chip Pin | Connector Pin |
| --------------------- | -------- | ------------- |
| Absolute Encoder 1 P1 | PA8      | CN12 Pin 3    |
| Absolute Encoder 1 P2 | PB4      | CN12 Pin 5    |
| Absolute Encoder 1 P3 | PC6      | CN12 Pin 6    |
| Absolute Encoder 2 P1 | PA8      | CN12 Pin 7    |
| Absolute Encoder 2 P2 | PA5      | CN12 Pin 8    |
| Absolute Encoder 2 P3 | PC7      | CN12 Pin 11   |
| Absolute Encoder 3 P1 | PA15     | CN12 Pin 12   |
| Absolute Encoder 3 P2 | PB12     | CN12 Pin 13   |
| Absolute Encoder 3 P3 | PC13     | CN12 Pin 14   |
| Absolute Encoder 3 P4 | PC1      | CN12 Pin 15   |
