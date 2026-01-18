# Project Background
Perusahaan ABC merupakan perusahaan yang menjual berbagai jenis kopi. Untuk mendukung pengambilan keputusan strategis, dilakukan analisis performa penjualan pada periode 2019–2022 guna memahami tren penjualan tahunan serta membandingkan kontribusi dan karakteristik performa antarjenis kopi. Selain itu, analisis ini juga mengevaluasi negara yang memberikan kontribusi terbesar terhadap total pendapatan perusahaan.

Berdasarkan hasil analisis, insight dan rekomendasi difokuskan pada dua area utama berikut.

* **Product Performance Insight:** Mengkaji pola pergerakan profit sepanjang tahun 2019–2022, termasuk identifikasi jenis kopi yang paling menguntungkan serta perannya dalam mendorong kenaikan dan penurunan penjualan bulanan, ditinjau dari volume order dan jumlah pelanggan aktif.
* **Customer Behavior Insight:** Menganalisis kontribusi profit berdasarkan negara serta dinamika jumlah pelanggan dari tahun ke tahun.

Worksheet Google Sheets dapat diakses melalui tautan berikut:
[link](https://docs.google.com/spreadsheets/d/1wa8ulH8iiOfSBkyEJqEhBvSGMDcTD60xle7uKJ-6DBw/edit?usp=sharing)

Dashboard Google Looker Studio dapat diakses melalui tautan berikut:
[Link](https://lookerstudio.google.com/reporting/24316dd9-a3ca-4905-8a62-c4709229a965)

## Data Description
Dataset ini terdiri atas 1.000+ baris data dan terbagi ke dalam tiga tabel/worksheet, yaitu **Orders**, **Customers**, dan **Products**.

* **Customers:** Tabel ini berisi data pelanggan yang mencakup identitas pelanggan serta berbagai atribut pendukung (seperti nama dan informasi kontak). Data ini digunakan untuk analisis segmentasi dan perilaku pelanggan.

* **Orders:** Tabel ini merepresentasikan transaksi pemesanan kopi. Setiap order dicatat dengan informasi tanggal pemesanan dan terhubung ke satu pelanggan, sehingga menggambarkan satu aktivitas pembelian oleh pelanggan.

* **Products:** Tabel ini menyimpan data master produk kopi yang mencakup karakteristik produk, informasi ukuran, harga, serta profitabilitas. Tabel ini digunakan untuk analisis performa produk dan kontribusinya terhadap penjualan dan profit.

# Executive Summary

## Overview of Findings
Antara tahun 2019 dan 2022, total penjualan mencapai $45.13K dengan profit sebesar $1.30K dari 3.551 unit yang terjual kepada 913 pelanggan, menunjukkan bahwa pertumbuhan pendapatan tidak diimbangi oleh profitabilitas yang kuat. Kontribusi profit terbesar didorong oleh Liberica dan Excelsa (~66% profit), sementara Arabica dan Light Roast, meskipun memimpin dalam volume penjualan, menghasilkan profit relatif rendah (~34% profit)

Kinerja penjualan mencapai puncaknya pada 2021 sebelum menurun tajam pada 2022 (profit turun sekitar 42,3%), menunjukkan adanya masalah dalam retensi dan loyalitas pelanggan. Dari aspek geografis, profit sangat terkonsentrasi di pasar AS ($1.013), dengan kontribusi minimal dari Irlandia dan Inggris, menunjukkan ketergantungan pada satu pasar dan peluang pertumbuhan regional yang belum termanfaatkan.

# Insights Deep Dive
## **Products Performance Insight:**
- Penjualan tinggi tetapi profit rendah, mengindikasikan masalah pada pricing atau cost structure.
- Penurunan penjualan pada 2022 (profit turun sekitar 42,3%) sejalan dengan penurunan jumlah customer serta turunnya pembelian kopi Liberika (~36,15% profit) dan Excelsa (~29.82% profit), yang mengindikasikan potensi masalah pada promosi atau ketersediaan stok kedua produk tersebut.
- Arabica dan Robusta mendominasi kuantitas penjualan tetapi menghasilkan profit rendah (sekitar 34,0% dari total profit), mengindikasikan isu pricing atau margin.

<p align="center">
  <kbd><img src="image/1.jpg" width=800px> </kbd> <br>
  Products Dashboard
</p>


##  **Customers Dashboard**
- Penurunan jumlah customer yang signifikan pada September menyebabkan penurunan penjualan pada periode yang sama (profit turun sekitar 42,3%), mengindikasikan masalah engagement atau retensi.
- Amerika Serikat merupakan negara dengan profit tertinggi (sekita 77.9% dari total profit), namun terdapat kesenjangan profit yang besar antar negara, mengindikasikan konsentrasi penjualan yang tinggi di pasar AS.

<p align="center">
  <kbd><img src="image/2.jpg" width=800px> </kbd> <br>
  Customers Dashboard
</p>

# Recommendations: 
Berdasarkan insight dan temuan yang telah dijelaskan, beberapa rekomendasi yang dapat dilakukan adalah:
1. Optimasi pricing dan margin per produk
Tinjau kembali strategi pricing dan cost structure, khususnya untuk Arabica dan Robusta yang memiliki volume tinggi namun profit rendah, guna meningkatkan margin tanpa mengorbankan permintaan.

2. Prioritaskan produk ber-margin tinggi
Perkuat fokus pada Liberika dan Excelsa melalui penyesuaian alokasi stok dan aktivitas promosi, mengingat kedua produk merupakan kontributor profit utama dan mengalami penurunan penjualan di 2022.

3. Perbaikan strategi retensi dan engagement customer
Evaluasi efektivitas program loyalty card yang saat ini belum optimal, dan pertimbangkan penguatan insentif repeat purchase untuk menekan penurunan jumlah customer, terutama pada periode kritis seperti September.

4. Mitigasi risiko konsentrasi pasar (opsional tapi kuat)
Kurangi ketergantungan pada pasar Amerika Serikat dengan mengembangkan strategi pemasaran bertahap di negara lain yang saat ini berkontribusi rendah terhadap profit.
