# 📊 Proyek Analisis Data: Brazilian E-Commerce (Olist)

## Deskripsi
Proyek ini menganalisis data e-commerce publik Olist (Sep 2016 – Okt 2018) untuk menjawab dua pertanyaan bisnis:
1. Pada bulan dan tahun apa penjualan mencapai nilai tertinggi, dan bagaimana pola tren pertumbuhannya?
2. Kategori produk apa yang menghasilkan pendapatan tertinggi dan bagaimana hubungannya dengan skor ulasan pelanggan?

Analisis mencakup Data Wrangling, EDA, Visualisasi, dan RFM Analysis untuk segmentasi pelanggan.

## Struktur Direktori
```
submission/
├── dashboard/
│   ├── dashboard.py        # Aplikasi Streamlit
│   └── main_data.csv       # Data gabungan untuk dashboard
├── data/
│   ├── orders_dataset.csv
│   ├── order_items_dataset.csv
│   ├── customers_dataset.csv
│   ├── order_payments_dataset.csv
│   ├── order_reviews_dataset.csv
│   ├── products_dataset.csv
│   ├── sellers_dataset.csv
│   └── product_category_name_translation.csv
├── notebook.ipynb          # Notebook analisis lengkap
├── README.md
├── requirements.txt
└── url.txt
```

## Setup Environment

### 1. Clone atau download repositori ini

### 2. Buat virtual environment
```bash
python -m venv venv
```

### 3. Aktifkan virtual environment
- **Windows:**
  ```bash
  venv\Scripts\activate
  ```
- **Mac/Linux:**
  ```bash
  source venv/bin/activate
  ```

### 4. Install dependencies
```bash
pip install -r requirements.txt
```

## Menjalankan Dashboard
```bash
streamlit run dashboard/dashboard.py
```
Dashboard akan terbuka otomatis di browser pada `http://localhost:8501`

## Fitur Interaktif Dashboard
- 📅 **Filter Rentang Tanggal** — eksplorasi data berdasarkan periode tertentu
- 📦 **Filter Status Order** — fokus pada delivered, shipped, cancelled, dst.
- 🏷️ **Filter Kategori Produk** — analisis kategori spesifik

## Key Insights
- Puncak penjualan: **November 2017** (>7.500 order, dipicu Black Friday)
- Kategori revenue tertinggi: **Bed, Bath & Table** (>R$ 1,7 juta)
- Mayoritas pelanggan masuk segmen **Lost Customers** → perlu strategi retensi agresif
