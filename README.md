# Capstone-Project-Module-2_SaaS-Sales-Analysis

## Ringkasan Project
Projek ini bertujuan untuk melakukan analisis eksploratif (EDA) terhadap dataset penjualan dari sebuah perusahaan SaaS. Analisis menggunakan pendekatan statistik non-parametrik, yaitu tidak mengasumsikan distribusi data normal. Fokus utama adalah pada pola diskon, profitabilitas, kuantitas, dan penjualan.

## Ringkasan Dataset
- Jumlah Observasi: 9.801 baris data.
- Missing Value: 0.
- Kolom Utama: Sales, Quantity, Discount, Profit.
- 
## Statistik Deskriptif 
| Statistik     | Sales     | Quantity | Discount | Profit    |
|---------------|-----------|----------|----------|-----------|
| Jumlah Data   | 9.801     | 9.801    | 9.801    | 9.801     |
| Median        | 51.84     | 3        | 0.15     | 8.80      |
| IQR           | 187.10    | 3.0      | 0.2      | 273.88    |
| Min - Max     | 0.44–11.199| 1–14    | 0–0.8    | -1.67–4.630|
| Skewness      | 7.6       | 1.17     | 1.75     | 10.64     |
| Nilai Nol     | 0         | 0        | 4.769    | 65        |
Notes: karena skewness tinggi dan outlier ekstrim menggunakan IQR sebagai ukuran utama penyebaran.

## Insight: 
- Hampir setengah dari transaksi (47%) dilakukan tanpa pemberian diskon (diskon = 0).
- Distribusi profit right-skewed, banyak transaksi dengan profit kecil atau rugi.
- Ditemukan nilai profit negatif, menunjukkan adanya potensi masalah dalam strategi harga atau diskon.
- Visualisasi scatter plot menunjukkan tren negatif antara diskon dan profit.
- Wilayah EMEA (Europe, Middle East, Africa) dan AMER (Americas) unggul dalam profitabilitas dibandingkan wilayah lain.
- Industri Finance, Healthcare, dan Manufacturing memiliki profit rata-rata lebih tinggi, sedangkan Communications dan Miscellaneous mendekati nol.
- Segmen SMB (UMKM) mendominasi volume penjualan.

## Alat yang Digunakan: 
- Python: Pandas, Matplotlib, Seaborn, SciPy Stats
- Tableau: Untuk dashboard interaktif
- Statistik Non-Parametrik: Median & IQR, Kruskal-Wallis & Mann-Whitney, Deteksi outlier dengan metode IQR.
