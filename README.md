# Latar Belakang
Sebuah Perusahaan SaaS (Software as a Service) ingin mengetahui performa bisnis untuk mengukur kinerja bisnis, menemukan tren, dan membuat keputusan strategis yang tepat.

# Pernyataa Masalah
Bagaimana tren penjualan dan keuntungan dari waktu ke waktu?
Produk mana yang paling banyak terjual dan paling menguntungkan?
Wilayah (Region) dan subwilayah (Subregion) mana yang memberikan kontribusi    penjualan dan keuntungan terbesar?
Segmen dan Industri pelanggan mana yang paling menguntungkan?
Bagaimana hubungan antara diskon yang diberikan dengan penjualan dan keuntungan?
Top 10 Customer yang memberikan kontribusi keuntungan terbesar?

# Data Understanding and Data Cleaning
Sebelum menganalisis lebih lanjut terkait dataset, tahapan pertama yang harus dilakukan adalah memahami dataset atau Data Understanding. Kita perlu mendapatkan gambaran menyeluruh tentang data yang kita miliki. Tujuannya untuk memahami struktur, isi, dan kualitas data. Dalam proses ini kita dapat mengetahui apakah data yang kita memiliki terdapaat data yang ambigu yang menyebabkan sumber anomali data atau anomali sebagai penyebab ambiguitas dan lain sebagainnya. Keduanya menunjukkan masalah kualitas data yang perlu ditangani melalui proses data cleaning
Secara garis besar, informasi yang terdapat pada dataset ini sebagai berikut:
1. Data set ini memilikin 19 kolom dan 9994 baris
2. Terdapat 3 kolom yang mengalami kesalahan tipe data yaitu Row ID yang merupakan* integer* yang seharusnya *string*, Order Date yang merupakan object yang seharus *datetime* dan Customer ID yang merupakan* integer* yang seharusnya *string*
3. Tidak adanya Data yang kosong pada dataset ini
4. Ada data yang menunjukkan tentang waktu, bisa dibuatkan kolom baru berdasarkan tahun dan bulannya untuk memudahkan analisis
5. Terdapat kolom Row ID yang merupakan ID unik untuk setiap transaksi, sehingga tidak relevan dalam analisis dan bisa dihapus saja.
6. Terdapat kolom Date Key yang merupakan Representasi numerik dari tanggal pesanan (YYYYMMDD), sehingga tidak relevan dalam analisis dan bisa dihapus saja.
7. Terdapat kolom License yang merupakan Kunci lisensi untuk produk, sehingga tidak relevan dalam analisis dan bisa dihapus saja.

# Data Analisis

## Korelasi antar variabel

Diperlakukanya informasi terkait korelasi antar variabel untuk memahami apakah ada hubungan antara dua atau lebih variabel.

## Tren Penjualan dan Keuntungan
1. Secara keseluruhan, bisnis menunjukkan tren pertumbuhan penjualan yang positif dan berkelanjutan sejak tahun 2022, menunjukkan keberhasilan dalam meningkatkan akuisisi atau retensi pelanggan.
2. Tren Profit menunjukkan bahwa, selain peningkatan volume penjualan, perusahaan juga berhasil meningkatkan efisiensi margin secara signifikan pada tahun 2023. Perusahaan semakin mahir dalam menjaga biaya atau mengalihkan penjualan ke produk dengan margin keuntungan lebih tinggi

## Tren Penjualan dan Keuntungan Berdasarkan Produk
Produk 'ContactMatcher' memiliki volume penjualan tertinggi, namun produk 'Alchemy' dan 'Site Analytics' menunjukkan profit yang lebih signifikan. Ini mengindikasikan bahwa produk dengan penjualan tertinggi belum tentu yang paling menguntungkan.Perusahaan juga harus memerhatikan produk Data Smasher dan Support karena biarpun berada di posisi 3 dan 4 tapi 2 produk ini memiliki profit margin tertinggi sebesar 25% dan 26%

## Tren Penjualan dan Keuntungan Berdasarkan Wilayah
AMER adalah Regional yang paling dominan secara absolut. Subregion NAMER (Amerika Utara) menduduki puncak daftar sebagai penyumbang terbesar baik dalam penjualan maupun keuntungan.Perusahaan dapat berfokus untuk mengembangkan produk Marketing Suite,Alchemy, Data Smasher, dan Big Ol Database untuk tahun 2024.Wilayah EMEA (Eropa, Timur Tengah, dan Afrika) secara keseluruhan adalah kontributor profit terbesar kedua perusahaan dapat berfokus untuk mengembangkan produk Marketing Suite,Alchemy,Site Analytics OneView, dan Big Ol Database untuk tahun 2024.Sedangkan di posisi ketiga ada IPJ ,Marketing Suite,Alchemy, Site Analytics, SaaS Connector Pack - Gold dan Big Ol Database untuk tahun 2024  

## Tren Penjualan dan Keuntungan Berdasarkan Segmen dan Industri
Segment SMB merupakan segmen yang paling menguntungkan dan memiliki penjualan tertinggi tetapi segment strategic memilik margin profit tertinggi. Industri Finance adalah konstribusi keuntungan tertinggi pada sektor SMB, perusahaan harus secara agresif menargetkan industri Energy dan Manufacturing karena mereka adalah top 3 teratas pada segmen SMB.

## Tren Penjualan dan Keuntungan Berdasarkan Diskon
Transaksi Tanpa Diskon adalah Kunci Profit.Strategi penjualan harus dioptimalkan untuk memaksimalkan transaksi harga penuh (0.00). Hentikan Diskon > 20%. Gunakan diskon 10-15% secara sangat selektif dan bertarget (misalnya, untuk pelanggan yang hampir churn atau untuk mempercepat penutupan di akhir kuartal), tetapi jangan menjadikannya sebagai praktik standar

## Top 10 Customers
Valero Energy adalah customer yang paling menguntungkan. Meskipun Valero Energy memiliki Profit tertinggi, tetapi Coca-Cola memiliki Profit margin  tinggi diantara 3 customer teratas.


## Kesimpulan dan Rekomendasi
Kesimpulan
1. Tren pertumbuhan penjualan dan keuntungan yang positif dan berkelanjutan
2. Produk 'ContactMatcher' memiliki volume penjualan tertinggi, namun produk 'Alchemy' dan 'Site Analytics' menunjukkan profit yang lebih signifikan. Ini mengindikasikan bahwa produk dengan penjualan tertinggi belum tentu yang paling menguntungkan.
Perusahaan juga harus memerhatikan produk Data Smasher dan Support karena biarpun berada di posisi 3 dan 4 tapi 2 produk ini memiliki profit margin tertinggi sebesar 25% dan 26%
3.  AMER adalah Regional yang paling dominan secara absolut. Subregion NAMER (Amerika Utara) menduduki puncak daftar sebagai penyumbang terbesar baik dalam penjualan maupun keuntungan.Perusahaan dapat berfokus untuk mengembangkan produk Marketing Suite,Alchemy, Data Smasher, dan Big Ol Database untuk tahun 2024.
4. Pertahankan fokus pada SMB untuk volume sales dan Profit terbesar.Industri Finance adalah konstribusi keuntungan tertinggi pada sektor SMB. Segment Strategic memiliki margin profit tertinggi
5. Transaksi Tanpa Diskon adalah Kunci Profit. Diskon 10-15% masih menguntungkan. Hentikan Diskon > 20.
6. Valero Energy adalah asset paling berharga bagi perusahaan. 

Rekomendasi

1. Secara General :
* Peluncuran produk baru
* Perubahan tim Sales atau kompensasi.
* Fokus pada region atau segmen tertentu.
  
2. Aksi yang dilakukan:
* Perusahaan dapat mengalokasikan sumber daya Riset & Pengembangan (R&D) dan dukungan teknis terbaik untuk mengembangkan produk
* Pelajari dan dokumentasikan faktor-faktor yang mendorong margin tinggi
* Gunakan Strategi Bundling produk
    
3. Lakukan forecasting dan manajemen risiko yang ketat di NAMER. Fokus pada perkembangan produk.Mengaudit dan Mengoptimalkan Pasar Volume Rendah dan Margin Rendah (EMEA & APJ) dengan aksi yang direkomendasikan sebagai berikut:
* Tinjau kembali struktur diskon
* Gunakan Strategi Bundling produk
  
4. * Kembangkan produk add-on pada segmen SMB
   * Mengoptimalkan Segmen Strategic (Kualitas):
   * Mengalokasikan Tim terbaik
   * Monetisasi Nilai Tambah seperti mengembangkan dan pasarkan fitur atau layanan yang berbasis nilai, bukan harga.
     
5. Aksi yang dilakukan:
   * Hentikan segera pemberian diskon di atas 20% dalam kebijakan penjualan
   * Fokuskan pemasaran dan pelatihan Sales pada nilai produk
   * Gunakan diskon 10%–15% masih efektif dalam profit
7. Aksi yang dilakukan:
   * Terapkan program akun priotitas customer dan memberikan fasilitas terbaik
   * Analisis produk apa yang dibeli oleh Top 10 ini. Jika mereka banyak membeli produk dengan profit, maka dorong mereka untuk mengadopsi produk terkait yang juga memiliki profit tinggi. Jika mereka   membeli produk dengan profit rendah, maka kembangkan paket bundling yang mendorong mereka ke produk premium/margin tinggi.
   * Lacak tingkat keterlibatan (engagement) dari Top 10 secara proaktif. Apakah kehilangan satu dari mereka  dapat berdampak negatif yang lebih besar daripada kehilangan ratusan pelanggan kecil.






