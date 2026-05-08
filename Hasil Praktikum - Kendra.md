# Praktikum-Analisis-Penjualan-
Kendra Respati Maheswara Ugroho XI RPL 8 / 18

===== DATA AWAL =====
   Order_ID  CustomerID  Order_Date Product_Category  Quantity  Price_Per_Unit  Ad_Budget  Total_Sales
0      1001        5039  2023-08-19            Books         4       1184000.0   982000.0    4736000.0
1      1002        5029  2023-08-29          Fashion         5       1733000.0  3513000.0    8665000.0
2      1003        5015  2023-02-21          Fashion         4       1767000.0  2117000.0    7068000.0
3      1004        5043  2023-04-06          Fashion         2        512000.0  4384000.0    1024000.0
4      1005        5008  2023-08-10       Home Decor         2       1820000.0  2625000.0    3640000.0

===== INFO DATA =====
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 150 entries, 0 to 149
Data columns (total 8 columns):
 #   Column            Non-Null Count  Dtype  
---  ------            --------------  -----  
 0   Order_ID          150 non-null    int64  
 1   CustomerID        150 non-null    int64  
 2   Order_Date        150 non-null    object 
 3   Product_Category  150 non-null    object 
 4   Quantity          150 non-null    int64  
 5   Price_Per_Unit    150 non-null    float64
 6   Ad_Budget         150 non-null    float64
 7   Total_Sales       143 non-null    float64
dtypes: float64(3), int64(3), object(2)
memory usage: 9.5+ KB
None

===== DATA KOSONG =====
Order_ID            0
CustomerID          0
Order_Date          0
Product_Category    0
Quantity            0
Price_Per_Unit      0
Ad_Budget           0
Total_Sales         7
dtype: int64

===== TUGAS 1 : PRODUK UNDERPERFORMER =====

Rata-rata Harga:
1024640.0

10 Produk Underperformer:
     Order_ID  CustomerID Order_Date Product_Category  Quantity  Price_Per_Unit  Ad_Budget  Total_Sales
7        1008        5019 2023-05-23           Gadget         1       1431000.0  1197000.0    1431000.0
19       1020        5044 2023-06-19            Books         1       1654000.0   552000.0    1654000.0
41       1042        5009 2023-07-17           Gadget         1       1992000.0  3773000.0    1992000.0
33       1034        5016 2023-07-09       Home Decor         1       1853000.0  3824000.0    1853000.0
88       1089        5026 2023-11-21          Fashion         1       1399000.0   126000.0    1399000.0
90       1091        5045 2023-07-17      Electronics         1       1512000.0  2505000.0    1512000.0
114      1115        5028 2023-05-31           Gadget         1       1200000.0  1088000.0    1200000.0
120      1121        5033 2023-12-12          Fashion         1       1811000.0  2419000.0    1811000.0
91       1092        5041 2023-08-28          Fashion         1       1831000.0  3642000.0    1831000.0
92       1093        5029 2023-05-24            Books         1       1191000.0  4122000.0    1191000.0

===== TUGAS 2 : RFM ANALYSIS =====

Hasil RFM:
            Recency  Frequency    Monetary
CustomerID                                
5001            213          4   8562000.0
5002             77          4   6931000.0
5003            118          3   9433000.0
5004            196          3  15368000.0
5005             23          2   9105000.0

10 Pelanggan Terbaik:
            Recency  Frequency    Monetary
CustomerID                                
5015             21          6  26309000.0
5008             15          6  22350000.0
5035             53          6  22066000.0
5014             54          6  20797000.0
5044             18          7  20631000.0
5025             75          4  18907000.0
5042              1          4  18754000.0
5023            114          3  17203000.0
5034            137          2  16895000.0
5026             36          5  15835000.0

===== TUGAS 3 : EFISIENSI KATEGORI =====

Efisiensi Kategori:
                  Total_Sales   Ad_Budget  Efisiensi
Product_Category                                    
Gadget             70523000.0  76539000.0   0.921400
Home Decor         69340000.0  64808000.0   1.069930
Fashion            96550000.0  82317000.0   1.172905
Books             107569000.0  89914000.0   1.196354
Electronics       114095000.0  79264000.0   1.439430

===== TUGAS 4 : PENGARUH IKLAN =====

Median Ad Budget:
2722500.0

Rata-rata Penjualan Iklan Tinggi:
3156275.362318841

Rata-rata Penjualan Iklan Rendah:
3247216.2162162163

KESIMPULAN:
Iklan tinggi belum tentu meningkatkan penjualan.

===== TREN PENJUALAN BULANAN =====
Month
2023-01    19910000.0
2023-02    39524000.0
2023-03    24003000.0
2023-04    45084000.0
2023-05    50372000.0
2023-06    44580000.0
2023-07    21909000.0
2023-08    83500000.0
2023-09    42062000.0
2023-10    23454000.0
2023-11    34654000.0
2023-12    29025000.0
Name: Total_Sales, dtype: float64

===== ANALISIS KORELASI =====
                Total_Sales  Ad_Budget  Price_Per_Unit
Total_Sales        1.000000   0.054778        0.686168
Ad_Budget          0.054778   1.000000       -0.053446
Price_Per_Unit     0.686168  -0.053446        1.000000

===== PROGRAM SELESAI =====


<img width="1920" height="1080" alt="Screenshot 2026-05-08 095307" src="https://github.com/user-attachments/assets/8b4f125e-4ee5-4ed8-a247-f6cead4229bc" />
<img width="1920" height="1080" alt="Screenshot 2026-05-08 095328" src="https://github.com/user-attachments/assets/206921e0-09dc-4336-aeb4-94924a2466e8" />
<img width="1920" height="1080" alt="Screenshot 2026-05-08 095323" src="https://github.com/user-attachments/assets/bd698583-f017-4ec7-9ce5-57ab23ca3be1" />
<img width="1920" height="1080" alt="Screenshot 2026-05-08 095318" src="https://github.com/user-attachments/assets/ee19df00-398e-4071-8ca4-f1db945590b3" />
