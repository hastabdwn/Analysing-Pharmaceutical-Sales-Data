# 💊 Analysing Pharmaceutical Sales Data

Proyek analisis data penjualan obat farmasi berdasarkan data historis harian dari sebuah apotek. Proyek ini merupakan bagian dari roadmap Data Analyst di [roadmap.sh](https://roadmap.sh/projects/analysing-pharmaceutical-sales-data).

---

## 📌 Business Understanding

Distributor farmasi membutuhkan pemahaman mendalam terhadap performa penjualan dari berbagai kategori obat (ATC Code) agar dapat mengoptimalkan strategi distribusi, manajemen stok, dan perencanaan bisnis ke depan.

**Pertanyaan analisis:**
- Berapa total kuantitas penjualan untuk setiap kategori obat (ATC Code)?
- Brand obat mana yang memiliki total penjualan tertinggi?
- Apa 3 obat dengan penjualan tertinggi pada Januari 2015, Juli 2016, dan September 2017?
- Obat mana yang paling sering terjual sepanjang tahun 2017?
- Kategori obat mana yang memiliki rata-rata penjualan harian tertinggi?
- Apakah obat pernapasan (R03) terjual lebih banyak di bulan-bulan tertentu?

---

## 📂 Dataset

- **Sumber**: [Kaggle – Pharma Sales Data](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data)
- **File**: `salesdaily.csv`
- **Periode**: 2014 – 2019
- **Format**: Data penjualan harian per sesi transaksi

### Kategori Obat (ATC Code)

| Kode   | Kategori                                      |
|--------|-----------------------------------------------|
| M01AB  | Anti-inflamasi – Acetic acid derivatives      |
| M01AE  | Anti-inflamasi – Propionic acid derivatives   |
| N02BA  | Analgesik – Salicylic acid derivatives        |
| N02BE  | Analgesik – Anilide (Paracetamol)             |
| N05B   | Anxiolitik (Obat penenang)                    |
| N05C   | Hipnotik & Sedatif                            |
| R03    | Obat Pernapasan                               |
| R06    | Antihistamin                                  |

---

## 🚀 Open in Google Colab

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1fXY9Zr9PPMpuLhyEch3D-u4wnaSgI5zE?usp=sharing)

---

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)

---

## 📁 Project Structure

```
Analysing-Pharmaceutical-Sales-Data/
│
├── data/
│   └── salesdaily.csv                        # Dataset mentah
│
├── Analysing_Pharmaceutical_Sales_Data.ipynb # Notebook utama
├── Pharmaceutical_Sales_Analysis.xlsx        # Output hasil analisis
└── README.md
```

---

## 📊 Alur Analisis

```
1. Business Understanding
        ↓
2. Import Library
        ↓
3. Import Dataset & Preview
        ↓
4. Data Understanding
        ↓
5. Data Preprocessing
   (missing values, duplikat, konversi tipe data)
        ↓
6. Exploratory Data Analysis (EDA)
   (distribusi, korelasi, tren harian & tahunan)
        ↓
7. Analysis Process
   (6 pertanyaan bisnis)
        ↓
8. Insight & Rekomendasi
        ↓
9. Exporting Data (.xlsx)
```

---

## 💡 Key Insights

- **N02BE** (Paracetamol) mendominasi total penjualan dan frekuensi transaksi — menjadikannya *core product* yang paling diandalkan.
- **Obat pernapasan (R03)** menunjukkan lonjakan penjualan di bulan-bulan tertentu, mengindikasikan pola musiman.
- Penjualan tertinggi cenderung terjadi di hari-hari kerja (weekday) dibandingkan akhir pekan.
- Kategori obat penenang dan sedatif (N05B, N05C) memiliki volume penjualan yang jauh lebih rendah dibanding analgesik.

---

## ▶️ Cara Menjalankan

1. Clone repository ini:
   ```bash
   git clone https://github.com/hastabdwn/Analysing-Pharmaceutical-Sales-Data.git
   cd Analysing-Pharmaceutical-Sales-Data
   ```

2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```

3. Buka notebook:
   ```bash
   jupyter notebook Analysing_Pharmaceutical_Sales_Data.ipynb
   ```

4. Jalankan semua cell secara berurutan (Run All).

> **Catatan**: Dataset akan otomatis diunduh dari Google Sheets saat notebook dijalankan. Pastikan koneksi internet tersedia.

---

## 👤 Author

**hastabdwn**  
[![GitHub](https://img.shields.io/badge/GitHub-hastabdwn-181717?logo=github)](https://github.com/hastabdwn)
