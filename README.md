# Project for BNSP Data Analyst Assessment  
## E-Commerce Sales & Customer Analysis (RFM Segmentation)

### Deskripsi Project  
Project ini merupakan portfolio Data Analyst yang dibuat untuk kebutuhan assessment skema Data Analyst (BNSP).  
Analisis dilakukan menggunakan dataset transaksi e-commerce UK (2010–2011) untuk memahami performa penjualan, perilaku pelanggan, serta menghasilkan insight bisnis berbasis data.

### Dataset  
- Sumber: UCI Machine Learning Repository (Online Retail Dataset)  
- Jumlah data: ±541.000 baris transaksi  
- Kolom utama:
  - InvoiceNo  
  - StockCode  
  - Description  
  - Quantity  
  - UnitPrice  
  - CustomerID  
  - Country  
  - InvoiceDate  

### Tujuan Analisis  
1. Menganalisis performa penjualan selama periode observasi.  
2. Mengidentifikasi produk dan customer dengan kontribusi revenue terbesar.  
3. Mengetahui negara dengan kontribusi revenue tertinggi.  
4. Menganalisis perilaku pelanggan menggunakan metode RFM (Recency, Frequency, Monetary).  
5. Menentukan segmen pelanggan yang perlu diprioritaskan untuk strategi bisnis.

### Tools  
- Python (Pandas, NumPy, Matplotlib, Seaborn)  
- Google Colab (Data Cleaning & EDA)  
- Looker Studio (Dashboard Visualisasi)  

### Data Preparation  
Proses data cleaning meliputi:
- Menghapus data duplikat.  
- Menghapus transaksi tidak valid (Quantity ≤ 0 dan UnitPrice ≤ 0).  
- Menghapus data dengan CustomerID kosong untuk analisis customer.  
- Konversi tipe data InvoiceDate ke format datetime.  
- Membuat kolom baru:  
  `TotalPrice = Quantity × UnitPrice`.

### Exploratory Data Analysis (EDA)  
Beberapa analisis utama yang dilakukan:
- Distribusi transaksi per negara (UK mendominasi >80%).  
- Tren revenue bulanan (peningkatan signifikan pada Nov–Des).  
- Pareto Analysis produk (≈20% produk menghasilkan ≈80% revenue).  
- RFM Analysis untuk segmentasi pelanggan berdasarkan:
  - Recency  
  - Frequency  
  - Monetary  

### Insight Utama  
- Sebagian besar revenue berasal dari UK (>80%).  
- Terdapat pola musiman dengan puncak penjualan menjelang akhir tahun.  
- Sekitar 20% produk menyumbang hampir 80% revenue (Prinsip Pareto).  
- Segmen **Best Customers** memberikan kontribusi revenue terbesar (>£7M).  
- Customer bernilai tinggi jumlahnya relatif sedikit namun sangat berpengaruh terhadap total revenue.

### Segmentasi Pelanggan (RFM)  
Distribusi segmen:
- Best Customers: 39%  
- Loyal Customers: 20%  
- Potential Loyalists: 23%  
- At Risk: 18%  

### Dashboard  
Dashboard interaktif dibuat menggunakan Looker Studio dengan KPI utama:
- Total Revenue: £8,89M  
- Total Orders: 18.532  
- Customer Count: 4.338  
- Average Order Value: £479,56  

Visualisasi mencakup:
- Monthly Revenue Trend  
- Revenue by Country  
- Top Products  
- Top Customers  
- Customer Segmentation (RFM)

### Business Recommendations  
1. Retain Best Customers dengan loyalty program dan promo eksklusif.  
2. Re-engage At Risk Customers melalui campaign email marketing dan diskon khusus.  
3. Convert Potential Loyalists menjadi loyal customers melalui strategi bundling produk.  
4. Optimasi stok produk utama berdasarkan Pareto Analysis.  
5. Ekspansi pasar ke negara Eropa selain UK berdasarkan potensi revenue.

### Struktur Folder
Project for BNSP Data Analyst assessment/ 
-> bnsp_data_analyst_analysis.ipynb
-> dataset.csv


### Cara Menjalankan Project  
1. Buka file notebook (.ipynb).  
2. Jalankan cell secara berurutan dari atas ke bawah.  
3. Visualisasi dan insight dapat dilihat langsung di notebook dan dashboard.

---

Project ini menunjukkan proses end-to-end Data Analytics mulai dari data cleaning, exploratory data analysis, segmentasi pelanggan, visualisasi dashboard, hingga rekomendasi bisnis.

