# Prediksi-Analytics-Prediksi-Harga-Berlian
## Pendahuluan: Predictive Analytics
Peningkatan penggunaan internet di seluruh dunia menghasilkan data dalam jumlah yang sangat besar. Berbagai perangkat cerdas dan internet membuat data menjadi berlimpah. Perusahaan dan organisasi mengumpulkan data berjumlah besar untuk berbagai kepentingan, salah satunya proses pengambilan keputusan.

Supaya memberikan manfaat dan dapat digunakan untuk membuat keputusan, data harus melalui proses analisis dan ekstraksi informasi (insight). Mengekstrak informasi dari data adalah inti dari pekerjaan data analytics. Predictive analytics, pokok bahasan dalam modul ini merupakan sub-bidang data analytics.

Dalam artikel berjudul “Competing on Analytics” yang diterbitkan oleh Harvard Business Review, Davenport, seorang ahli business analytics berpendapat bahwa senjata strategis di bidang bisnis saat ini adalah pengambilan keputusan analytics. Ia merupakan teknik pengambilan keputusan berdasarkan berbagai informasi yang diekstrak dari data.

Bagaimana data diubah menjadi informasi kemudian menghasilkan keputusan diilustrasikan dalam gambar berikut [19].

<p align="center">
  <a href='https://www.dicoding.com/academies/319/tutorials/16989#'><img src="https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:da94bb2d58d5b75d024504e73cbc45fe20210910103332.png"></a>
</p>


Saat mendengar istilah data analytics, Anda mungkin bertanya-tanya, apa bedanya istilah analytics dan analysis

Meskipun kedua istilah ini sering digunakan secara bergantian (interchangeably), keduanya tidaklah sama. Delen dalam “Predictive Analytic: Data Mining, Machine Learning and Data Science for Practitioners” [20] menyatakan, analisis mengacu pada proses pemisahan seluruh masalah menjadi bagian-bagian untuk diperiksa secara rinci dan --jika perlu-- diperbaiki. Setelah proses pemeriksaan dan perbaikan selesai, seluruh sistem dapat dipadukan kembali.

Sementara itu, analytics mencakup berbagai metode, teknologi, dan alat untuk menciptakan informasi baru demi memecahkan permasalahan kompleks serta membuat keputusan yang lebih baik. Analytics merupakan pendekatan multidisiplin yang memanfaatkan data dan model matematika untuk memahami berbagai situasi yang kompleks. Proses analisis merupakan salah satu cakupan dari tahapan analytics.

Pertanyaan selanjutnya adalah, apa itu predictive analytics? Predictive analytics adalah bidang terapan yang menggunakan berbagai metode kuantitatif untuk membuat prediksi dengan memanfaatkan data. Ia merupakan seni membangun serta menggunakan model prediksi berdasarkan pola data historis. Dikutip dari Delen [20], beberapa contoh penggunaan predictive analytics, antara lain:

1. Prediksi Harga
Organisasi bisnis seperti jaringan hotel, maskapai penerbangan, dan bisnis penjualan daring perlu terus-menerus menyesuaikan harga mereka untuk memaksimalkan keuntungan. Perusahaan harus bisa meningkatkan atau mempertahankan pendapatan dan profit meski menghadapi situasi yang sulit. Situasi sulit ini bisa disebabkan oleh berbagai faktor, antara lain perubahan musim, pergeseran permintaan pelanggan, dan terjadinya kejadian khusus seperti pandemi.

2. Model predictive analytics dapat dilatih untuk memprediksi harga optimal berdasarkan data atau catatan historis penjualan. Perusahaan kemudian dapat menggunakan prediksi ini sebagai masukan untuk menentukan berbagai keputusan bisnis, misalnya strategi penetapan harga.


3. Prediksi Dosis
Dokter dan ilmuwan menentukan berapa banyak obat atau zat kimia yang diperlukan dalam pengobatan. Model predictive analytics dapat digunakan untuk membantu pengambilan keputusan dengan memprediksi dosis optimal berdasarkan data dosis masa lalu dan hasil terkait. Prediksi dosis dengan model predictive analytics tentu harus dibuat dengan sangat hati-hati demi keselamatan pasien.


4. Penilaian Risiko
Risiko merupakan salah satu hal yang sangat berpengaruh dalam setiap keputusan organisasi. Model predictive analytics dapat digunakan untuk memprediksi risiko yang terkait dengan keputusan, seperti mengeluarkan pinjaman atau menanggung polis asuransi. Model ini dilatih menggunakan data historis yang berkaitan dengan indikator utama risiko. Keluaran dari model prediksi risiko dapat digunakan oleh organisasi untuk membuat penilaian risiko yang lebih baik di masa mendatang.

Bagaimana, Anda tertarik untuk membuat model predictive analytics? Di modul kali ini Anda akan mempelajari kasus predictive analytics pada bidang marketing. Hingga akhir modul ini diharapkan Anda dapat:

* Memahami problem statement pada kasus prediksi harga diamonds (berlian).
* Melakukan proses exploratory data analysis.
* Melakukan tahap data preparation. 
* Membuat model machine learning dengan pendekatan K-Nearest Neighbor.
* Membuat model machine learning dengan pendekatan Random Forest.
* Membuat model machine learning dengan pendekatan Boosting Algorithm.
*Mengevaluasi Model.

# Predictive Analytics Lifecycle
Seperti proyek machine learning lainnya, proyek predictive analytics memiliki beberapa tahapan dalam proses pengembangannya. Keberhasilan proyek predictive analytics tidak hanya ditentukan oleh pemilihan algoritma machine learning saja, melainkan juga penerapan metodologi standar dalam mengelola seluruh tahapan atau siklus proyek. Cross-Industry Standard Process for Data Mining atau disingkat menjadi CRISP-DM merupakan salah satu metode standar proses analitik yang paling umum digunakan. Metode ini akan membantu Anda mengelola proyek dari tahapan mendefinisikan masalah hingga mendapatkan insight.

<p align="center">
  <a href='https://www.dicoding.com/academies/319/tutorials/16989#'><img src="https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:07e8c97a32a3c019f20b0fe92c806e8920210910103523.png"></a>
</p>


Dalam metode ini, proses analitik dibagi menjadi enam fase utama, antara lain:

Business understanding
Proyek predictive analytics biasanya berfokus pada hal-hal seperti mendapatkan pelanggan baru, meningkatkan performa penjualan, dan menambahkan efisiensi pada suatu proses tertentu. Fase awal dari proyek analitik bertujuan untuk memahami masalah bisnis kemudian merancang solusi analitik berdasarkan data untuk menyelesaikan permasalahan tersebut. Tahapan ini mencakup proses klarifikasi masalah, menentukan tujuan atau objective, dan mengidentikasi sumber daya yang dimiliki.
 

Data understanding
Memiliki pemahaman mengenai data yang tersedia berikut sumbernya merupakan fase yang penting setelah tujuan proyek diputuskan. Fase ini memungkinkan Anda untuk memahami informasi dalam data dan menentukan kualitasnya. Pemahaman data sangat penting untuk menghindari masalah yang tidak terduga selama fase berikutnya, yaitu fase persiapan data (data preparation).


Data preparation
Data preparation merupakan salah satu tahapan penting yang paling memakan waktu. Proses yang Anda lakukan dalam tahapan ini bisa berbeda tergantung kebutuhan dan tujuannya. Namun, secara umum, hal-hal yang akan Anda lakukan dalam fase ini adalah sebagai berikut:

* Menggabungkan data.

* Menyeleksi data yang akan digunakan.

* Melakukan proses transformasi data

* Membagi data menjadi data training dan test.


Modeling
Pemodelan biasanya dilakukan dalam beberapa iterasi. Pada fase ini, Anda menggunakan algoritma machine learning yang berbeda untuk membuat model prediksi. Model-model ini kemudian dibandingkan dan model terbaiklah yang akan dipilih untuk diterapkan.
 

Evaluation
Sebelum model diterapkan, model perlu dievaluasi agar terbukti cocok untuk tujuan yang telah ditentukan. Fase ini bertujuan untuk memastikan bahwa model akan mampu membuat prediksi yang akurat dan tidak mengalami overfitting atau underfitting.


Deployment
Pada fase ini, model machine learning yang telah Anda buat akan diintegrasikan ke dalam sistem organisasi. Secara umum, proses yang Anda lakukan dalam fase ini adalah:

* Mengintegrasikan model ke dalam sistem (proses deployment).

* Memonitor hasil deployment.

* Membuat laporan akhir dan melakukan evaluasi proyek.

Setiap tahapan dalam metode ini penting untuk keberhasilan proyek. Urutan tahapan dalam metode ini menunjukkan hubungan yang paling sering antar fase. Ia membantu Anda dalam melihat skema garis besarnya serta memahami bagaimana setiap tahapan memberikan kontribusi pada tahapan berikutnya. Namun, tahapan-tahapan ini tidak harus diikuti secara berurutan. Seperti halnya sebuah siklus, Anda dapat mengulang setiap tahapan jika diperlukan. Biasanya ini terjadi jika Anda menemukan informasi yang bertentangan dengan apa yang telah Anda temukan sebelumnya.

Sebagai contoh, saat membuat proyek machine learning untuk kasus predictive analytics, Anda merasa telah selesai dengan tahap persiapan data. Namun, saat melakukan proses pemodelan Anda menemukan fakta bahwa data Anda tidak dapat mengakomodasi kondisi tertentu. Oleh karena itu, Anda perlu kembali ke tahapan sebelumnya dan melakukan proses persiapan data kembali. 

# Business Understanding
Bayangkan Anda adalah pemilik perusahaan yang bergerak di bidang jual-beli diamonds (berlian). Model bisnis Anda adalah distributor dan retail, perusahaan membeli diamonds dari produsen kemudian menjualnya kepada konsumen. Perusahaan juga menerima penjualan kembali diamonds dari konsumen. Untuk efisiensi, Anda ingin menerapkan automasi pada sistem dalam memprediksi harga diamonds dengan teknik predictive modelling.

<p align="center">
  <a href='https://www.dicoding.com/academies/319/tutorials/16989#'><img src="https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:d0168045ce52afc1d01e30f70f7806f920210910103802.png"></a>
</p>

Contoh kasus, Anda mengetahui bahwa harga sebuah diamonds dengan karakteristik tertentu bernilai $9000 di pasaran.  Jika ingin mendapatkan profit, tentu perusahaan harus mendapatkan harga beli diamond yang lebih rendah dari $9000. Sebut saja misal, harga belinya adalah $5000. Sudah pasti ini akan menjadi keuntungan besar bagi perusahaan. Sebaliknya, jika perusahaan membeli diamonds tersebut dengan harga di atas $9000, maka perusahaan akan rugi.

Tentu saja semua bisnis mengejar profit. Oleh karena itu, penting bagi perusahaan untuk mengetahui dan dapat memprediksi harga diamonds di pasar. Prediksi akan digunakan untuk menentukan berapa harga beli yang pantas untuk diamonds dengan karakteristik tertentu sehingga perusahaan bisa mendapatkan profit sebesar mungkin.

Tidak seperti emas yang harga jual dan belinya mengacu pada harga perdagangan emas dunia, harga diamonds dipengaruhi oleh beberapa fitur khusus. Fitur tersebut antara lain, karat, ukuran, bentuk potongan, warna, serta tingkat kejernihan diamonds. Tidak adanya acuan harga diamonds seperti acuan harga emas menyebabkan perusahaan memerlukan sistem untuk memprediksi harganya.



Problem Statements dan Goals
Berdasarkan kondisi yang telah diuraikan sebelumnya, perusahaan akan mengembangkan sebuah sistem prediksi harga diamonds untuk menjawab permasalahan berikut.

Dari serangkaian fitur yang ada, fitur apa yang paling berpengaruh terhadap harga diamonds?
Berapa harga pasar diamonds dengan karakteristik atau fitur tertentu?  
Untuk  menjawab pertanyaan tersebut, Anda akan membuat predictive modelling dengan tujuan atau goals sebagai berikut:

Mengetahui fitur yang paling berkorelasi dengan harga diamonds.
Membuat model machine learning yang dapat memprediksi harga diamonds seakurat mungkin berdasarkan fitur-fitur yang ada.


Metodologi
Prediksi harga adalah tujuan yang ingin dicapai. Seperti yang kita tahu, harga merupakan variabel kontinu. Dalam predictive analytics, saat membuat prediksi variabel kontinu artinya Anda sedang menyelesaikan permasalahan regresi. Oleh karena itu, metodologi pada proyek ini adalah: membangun model regresi dengan harga diamonds sebagai target.



Metrik
Metrik digunakan untuk mengevaluasi seberapa baik model Anda dalam memprediksi harga. Untuk kasus regresi, beberapa metrik yang biasanya digunakan adalah Mean Squared Error (MSE) atau Root Mean Square Error (RMSE). Secara umum, metrik ini mengukur seberapa jauh hasil prediksi dengan nilai yang sebenarnya. Kita akan bahas lebih detail mengenai metrik ini di modul Evaluasi.

Pengembangan model akan menggunakan beberapa algoritma machine learning yaitu K-Nearest Neighbor, Random Forest, dan Boosting Algorithm. Dari ketiga model ini, akan dipilih satu model yang memiliki nilai kesalahan prediksi terkecil. Dengan kata lain, kita akan membuat model seakurat mungkin, yaitu model dengan nilai kesalahan sekecil mungkin.

Membuat model prediktif dengan machine learning tentu memerlukan data. Berita baiknya adalah, perusahaan memiliki data yang dibutuhkan untuk membuat model prediksi. Dataset yang akan kita gunakan pada praktik kali ini adalah Diamond dataset. Ia merupakan real-world dataset yang menjadi data bawaan (built in) dari ggplot2 packages. Anda dapat mengunduhnya melalui repository GitHub ggplot.

Pada modul berikutnya, Anda akan mengeksplorasi dataset ini lebih detail. Sudah siap untuk lanjut? 

# Data Understanding
<p align="center">
  <a href='https://www.dicoding.com/academies/319/tutorials/16989#'><img src="https://dicoding-web-img.sgp1.cdn.digitaloceanspaces.com/original/academy/dos:e8a8e2fed3b414d0503d2fad091b303120210910103958.png"></a>
</p>

Data yang Anda gunakan pada proyek kali ini adalah Diamond dataset yang diunduh dari repository GitHub ggplot. Untuk tahap latihan, Anda hanya akan menggunakan dataset ini sehingga tidak perlu menambahkan data lain atau melakukan penggabungan dataset lagi. Selain itu, dataset ini juga cukup bersih sehingga tidak terlalu banyak memerlukan proses data cleaning.

Dataset ini memiliki 53.940 jenis diamonds dengan berbagai karakteristik dan harga. Karakteristik yang dimaksud di sini adalah fitur non-numerik seperti cut, color, dan clarity, serta fitur numerik seperti carat, x, y, z, table, dan depth. Kesembilan fitur ini adalah fitur yang akan Anda gunakan dalam menemukan pola pada data, sedangkan harga merupakan fitur target.

Dalam membuat model prediktif dengan machine learning, Anda dapat menggunakan tools manapun yang biasa Anda gunakan, misalnya Google Colaboratory, Jupyter Notebook, Python Anaconda. Jika ingin menggunakan Python IDE (integrated Development Tools) Anda bisa menggunakan tools seperti Pycharm atau Visual Studio. Selain itu, Anda juga dapat menggunakan notebook dari penyedia layanan cloud seperti IBM Watson Studio.

Untuk kemudahan dalam menguraikan setiap tahapan kode, proyek ini menggunakan tools Google Colaboratory. Bagaimana dengan Anda? Sudah menentukan tools apakah yang ingin digunakan? 

Jika sudah, mari langsung coba memahami data kita dalam beberapa tahapan berikut:

Data loading
Exploratory Data Analysis - Deskripsi Variabel
Exploratory Data Analysis - Menangani Missing Value dan Outliers
Exploratory Data Analysis - Univariate Analysis
Exploratory Data Analysis - Multivariate Analysis

# Rangkuman : Predictive Analytics

Predictive analytics adalah bidang terapan yang menggunakan berbagai metode kuantitatif untuk membuat prediksi dengan memanfaatkan data. Ia merupakan seni membangun serta menggunakan model prediksi berdasarkan pola data historis. Data diubah dan diekstrak menjadi informasi berharaga untuk menghasilkan keputusan analytics. Saat ini, keputusan analytics merupakan senjata strategis di bidang bisnis.

Keberhasilan proyek predictive analytics tidak hanya ditentukan oleh pemilihan algoritma machine learning saja, melainkan juga penerapan metodologi standar dalam mengelola seluruh tahapan atau siklus proyek. Cross-Industry Standard Process for Data Mining atau disingkat menjadi CRISP-DM merupakan salah satu metode standar proses analitik yang paling umum digunakan. 

Berikut merupakan fase-fase utama proses analitik dalam metode CRISP-DM:

Business understanding.
Fase atau tahapan ini mencakup proses klarifikasi masalah, menentukan tujuan atau objective, dan mengidentikasi sumber daya yang dimiliki.
Data understanding.
Ini merupakan tahapan untuk memahami informasi dalam data dan menentukan kualitasnya.

Data preparation.  
Pada tahapan ini, Anda melakukan proses transformasi pada data sehingga menjadi bentuk yang cocok untuk proses pemodelan..

Modeling.
Ini merupakan tahapan saat Anda menggunakan algoritma machine learning untuk membuat model prediksi.

Evaluation.
Tahapan ini bertujuan untuk memastikan bahwa model akan mampu membuat prediksi yang akurat dan tidak mengalami overfitting atau underfitting.

Deployment.
Pada tahap ini, model machine learning yang telah Anda buat akan diintegrasikan ke dalam sistem organisasi.  

Pada modul ini, Anda telah belajar menerapkan metode CRISP-DM dengan studi kasus prediksi harga diamonds. Pada studi kasus ini, Anda menggunakan tiga jenis algoritma, yaitu:

K-Nearest Neighbor.
KNN bekerja dengan membandingkan jarak satu sampel ke sampel pelatihan lain dengan memilih sejumlah k-tetangga terdekat. Algoritma KNN menggunakan ‘kesamaan fitur’ untuk memprediksi nilai dari setiap data yang baru. Dengan kata lain, setiap data baru diberi nilai berdasarkan seberapa mirip titik tersebut dalam set pelatihan.

Random Forest.
Algoritma random forest adalah salah satu algoritma supervised learning yang dapat digunakan untuk menyelesaikan masalah klasifikasi dan regresi. Ia termasuk ke dalam kelompok model ensemble (group). Algoritma ini disusun dari banyak algoritma pohon (decision tree) yang pembagian data dan fiturnya dipilih secara acak.

Boosting Algorithm.
Algoritma boosting bekerja dengan membangun model dari data latih. Kemudian ia membuat model kedua yang bertugas memperbaiki kesalahan dari model pertama. Model ditambahkan sampai data latih terprediksi dengan baik atau telah mencapai jumlah maksimum model untuk ditambahkan.

Dengan uraian tersebut, diharapkan Anda dapat memahami apa itu model predictive analytics dan langkah-langkah dalam membuat modelnya. Jika ada materi yang masih belum dipahami, Anda bisa mengulas kembali materi yang diberikan di modul ini atau menanyakan di forum diskusi. 



Daftar Referensi
Jika tertarik untuk mengeksplorasi lebih lanjut mengenai materi Predictive Analytics Anda dapat mempelajarinya melalui daftar referensi berikut:

[19] Kelleher, John D, et al. "Machine Learning for Predictive Data Analytics". MIT Press. 2020. Tersedia: tautan informasi buku.

[20] Delen, Dursun. “Predictive Analytic: Data Mining, Machine Learning and Data Science for Practitioners”. Pearson FT. Press. 2020. Tersedia: O'Reilly media. 

[21] IBM Cloud. "Exploratory Data Analysis". Tersedia: tautan. Diakses pada 2 Juni 2021.

[22] Kang, Hyun. "The Prevention and Handling the Missing Data". Tersedia: tautan. Diakses pada Juni 2021.

[23] Kuhn, Max dan Johnson Kjell. "Applied Predictive Modeling". Springer. 2013.

[24] Seltman, Howard J. “Experimental Design and Analysis”. 2018. Tersedia: tautan. DIakses pada Juni 2021.

[25] Fuentes, Alvaro. "Hands-on Predictive Analytics with Python". Packt Publishing. 2018. Tersedia: O'Reilly Media.

[26] Rhys, Hefin. "Machine Learning with R, the Tidyverse, and MLR". Manning Publications. 2020. Tersedia: O'Reilly Media.

[27] Scikit-learn Documentation. Tersedia: tautan. Diakses pada: Juni 2021.

[28] Parker, Mary. "Sampling with Replacement and Sampling without Replacement". Tersedia: tautan. Diakses pada Juni 2021. 
