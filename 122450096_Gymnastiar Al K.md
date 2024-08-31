# Tugas VDI – Resume Artikel "Making Data Visualization More Efficient and Effective: A Survey"
Gymnastiar Al Khoarizmy - 122450096 - RC

## Ringkasan Artikel "Making Data Visualization More Efficient and Effective: A Survey" (Qin, 2019)

### 1. Introduction
Bagian Pendahuluan dari artikel ini menyoroti pentingnya visualisasi data dalam dunia bisnis yang semakin bergantung pada data. Seiring dengan meningkatnya volume data, organisasi semakin sering menggunakan visualisasi data untuk membantu proses pengambilan keputusan. Tujuan utama visualisasi data adalah mengubah data yang abstrak menjadi bentuk visual seperti grafik dan diagram, sehingga lebih mudah dipahami oleh analis dan pengambil keputusan dalam memahami data yang kompleks secara intuitif.

Pendahuluan juga menekankan bahwa visualisasi data telah berkembang pesat berkat kontribusi dari beberapa komunitas riset. Komunitas grafis komputer telah meningkatkan teknologi untuk menciptakan visualisasi yang menarik dan mudah dipahami. Komunitas visualisasi berfokus pada pengembangan alat-alat seperti D3.js dan Tableau yang memudahkan desain serta interaksi dengan visualisasi. Komunitas basis data juga berperan dalam memajukan visualisasi data secara real-time, terutama untuk dataset besar.

Artikel ini bertujuan untuk menghadapi tantangan dalam memvisualisasikan dataset besar dengan lebih efisien. Penulis menekankan bahwa peningkatan pada spesifikasi visualisasi dan pemrosesan back-end adalah kunci untuk memastikan visualisasi data lebih cepat dan interaktif.

Survei ini mencakup tiga topik utama:
1. Spesifikasi visualisasi – Cara pengguna menentukan jenis visualisasi yang diperlukan.
2. Teknik visualisasi data yang efisien – Strategi untuk mempercepat pemrosesan data besar.
3. Sistem rekomendasi visualisasi – Metode untuk membantu pengguna menghasilkan visualisasi yang relevan secara otomatis.

### 2. Visualization Specifications
Bagian Visualisasi Spesifikasi dalam artikel tersebut membahas cara-cara yang digunakan pengguna untuk menentukan visualisasi data secara efektif. Ada beberapa poin utama yang disorot:

1. **Data**: 
   - Data yang divisualisasikan disebut records, dan sering kali mengalami transformasi seperti pengelompokan, pengurutan, atau penyaringan sebelum divisualisasikan.
2. **Marks**: 
   - Elemen visual yang mewakili data, seperti batang, garis, atau titik. Tanda-tanda visual ini juga mencakup ukuran, legenda, serta properti tambahan seperti warna dan lebar.
3. **Pemetaan**: 
   - Proses yang menghubungkan data dengan tanda-tanda visual, menciptakan visualisasi yang bermakna.

Bahasa visualisasi dikategorikan berdasarkan tingkat ekspresivitas dan kemudahan penggunaan:
- **Bahasa Tingkat Rendah**: Memerlukan pengguna untuk menentukan elemen pemetaan secara manual, seperti bahasa Vega.
- **Bahasa Tingkat Tinggi**: Menyederhanakan proses dengan menyembunyikan detail teknis, contohnya ggplot2 di R dan Vega-Lite di JavaScript.

Pendekatan berbasis GUI (antarmuka grafis pengguna) seperti Tableau, Excel, dan Power BI menawarkan kemudahan dengan antarmuka visual, memungkinkan pengguna membuat visualisasi tanpa menulis kode.

Terakhir, disebutkan adanya spesifikasi yang kurang rinci (underspecified), di mana sistem visualisasi diharapkan bisa menafsirkan masukan yang kurang jelas dan tetap menyarankan visualisasi yang tepat.

Bagian ini menunjukkan bahwa alat visualisasi dirancang untuk memenuhi berbagai kebutuhan, dari pengguna non-teknis hingga teknis tingkat lanjut.

### 3. Efficient Approaches for Data Visualization
Bagian ini berisi cara-cara efisien untuk memvisualisasikan data karena siklus hidup visualisasi data berulang dan melibatkan manusia aktif dalam proses tersebut. Ada tiga pendekatan utama:

1. **Visualisasi Data yang Tepat (Exact Data Visualization)**: Berkaitan dengan metode untuk secara efisien melakukan visualisasi data yang tepat, biasanya menggunakan teknik database seperti kueri data yang efisien di SQL. Sistem-sistem seperti DeepEye, Polaris, dan SeeDB mengadopsi paradigma ini untuk memberikan solusi visualisasi yang akurat dengan cepat.

2. **Visualisasi Data yang Mendekati (Approximate Data Visualization)**: Ketika data berskala sangat besar atau kompleksitas permintaan sangat tinggi, mungkin tidak mungkin memberikan hasil visualisasi yang tepat. Di sinilah digunakan visualisasi yang mendekati (aproksimasi) untuk memberikan hasil dalam waktu singkat, meskipun mungkin tidak sepenuhnya akurat.

3. **Visualisasi Data Progresif (Progressive Data Visualization)**: Ini merupakan jenis teknik di mana hasil visualisasi diproduksi sedikit demi sedikit, bukannya diperkirakan sekali. Ini memungkinkan pengguna untuk melihat hasil sementara dan mendapatkan gambaran umum sebelum hasil akhir ditampilkan.

Cara-cara ini dimaksudkan untuk mendukung peningkatan efisiensi dan skalabilitas visualisasi data, terutama dalam mengelola data besar dan kompleks.

### 4. Visualization Recommendations
Bagian ini membahas berbagai solusi rekomendasi visualisasi yang bertujuan membantu langkah-langkah berulang dalam menghasilkan visualisasi data. Beberapa pendekatan telah diulas:

1. **Rekomendasi Spesifikasi Terikat**: Sistem rekomendasi ini beroperasi di bawah spesifikasi yang lengkap dan sebagian elemen visualisasi. Dalam kondisi spesifikasi sebagian, sistem merekomendasikan elemen visualisasi berdasarkan model pembelajaran mesin atau aturan. Misalnya, DeepEye menggunakan klasifikasi untuk menilai apakah visualisasi itu baik atau buruk, dan kemudian menggunakan model pembelajaran untuk memberi peringkat visualisasi.

2. **Rekomendasi Berbasis Perilaku**: Teknik ini mengamati perilaku pengguna saat berinteraksi dengan data atau visualisasi untuk memberikan rekomendasi visualisasi yang kontekstual. Sistem terus belajar dari pola perilaku pengguna untuk menyarankan visualisasi yang lebih relevan dengan kebutuhan eksplorasi data mereka.

3. **Rekomendasi Personal**: Sistem ini beroperasi berdasarkan pada preferensi dan kebutuhan individual pengguna. Dengan memanfaatkan riwayat interaksi pengguna serta data pribadi lainnya, sistem ini dapat memberikan rekomendasi visualisasi yang lebih sesuai dengan preferensi pengguna.

Sistematika ini diarahkan pada meningkatkan kinerja dan pengaruh analisis data visualisasi melalui rekomendasi yang relevan dan bermanfaat bagi pengguna.

### 5. Other Research Directions
Bagian ini membahas beberapa ruang penelitian lain yang terlibat dalam memproses data dalam konteks visualisasi, tetapi yang belum mendapatkan perhatian yang cukup:

1. **Pra-Pemrosesan Data untuk Visualisasi Data**: Data yang diekstraksi untuk visualisasi umumnya kotor dan sangat misrepresentatif tanpa pembersihan. Oleh karena itu, normalisasi nilai, deduplikasi, imputasi nilai yang hilang, dan deteksi outlier harus diselesaikan sebelum visualisasi dilakukan. Misalnya, alat seperti Tableau telah mengintegrasikan Trifacta untuk persiapan data.

2. **Benchmark Visualisasi Data**: Sebagaimana benchmark seperti ImageNet telah berguna dalam pengenalan gambar, ada kebutuhan untuk menciptakan benchmarking yang dapat digunakan untuk mengukur kinerja dan rekomendasi dalam visualisasi data. Benchmark ini harus mencerminkan tugas analisis visual yang sebenarnya dan memiliki cakupan serta kualitas label yang baik. Salah satu usaha di bidang ini adalah VizNet, yang bertujuan untuk menyediakan koleksi data besar yang berguna untuk perbandingan teknik desain visualisasi.

3. **Visualisasi Data untuk Aplikasi Berbasis Database**: Visualisasi data sangat penting tidak hanya dalam aplikasi berbasis penyimpanan data, tetapi juga dalam aplikasi berbasis database seperti Microsoft Excel, Google Sheets, dan Microsoft Power BI. Pengembangan teknik visualisasi yang lebih canggih juga dapat digunakan untuk mendukung proses eksplorasi dan debugging data, seperti yang diusulkan dalam sistem Data Civilizer.

### 6. Conclusions
Artikel ini menekankan bahwa visualisasi data adalah bidang yang berkembang pesat, didorong oleh kebutuhan dari berbagai domain dan aplikasi. Meskipun banyak sistem visualisasi data komersial yang ada sudah memudahkan pengguna dalam hal spesifikasi visualisasi, banyak praktisi masih menghadapi masalah efisiensi dan rekomendasi dalam sistem ini. Artikel ini mengidentifikasi beberapa masalah terbuka yang dapat diatasi oleh peneliti basis data untuk memajukan bidang visualisasi data lebih lanjut.
