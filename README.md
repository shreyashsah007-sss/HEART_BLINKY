# ❤️ Heart Blinky
### ABOUT
 I MAade a Heart-shaped LED chaser PCB with custom artwork, powered by NE555 and CD4017. Designed in KiCad for Blueprint.
### 3d view
<img width="1703" height="878" alt="Screenshot 2026-02-17 172040" src="https://github.com/user-attachments/assets/2466856c-21dd-4353-afb2-543ac14b5abc" />
### PCB
<img width="1052" height="723" alt="image" src="https://github.com/user-attachments/assets/675cd9db-a01a-4c49-b3f7-c0daf0d2f86d" />
### schematic
<img width="3507" height="2480" alt="image" src="https://github.com/user-attachments/assets/fbbec5b5-c905-44c3-a0d4-822fef99e253" />
### BOM
Id                                        Designator  Footprint           Quantity  Designation  Supplier and ref  Unnamed: 6
1  D5,D9,D7,D8,D10,D6,D1,D3,D2,D4                                        LED_D3.0mm         10                LED          NaN               NaN         NaN
2                             RV1               Potentiometer_Vishay_T93YA_Vertical          1                50k          NaN               NaN         NaN
3                              R1  R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal          1                 1k          NaN               NaN         NaN
4                              J1                   PinHeader_1x02_P2.54mm_Vertical          1  Conn_01x02_Socket          NaN               NaN         NaN
5                              C2                      C_Disc_D7.5mm_W2.5mm_P5.00mm          1            0.01 uF          NaN               NaN         NaN
<class 'pandas.core.frame.DataFrame'>
Index: 9 entries, 1 to 9
Data columns (total 7 columns):
 #   Column            Non-Null Count  Dtype  
---  ------            --------------  -----  
 0   Id                9 non-null      object 
 1   Designator        9 non-null      object 
 2   Footprint         9 non-null      int64  
 3   Quantity          9 non-null      object 
 4   Designation       0 non-null      float64
 5   Supplier and ref  0 non-null      float64
 6   Unnamed: 6        0 non-null      float64
dtypes: float64(3), int64(1), object(3)
memory usage: 576.0+ bytes
None

Python
import pandas as pd

# Read the CSV file
df = pd.read_csv('blinky.csv', sep=';')

# Based on inspection, the columns are shifted.
# Mapping:
# 'Id' -> Designator
# 'Designator' -> Footprint
# 'Footprint' -> Quantity
# 'Quantity' -> Value/Designation

bom_df = pd.DataFrame({
    'Designator': df['Id'],
    'Value': df['Quantity'],
    'Footprint': df['Designator'],
    'Quantity': df['Footprint']
})

# Display the cleaned BOM
print(bom_df.to_markdown(index=False))
[blinky.csv](https://github.com/user-attachments/files/25364889/blinky.csv)





