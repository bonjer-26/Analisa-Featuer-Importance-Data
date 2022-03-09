# Analisa-Feature-Importance-Data
Analisa Data Sosiodemografi pada sektor perhotelan

LATAR BELAKANG

Salah satu sektor yang paling terdampak dari kondisi pandemi Covid-19 adalah sektor perhotelan. Dimana penetapan kebijakan pembatasan pergerakan di seluruh wilayah provinsi Jawa Barat telah memutus rantai perekonomian kegiatan sektor perhotelan. Sektor perhotelan sendiri merupakan salah satu penyumbang sumber pendapatan asli daerah yang utama bersamaan dengan sektor pariwisata. Penurunan jumlah pendapatan asli daerah (PAD) pada sektor perhotelan terjadi sejak tahun 2018 hingga 2020. Selain itu, perbedaan kondisi dan karakterisiktik dari tiap wilayah kabupaten/kota di provinsi Jawa Barat merupakan tantangan tersendiri dalam penentuan kebijakan dan pengambilan keputusan yang tepat. Dalam rangka meningkatkan pemahaman terhadap kondisi sektor perhotelan di wilayah provinsi Jawa Barat, penulis mencoba melakukan analisa pemodelan sektor perhotelan dari sisi informasi data sosiodemografi.

TUJUAN

•Membuat analisa pemodelan sektor perhotelan berdasarakan sumber data sosiodemografi wilayah provinsi Jawa Barat
•Menentukan variabel pendukung yang berkontribusi positif dan negatif terhadap perkembangan sektor perhotelan di wilayah Provinsi Jawa Barat

BATASAN MASALAH

•Data secara umum merupakan informasi sosiodemografi provinsi Jawa Barat
•Data tersedia dalam kategori spasial pada tingkat level Kabupaten/Kota
•Data tersedia pada rentang tahunan pada periode 2014 – 2020
•Banyak terdapat kekosongan informasi dengan kondisi laporan tidak lengkap
•Informasi target (Dependant Variable) dibatasi pada besar Jumlah Pendapatan Asli Daerah (PAD) dari sektor Perhotelan
•Informasi pemodelan (Independent Variables) menggunakan 104 jenis fitur pendukung

SUMBER DATA PENGOLAHAN

Sumber data yang digunakan berasal dari berbagai sumber data baik dari yang disediakan oleh tim panitia Turnamen Sains Data Nasional 2021 maupun sumber data eksternal lainnya dengan rincian sebagaimana table di bawah ini. Penentuan pemilihan sumber data yang digunakan pada mengacu pada rincian batasan masalah.

PROSES PENGOLAHAN DATA

Environment aplikasi yang digunakan:

1. Python 3.7.6
2. Tableau Desktop
3. IDE: Jupyter Notebook

Library yang digunakan:

1. Numpy
2. Pandas
3. Sklearn
4. XGBOOST
5. Matplotlib
6. Seaborn
7. Jupyter Nbextensions
8. J.COP Snippets
9. Shapley Additive Explanationm (SHAP)

INTERPRETASI HASIL

Dalam hal melakukan interpretasi hasil, kami menggunakan parameter nilai SHAP untuk melihat kontribusi dari ke-22 fitur sampel terhadap total Pendapatan Asli Daerah (PAD) dari sektor perhotelan di tiap lokasi Kabupaten/Kota provinsi Jawa Barat. Shapley Additive Explanations (SHAP) adalah metode yang diperkenalkan oleh Lundberg dan Lee pada tahun 2017 untuk interpretasi prediksi model Machine Learning melalui nilai Shapely.

Dengan menggunakan informasi sebagaimana terlampir pada slide sebelumnya, kita akan mencoba melakukan analisa kontribusi nilai SHAP terhadap nilai PAD di wilayah Kabupaten Kuningan. 

Berdasarkan dari distribusi nilai SHAP, nilai pendapatan asli daerah dari sektor perhotelan didominasi oleh beberapa faktor:
Faktor pertama didominasi oleh Jumlah Restoran, dalam hal ini secara statistik wilayah tersebut memiliki potensi kuliner yang cukup baik. Dalam menghadapi kondisi pandemic sektor perhotelan memiliki potensi yang baik untuk bertransformasi ke bisnis kuliner. Sektor kuliner dan rumah makan merupakan sektor yang paling bertahan selama kondisi pandemi, sehingga untuk tetap mampu menjalankan operasional hotel sebaiknya sektor perhotelan juga mampu berpartisipasi dalam bisnis kuliner dengan memanfaatkan kemudahan berbagai channel yang sudah tersedia seperti; delivery system, logistic, order, dan drive-thru.

Faktor kedua dipengaruhi oleh Jumlah Pengujung Museum. Melalui output ini, secara statistik dapat menunjukkan destinasi wisata museum menjadi salah satu obyek wisata yang memberikan kontribusi positif di wilayah tersebut.
Faktor ketiga dipengaruhi oleh Jumlah Kendaraan Pribadi jenis Sedan, Jeep, Minibus. Melalui output ini dapat diperkirakan kebutuhan dari lahan parkir dan akses jalan akan mampu meningkatkan sektor perhotelan pada wilayah tersebut
Apabila kita melihat ke sisi sebaliknya, fitur JML_HT (Jumlah Hotel Bintang) memberikan kontribusi negative sangat dominan. Melalui output ini dapat diinterpretasikan bahwa keberadaan jumlah hotel bintang tidak memberikan kontribusi positif terhadap sektor perhotelan. Untuk menganalisa lebih jauh kita dapat melihat fitur-fitur lain yang mungkin berpengaruh terhadap hal tersebut seperti, range harga yang tidak sesuai, review yang kurang baik, dan lainnya.

Selain itu juga diberikan informasi mengenai kondisi pergerakan (mobility) penduduk pada tiap wilayah dari beberapa sumber eksternal. Melalui informasi ini kita dapat melihat bahwa peningkatan intensitas pergerakan penduduk menunjukkan kondisi positif terhadap recovery sektor perhotelan dari kondisi pandemic. Namun perlu diantisipasi bahwa kondisi pandemic atau hal serupa juga dapat terjadi di masa mendatang.


KESIMPULAN

Keberagaman kondisi sosiodemografi dari tiap wilayah Kabupaten/Kota di Provinsi Jawa Barat membutuhkan kebijakan dan pengambilan keputusan yang spesifik dari tiap wilayah. Dengan menggunakan Dashboard Analisa Feature-Importance Data Sosiodemografi di Wilayah Provinsi Jawa Barat, melalui pemanfaatan distribusi nilai parameter SHAP dari model yang dihasilkan, kita dapat menentukan komponen mana yang paling dominan dan berpengaruh dari tiap wilayah lokasi Kabupaten/Kota.

Melalui penilaian ini kita dapat menentukan komponen apa saja yang menjadi perhatian dalam melakukan analisa lebih jauh, penentuan kebijakan serta pengambilan keputusan yang lebih baik dalam rangka meningkatkan potensi sektor perhotelan dari tiap wilayah Kabupaten/Kota di provinsi Jawa Barat.











