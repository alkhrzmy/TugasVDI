# Tugas VDI – Resume Artikel "Making Data Visualization More Efficient and Effective: A Survey"
Gymnastiar Al Khoarizmy - 122450096 - RC
### 1. Introduction
Dalam dunia bisnis yang semakin bergantung pada data, artikel ini menekankan betapa pentingnya visualisasi data. Dengan semakin bertambahnya volume data, organisasi kini lebih sering memanfaatkan visualisasi data sebagai alat bantu untuk proses pengambilan keputusan. Mengubah data yang abstrak menjadi bentuk visual seperti grafik dan diagram merupakan tujuan utama dari visualisasi data, agar analis dan pengambil keputusan dapat dengan mudah memahami data yang kompleks secara intuitif.

Selain itu, dalam pendahuluan juga disorot bahwa pertumbuhan visualisasi data terjadi secara signifikan berkat sumbangan dari beberapa komunitas riset. Teknologi yang digunakan oleh komunitas grafis komputer telah ditingkatkan untuk menciptakan visualisasi yang menarik dan mudah dipahami. Fokus dari komunitas visualisasi adalah untuk mengembangkan alat-alat seperti D3. js dan Tableau membantu dalam desain serta interaksi dengan visualisasi. Komunitas basis data juga ikut berpartisipasi dalam meningkatkan visualisasi data secara real-time, terutama untuk dataset yang memiliki ukuran besar.

Tujuan dari artikel ini adalah untuk mengatasi tantangan dalam melakukan visualisasi data yang besar dengan lebih efektif. Penulis menyatakan bahwa untuk memastikan visualisasi data lebih cepat dan interaktif, penting bagi kita untuk fokus pada peningkatan spesifikasi visualisasi dan pemrosesan back-end.

Survei ini mencakup tiga topik utama:

1. Spesifikasi visualisasi – Bagaimana cara pengguna menentukan jenis visualisasi yang mereka perlukan.
2. Metode efisien dalam visualisasi data - Langkah-langkah untuk meningkatkan kecepatan pemrosesan jumlah data yang besar.
3. Metode sistem rekomendasi visualisasi digunakan untuk membantu pengguna dalam menghasilkan visualisasi secara otomatis yang sesuai dengan kebutuhan mereka.

### 2. Visualization Specifications
Dalam artikel tersebut, ada pembahasan mengenai metode-metode yang dapat digunakan oleh pengguna untuk memperoleh visualisasi data yang efektif di bagian Visualisasi Spesifikasi. Ada beberapa poin utama yang disorot:Ada beberapa poin utama yang disorot:

1. **Data**:
- Data yang dikonversi ke dalam bentuk visualisasi disebut sebagai records, dan seringkali mengalami proses transformasi seperti pengelompokan, pengurutan, atau penyaringan sebelum dihasilkan visualisasinya.
2. **Marks**:
- Beberapa bentuk visual yang dapat mewakili data, seperti garis, batang, atau titik. Elemen-elemen visual ini juga meliputi ukuran, legenda, serta atribut tambahan seperti warna dan lebar.
3. **Pemetaan**:
- Dengan menghubungkan data dengan tanda-tanda visual, kita dapat menciptakan visualisasi yang memiliki makna.

Bahasa visualisasi dikategorikan berdasarkan tingkat ekspresivitas dan kemudahan penggunaan:Bahasa visualisasi dikategorikan berdasarkan tingkat ekspresivitas dan kemudahan penggunaan:
- **Bahasa Tingkat Rendah**: Pengguna diminta untuk secara manual menentukan elemen pemetaan, seperti dalam Bahasa Vega.
- **Bahasa Tingkat Tinggi**: Proses dapat disederhanakan dengan mengaburkan detail teknis, seperti yang dilakukan oleh ggplot2 di R dan Vega-Lite di JavaScript.

Pendekatan yang menggunakan GUI seperti Tableau, Excel, dan Power BI menyediakan kemudahan bagi pengguna karena antarmuka visualnya yang memungkinkan pembuatan visualisasi tanpa perlu menulis kode.

Pada akhirnya, disebutkan adanya kekurangan spesifikasi yang rinci (lack of detailed specifications), di mana sistem visualisasi diminta untuk mampu menafsirkan masukan yang ambigu dan tetap memberikan saran visualisasi yang sesuai.

Bagian ini menunjukkan bahwa alat visualisasi didesain untuk memenuhi berbagai keperluan, mulai dari pengguna yang tidak memiliki latar belakang teknologi hingga mereka yang memiliki kemampuan teknis tingkat tinggi.

### 3. Efficient Approaches for Data Visualization
Di bagian ini, kami menjelaskan teknik-teknik yang efisien untuk memvisualisasikan data karena visualisasi data merupakan proses berulang dan melibatkan partisipasi aktif manusia. Ada tiga pendekatan utama:

1. **Visualisasi Data yang Tepat (Exact Data Visualization)**: Untuk secara efisien melakukan visualisasi data yang tepat, sering kali digunakan teknik database seperti kueri data yang tidak memberatkan SQL. DeepEye, Polaris, dan SeeDB mengadopsi pendekatan ini untuk menyajikan solusi visualisasi yang akurat dengan efisiensi tinggi.

2. **Visualisasi Data yang Mendekati (Approximate Data Visualization)**: Jika data memiliki skala yang sangat besar atau permintaan memiliki tingkat kompleksitas yang sangat tinggi, mungkin sulit untuk menghasilkan visualisasi yang akurat. Di sini, visualisasi yang hampir mendekati (aproksimatif) digunakan untuk memberikan hasil dalam waktu singkat, meski mungkin tidak sepenuhnya akurat.

3. **Visualisasi Data Progresif (Progressive Data Visualization)**: Ini adalah jenis teknik di mana hasil visualisasi dibuat secara bertahap, bukan diprediksi sekaligus. Pengguna dapat melihat hasil sementara dan mendapatkan gambaran umum sebelum tampilannya menjadi hasil akhir.

Penjelasan ini bertujuan untuk memberikan dukungan dalam meningkatkan efisiensi dan skalabilitas visualisasi data, terutama ketika mengelola data yang besar dan kompleks.

### 4. Visualization Recommendations
Bagian ini berfokus pada solusi rekomendasi visualisasi yang bertujuan untuk membantu dalam menghasilkan langkah-langkah berulang dalam membuat visualisasi data. Beberapa pendekatan telah diulas:

1. **Rekomendasi Spesifikasi Terikat**: Sistem rekomendasi ini berjalan dengan menggunakan spesifikasi yang lengkap dan beberapa elemen visualisasi. Dalam beberapa kondisi spesifikasi, sistem dapat merekomendasikan elemen visualisasi berdasarkan model pembelajaran mesin atau aturan. Contohnya, DeepEye menerapkan klasifikasi untuk mengevaluasi kebaikan atau keburukan visualisasi, serta menggunakan model pembelajaran untuk memberikan peringkat pada visualisasi tersebut.

2. **Rekomendasi Berbasis Perilaku**: Metode ini mengobservasi tindakan pengguna saat berinteraksi dengan data atau visualisasi guna memberikan saran visualisasi yang sesuai dengan konteks. Sistem belajar secara kontinu dari pola perilaku pengguna untuk memberikan rekomendasi visualisasi yang lebih relevan bagi eksplorasi data mereka.

3. **Rekomendasi Personal**: Sistem ini beroperasi sesuai dengan preferensi dan kebutuhan individual pengguna. Sistem ini bisa memberikan rekomendasi visualisasi yang lebih sesuai dengan preferensi pengguna berdasarkan riwayat interaksi pengguna dan data pribadi lainnya.

Tujuan dari sistematika ini adalah meningkatkan kinerja dan pengaruh analisis data visualisasi dengan memberikan rekomendasi yang relevan serta bermanfaat bagi pengguna.

### 5. Other Research Directions
Bagian ini membahas beberapa ruang penelitian lain yang terlibat dalam memproses data dalam konteks visualisasi, tetapi yang belum mendapatkan perhatian yang cukup:Bagian ini membahas beberapa ruang penelitian lain yang terlibat dalam memproses data dalam konteks visualisasi, tetapi yang belum mendapatkan perhatian yang cukup:

1. **Pra-Pemrosesan Data untuk Visualisasi Data**: Tanpa melakukan pembersihan, data yang diambil untuk tujuan visualisasi cenderung kotor dan memberikan gambaran yang sangat salah. Sehingga, sebelum melakukan visualisasi, perlu dilakukan normalisasi nilai, deduplikasi data, imputasi data yang hilang, serta deteksi outlier. Contohnya, alat seperti Tableau sudah menggabungkan Trifacta dalam proses persiapan data.

2. **Benchmark Visualisasi Data**: Sama seperti bagaimana ImageNet bermanfaat dalam pengenalan gambar, diperlukan benchmarking yang dapat digunakan untuk mengukur kinerja dan memberikan rekomendasi dalam visualisasi data. Tugas analisis visual yang sebenarnya harus tercermin dalam benchmark ini, dengan cakupan dan kualitas label yang baik. Satu upaya dalam bidang ini adalah VizNet, yang berupaya untuk mengumpulkan sejumlah besar data yang bermanfaat bagi perbandingan teknik desain visualisasi.

3. **Visualisasi Data untuk Aplikasi Berbasis Database**: Visualisasi data memiliki pentingan yang besar, bukan hanya dalam aplikasi penyimpanan data tetapi juga pada aplikasi database seperti Microsoft Excel, Google Sheets, dan Microsoft Power BI. Selain itu, metode visualisasi yang lebih maju juga bisa dimanfaatkan untuk memfasilitasi eksplorasi dan pemecahan masalah data, seperti yang diproposikan dalam sistem Data Civilizer.

### 6. Conclusions
Dalam artikel ini menekankan betapa pesatnya perkembangan bidang visualisasi data yang didorong oleh berbagai kebutuhan dari domain dan aplikasi yang berbeda. Walaupun banyak sistem visualisasi data komersial yang ada telah memberikan kemudahan kepada pengguna dalam spesifikasi visualisasi, masih banyak praktisi yang mengalami kesulitan dalam hal efisiensi dan rekomendasi di dalam sistem ini. Dalam artikel ini, beberapa masalah terbuka yang dapat dihadapi oleh peneliti basis data akan dikemukakan agar bidang visualisasi data dapat berkembang lebih jauh.
