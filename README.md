# ❤️ Heart Blinky
### ABOUT
 I Made a Heart-shaped LED chaser PCB with custom artwork, powered by NE555 and CD4017. Designed in KiCad for Blueprint.
### **Why I Made This**
I finished my exams and had some free time, so I decided to jump back into another Blueprint project to keep improving my skills.
### **How to Use It**
Connect a 5V to 9V DC power source to the J1 header.

The LEDs will begin to chase in a heart-shaped sequence.

Turn the RV1 potentiometer knob to speed up or slow down the "heartbeat" effect.

### **3d view**
<img width="1703" height="878" alt="Screenshot 2026-02-17 172040" src="https://github.com/user-attachments/assets/2466856c-21dd-4353-afb2-543ac14b5abc" />





### **PCB**
<img width="1052" height="723" alt="image" src="https://github.com/user-attachments/assets/675cd9db-a01a-4c49-b3f7-c0daf0d2f86d" />





### **schematic**
<img width="3507" height="2480" alt="image" src="https://github.com/user-attachments/assets/fbbec5b5-c905-44c3-a0d4-822fef99e253" />





### ** Bill of Materials (BOM)**

| Designator                     | Value             | Footprint                                        |   Quantity |
|:-------------------------------|:------------------|:-------------------------------------------------|-----------:|
| D5,D9,D7,D8,D10,D6,D1,D3,D2,D4 | LED               | LED_D3.0mm                                       |         10 |
| RV1                            | 50k               | Potentiometer_Vishay_T93YA_Vertical              |          1 |
| R1                             | 1k                | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal |          1 |
| J1                             | Conn_01x02_Socket | PinHeader_1x02_P2.54mm_Vertical                  |          1 |
| C2                             | 0.01 uF           | C_Disc_D7.5mm_W2.5mm_P5.00mm                     |          1 |
| U2                             | 4017              | DIP-16_W7.62mm                                   |          1 |
| C1                             | 1 uF              | CP_Radial_D5.0mm_P2.00mm                         |          1 |
| R2                             | 470               | R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal |          1 |
| U1                             | NE555P            | DIP-8_W7.62mm                                    |          1 |




[blinky.csv](https://github.com/user-attachments/files/25366329/blinky.csv)


