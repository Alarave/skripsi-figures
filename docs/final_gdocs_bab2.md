# 2. TINJAUAN PUSTAKA

## 2.1 Penelitian Terdahulu

Telaah literatur terhadap penelitian terdahulu menunjukkan pergeseran paradigma yang jelas dalam pemrosesan data katalog produk perdagangan digital. Pendekatan awal yang berfokus pada ekstraksi atribut berbasis representasi teks murni telah berkembang menuju integrasi penambatan visual multimodal guna menangkap keterkaitan spasial antara deskripsi produk dan citra kemasan. Perkembangan lanjutan menunjukkan keberhasilan modul deteksi objek dan sistem OCR terdedikasi dalam mengekstraksi teks pada permukaan kemasan ritel fisik secara deterministik. Pada tahap kontemporer, kemunculan model fondasi multimodal beresolusi dinamis dan agen cerdas berbasis penalaran bertahap memperluas kapabilitas audit visual dalam memverifikasi kepatuhan atribut produk berskala besar. Pemetaan sistematis terhadap delapan penelitian terdahulu yang relevan dirangkum pada Tabel 2.1.

**Tabel 2.1 Penelitian Terdahulu**

| No | Peneliti dan Tahun | Objek Penelitian | Metode | Hasil Penelitian | Perbedaan |
|:---:|:---|:---|:---|:---|:---|
| 1 | Huma dkk. (2026) | Kemasan pangan olahan | YOLOv8 dan PaddleOCR | Akurasi ekstraksi 84,20% | Menguji kemasan kosmetik permukaan lengkung tiga atribut dan membandingkannya dengan MLLM. |
| 2 | Liu dkk. (2026) | Citra perdagangan digital permukaan lengkung | DBNet++ dan SVTR | F-measure 88,70% pada permukaan lengkung | Mengintegrasikan detektor objek spasial dan sistem verifikasi aturan katalog terpadu. |
| 3 | Kumar dkk. (2026) | Katalog produk ritel perdagangan digital | Agentic MLLM ReAct | Akurasi audit 98,20% dan penambahan kelengkapan atribut 90,40% | Menguji komparasi langsung terhadap alur konvensional melalui uji statistik inferensial formal. |
| 4 | Richo (2025) | Kemasan ritel | YOLOv11m dan PaddleOCR | mAP@50 98,44% dan akurasi verifikasi 97,42% | Memverifikasi multi-atribut katalog dengan partisi data bebas bocor antar-merek. |
| 5 | Shukla dan Sonalkar (2025) | Atribut terperinci perdagangan digital | MLLM Zero-Shot | Akurasi makro 86,10% turun ke 61,80% pada teks mikro | Membandingkan modul inspeksi lokal dinamis terhadap detektor spasial fisik terpisah. |
| 6 | Wang dkk. (2024) | Dokumen visual umum | Qwen2-VL Dynamic Resolution | Akurasi DocVQA 95,70% | Menguji adaptasi model penalaran pada citra fisik kemasan kosmetik ritel berlatar studio. |
| 7 | Wu dkk. (2023) | Pasangan produk ritel berjumlah 2,3 juta | Catalog Phrase Grounding | mAP 68,50% melokalisasi frasa atribut | Menuntaskan pembacaan teks karakter mikro dan kepatuhan nomor izin edar BPOM. |
| 8 | Yang dkk. (2022) | Produk MAVE berjumlah 2,2 juta | Multimodal Sequence Tagging | F1-Score ekstraksi atribut 82,40% | Mencakup verifikasi silang fisik kemasan permukaan lengkung berlatar studio terstandardisasi. |

Sintesis terhadap Tabel 2.1 memperlihatkan evolusi metodologis yang berkesinambungan dari model sekuensial berbasis teks menuju pemodelan spasial multimodal dan penalaran agen cerdas otonom. Pada tahap awal rekayasa visi komputer, kolaborasi antara detektor spasial dan modul OCR terbukti efektif mengekstraksi teks spesifikasi pada kemasan produk ritel maupun pangan olahan (Huma, Fanggidae, Rumlaklak, dan Triwahyuadi, 2026). Meskipun demikian, efektivitas metode deteksi spasial konvensional tersebut umumnya diuji pada kemasan datar dengan orientasi horizontal yang seragam. Ketika dihadapkan pada produk kosmetik, kelengkungan bidang wadah botol dan toples menimbulkan distorsi optis non-linear yang menuntut pemodelan geometri khusus. Menjawab kendala deformasi tersebut, Liu dkk. (2026) membuktikan bahwa adaptasi arsitektur DBNet++ dan rekognisi sekuensial SVTR mampu mempertahankan ketahanan pembacaan karakter pada permukaan lengkung hingga mencapai nilai *F-measure* sebesar 88,70%.

Perkembangan berikutnya bergerak melampaui sekadar ekstraksi teks fisik, yakni menghubungkan entitas visual kemasan dengan struktur atribut katalog niaga elektronik. Dalam hal ini, Yang dkk. (2022) menginisiasi penandaan sekuensial multimodal berbasis representasi gabungan teks judul dan citra produk guna mengekstraksi atribut bernilai tinggi pada skala jutaan data. Kerangka penambatan visual ini kemudian disempurnakan oleh Wu dkk. (2023) melalui mekanisme penambatan frasa visual teks yang secara eksplisit memetakan frasa deskripsi katalog ke koordinat wilayah kotak pembatas objek pada kemasan ritel. Integrasi representasi lintas modalitas ini meletakkan fondasi penting bagi verifikasi otomatis, sebab ketidakcocokan antara teks klaim katalog dan wujud visual kemasan dapat diidentifikasi secara langsung melalui relasi semantik antarmodalitas.

Pada perkembangan teknologi terkini, kemunculan model fondasi multimodal dan paradigma agen otonom membuka kapabilitas baru dalam audit katalog produk digital. Kumar dkk. (2026) membuktikan bahwa pemanfaatan agen multimodal berbasis siklus ReAct mampu meningkatkan kelengkapan atribut produk hingga 90,40% dan mencatatkan akurasi audit sebesar 98,20% melalui koordinasi dinamis antar-alat bantu visual. Di sisi lain, Wang dkk. (2024) mendemonstrasikan bahwa arsitektur Qwen2-VL dengan mekanisme resolusi dinamis mencapai akurasi 95,70% pada pemahaman dokumen visual kompleks tanpa terdistorsi oleh rasio aspek masukan. Meskipun demikian, Shukla dan Sonalkar (2025) mengidentifikasi batasan mendasar model fondasi multimodal saat dihadapkan pada karakter teks berukuran mikro pada kemasan fisik produk, yang menyebabkan akurasi pembacaan mengalami penurunan tajam dari 86,10% menjadi 61,80%.

Berdasarkan telaah kritis terhadap penelitian terdahulu, ditemukan celah penelitian yang belum terselesaikan. Sebagian besar penelitian menguji sistem verifikasi pada kemasan datar atau dokumen pindaian ideal, belum mengintegrasikan detektor objek YOLOv11 dan mesin PaddleOCR secara komparatif melawan model penalaran otonom Agentic MLLM Qwen2-VL, serta belum mengevaluasi performa model menggunakan pengujian statistik inferensial formal pada produk kosmetik berkemasan lengkung. Penelitian ini hadir untuk menutup celah tersebut dengan membandingkan kedua paradigma kecerdasan buatan secara empiris pada dataset katalog Sociolla berbasis partisi bebas kebocoran merek.

## 2.2 Kemasan Kosmetik

Katalog kosmetik digital pada platform niaga elektronik seperti Sociolla mengelola ribuan data spesifikasi produk resmi yang memuat informasi teks dan citra kemasan fisik. Secara fisik, produk kosmetik memiliki variasi geometri kemasan yang beragam, meliputi botol silindris, toples bundar, tabung plastik fleksibel, dispenser pompa, hingga wadah padat. Ragam geometri ini menampung berbagai kategori sediaan produk, seperti sediaan cair (toner, serum, micellar water), emulsi atau krim (pelembap, tabir surya), gel, losion, hingga serbuk padat.

Karakteristik visual kemasan kosmetik tampak depan menyajikan tiga atribut utama yang menjadi fokus identifikasi konsumen dan kurasi katalog, yaitu nama merek dagang, volume atau berat isi bersih, dan tipe sediaan produk. Merujuk pada Undang-Undang Perlindungan Konsumen Nomor 8 Tahun 1999 serta Peraturan BPOM Nomor 23 Tahun 2019 tentang Persyaratan Teknis Penandaan Kosmetika, setiap produk yang beredar wajib mencantumkan penandaan yang benar, jelas, dan tidak menyesatkan pada panel utama tampak depan:
1. Nama Kosmetika: Memuat nama produk dan nama merek dagang yang telah terdaftar resmi pada sistem notifikasi BPOM.
2. Isi Bersih atau Netto: Dinyatakan secara tegas dalam satuan metrik volume mililiter atau liter untuk sediaan cair, serta satuan massa gram atau miligram untuk sediaan padat dan semi-padat.
3. Bentuk Sediaan: Penjelasan fungsi atau wujud fisik produk yang membedakan peruntukan penggunaannya.

Posisi ketiga atribut label dan wujud fisik kemasan disajikan pada Gambar 2.1.

![Gambar 2.1 Karakteristik Fisik Kemasan dan Label Atribut](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_1_kemasan_kosmetik.png)

**Gambar 2.1 Karakteristik Fisik Kemasan dan Label Atribut**

Gambar 2.1 memperlihatkan posisi fisik ketiga atribut utama pada kemasan kosmetik tampak depan, dengan nama merek diletakkan pada bagian atas, jenis sediaan produk pada bagian tengah, dan keterangan isi bersih berada pada bagian bawah label. Pada saat yang sama, Gambar 2.1 memperlihatkan tantangan pantulan cahaya studio pada permukaan wadah plastik dan kaca yang menghasilkan area kilap luminansi tinggi sehingga berpotensi menutupi karakter teks label.

Selain pantulan cahaya studio, kelengkungan fisik botol silindris menyebabkan baris teks label tampak melengkung secara optis terhadap sudut tangkapan kamera, serta ukuran huruf mikro pada informasi netto memiliki ketebalan goresan hanya beberapa piksel pada resolusi standar katalog digital. Ketidaksesuaian antara teks klaim katalog dan kondisi fisik kemasan merupakan pelanggaran terhadap hak konsumen dan regulasi BPOM. Oleh karena itu, label kemasan fisik yang tampak pada citra katalog diposisikan sebagai rujukan hukum dan faktual primer atau *ground truth*. Sistem verifikasi otomatis bertugas mencocokkan data entri teks katalog terhadap data visual kemasan fisik guna memastikan kepatuhan penandaan sebelum produk ditayangkan.

## 2.3 Citra Digital

Citra digital didefinisikan sebagai fungsi intensitas cahaya dua dimensi f(x, y), dengan x dan y menyatakan koordinat spasial bidang citra, sedangkan amplitudo nilai f pada sembarang koordinat (x, y) menyatakan intensitas kecerahan atau derajat keabuan citra pada titik tersebut (Gonzalez dan Woods, 2018). Menurut Putra (2010), suatu citra visual diklasifikasikan sebagai citra digital apabila nilai koordinat spasial x, y serta nilai amplitudo intensitas f seluruhnya bernilai diskret dan berhingga. Ditinjau melalui representasi komputasi, citra digital dinyatakan dalam susunan matriks dua dimensi berukuran M × N, dengan M menyatakan jumlah baris dan N menyatakan jumlah kolom, sebagaimana dirumuskan pada Persamaan (2.1):



![Persamaan 2.1](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_1.png)



Setiap elemen diskret pada perpotongan baris dan kolom pada Persamaan (2.1) disebut sebagai elemen gambar atau piksel. Pada citra berwarna standar, representasi visual disusun berdasarkan model warna aditif RGB. Model ini merepresentasikan citra sebagai matriks tiga dimensi berukuran M times N times 3 yang tersusun atas tiga kisi kanal warna primer, yaitu kanal merah, kanal hijau, dan kanal biru. Setiap elemen piksel pada masing-masing kanal warna memiliki kedalaman kuantisasi 8-bit, sehingga menyimpan variasi intensitas warna sebanyak 2^8 atau 256 derajat nilai diskret dengan rentang integer antara 0 hingga 255.

Dalam konteks fotografi produk katalog perdagangan digital Sociolla, citra kemasan kosmetik diambil di lingkungan studio dengan pencahayaan buatan berlatar putih bersih dengan dimensi standar 800 times 800 piksel. Interaksi berkas cahaya studio pada permukaan wadah kosmetik berbahan plastik kilap atau kaca menghasilkan fenomena pantulan spekular. Secara numerik pada matriks piksel, pantulan ini memicu saturasi intensitas maksimal pada ketiga kanal warna secara serentak dengan nilai R = G = B = 255. Saturasi intensitas tersebut menghilangkan detail gradien tekstur dan kontur goresan huruf teks label mikro kemasan fisik, seperti nama produk dan informasi netto. Oleh karena itu, pemahaman karakteristik matematis citra digital menjadi dasar perancangan tahapan praproses penstabilan luminansi dan perbaikan kontras lokal adaptif sebelum ekstraksi fitur dilakukan oleh model pembelajaran mendalam.

Representasi sistem koordinat spasial dan struktur matriks piksel diskret citra kemasan disajikan pada Gambar 2.2.

![Gambar 2.2 Representasi Citra Digital dalam Matriks Piksel](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_2_matriks_citra_digital.png)

**Gambar 2.2 Representasi Citra Digital dalam Matriks Piksel**

Gambar 2.2 memperlihatkan pemetaan citra kemasan kosmetik ke dalam sistem koordinat spasial diskret. Panel (a) menampilkan potongan citra label kemasan asli katalog Sociolla dengan penanda wilayah target pembesaran. Panel (b) memperlihatkan kisi piksel visual pembentuk kontur huruf teks, sedangkan Panel (c) menyajikan representasi matriks nilai intensitas kecerahan diskret f(x, y) berskala 8-bit yang membedakan goresan huruf bernilai intensitas rendah dari permukaan wadah bernilai intensitas tinggi.


## 2.4 Praproses Citra

Praproses citra merupakan tahap awal pengolahan data visual yang bertujuan memperbaiki kualitas data citra mentah, menekan gangguan distorsi yang tidak diinginkan, serta menonjolkan fitur visual penting agar model pembelajaran mesin dapat mengekstrak informasi secara optimal (Sonka, Hlavac, dan Boyle, 1993). Dalam visi komputer, data citra mentah yang diperoleh dari sensor atau kamera umumnya masih memiliki variasi pencahayaan, derau latar belakang, dan perbedaan dimensi yang belum seragam. Sebagaimana ditegaskan oleh Stojnev dan Stojnev Ilić (2020), praproses data citra berfungsi mereduksi derau dan meningkatkan kualitas representasi masukan sehingga menghasilkan presisi lokalisasi dan akurasi prediksi yang lebih tinggi pada model klasifikasi maupun deteksi objek.

Pada kemasan kosmetik, citra katalog digital menghadapi kendala berupa pantulan cahaya spekular pada permukaan wadah kaca atau plastik, teks berukuran mikro pada label isi bersih, serta orientasi kemasan yang bervariasi. Untuk mempersiapkan citra agar siap diproses oleh detektor objek YOLOv11 dan mesin PaddleOCR, diterapkan rangkaian tahapan praproses terstruktur sebagaimana disajikan pada Gambar 2.3.

![Gambar 2.3 Tahapan Pengolahan Citra Digital](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_1_tahapan_pengolahan_citra.png)

**Gambar 2.3 Tahapan Pengolahan Citra Digital**

Bagan alir pada Gambar 2.3 memperlihatkan alur praproses citra kemasan kosmetik yang mencakup enam tahapan berurutan, dimulai dari penerimaan citra mentah, reduksi derau dengan penapisan bilateral, pemisahan pantulan kilap pada ruang warna HLS, penajaman adaptif tepi karakter teks, perbaikan kontras lokal adaptif CLAHE, hingga standardisasi kanvas *letterbox padding* berukuran 640 × 640 piksel.

Peningkatan kontras teks kemasan tidak dapat dilakukan secara langsung pada kanal warna RGB asli karena ketiga kanal tersebut memiliki korelasi intensitas yang saling terikat. Manipulasi langsung pada kanal RGB berpotensi mengubah warna asli produk dan merusak identitas merek dagang. Oleh karena itu, citra terlebih dahulu ditransformasikan ke dalam ruang warna perseptual CIE L*a*b* guna memisahkan komponen intensitas luminansi L* secara ortogonal dari dua komponen krominans a* dan b*. Merujuk pada standar kolorimetri CIE, konversi nilai koordinat (L*, a*, b*) dari ruang tristimulus (X, Y, Z) terhadap titik referensi putih standar (X_n, Y_n, Z_n) dirumuskan pada Persamaan (2.2) dan Persamaan (2.3):



![Persamaan 2.2](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_2.png)



dengan fungsi pemetaan non-linear f(t) yang dirumuskan sebagai berikut:



![Persamaan 2.3](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_3.png)



Setelah komponen luminansi L* terisolasi, perbaikan kontras lokal diterapkan menggunakan metode *Contrast Limited Adaptive Histogram Equalization* atau CLAHE (Zuiderveld, 1994). CLAHE bekerja dengan membagi kanvas citra menjadi kisi-kisi ubin lokal kontekstual berukuran M_{tile} times N_{tile} seperti kisi 8 × 8 ubin, lalu melakukan perataan histogram secara mandiri pada setiap blok. Untuk mencegah penguatan derau visual pada area latar belakang kemasan yang polos, distribusi histogram lokal dipangkas berdasarkan ambang batas klip β sesuai formulasi Persamaan (2.4):



![Persamaan 2.4](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_4.png)



Piksel yang melampaui batas ambang β didistribusikan kembali secara merata ke seluruh kelas intensitas, dan artefak garis batas antar-ubin dieliminasi menggunakan interpolasi bilinear.

Tahap akhir praproses adalah penyeragaman dimensi citra menuju ukuran target W_t × H_t sebesar 640 × 640 piksel dan normalisasi rentang nilai piksel ke dalam skala 0 hingga 1. Penyeragaman dimensi pada deteksi kemasan tidak boleh menggunakan pengubahan ukuran langsung secara *direct resize* yang meregangkan gambar, karena perubahan rasio aspek akan mendistorsi bentuk fisik botol dan geometri teks label. Oleh sebab itu, diterapkan teknik *letterbox padding* yang mempertahankan rasio aspek asli dengan menyisipkan batas abu-abu netral pada sisi yang lebih pendek. Faktor skala proporsional s serta offset pergeseran pusat (d_x, d_y) dari dimensi citra awal (w₀, h₀) dihitung melalui Persamaan (2.5):



![Persamaan 2.5](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_5.png)



Penyusutan resolusi dilakukan dengan interpolasi area piksel untuk mempertahankan ketajaman garis huruf kecil pada label netto. Parameter affine [s, d_x, d_y] disimpan untuk memetakan kembali koordinat *bounding box* hasil deteksi pada kanvas letterbox (x′, y′) ke koordinat piksel citra kemasan asli (x_orig, y_orig) melalui Persamaan (2.6):



![Persamaan 2.6](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_6.png)



## 2.5 Deep Learning

*Deep learning* merupakan sub-bidang dari *machine learning* dan bagian dari ranah *artificial intelligence* yang memanfaatkan arsitektur jaringan saraf tiruan berlapis banyak untuk mempelajari representasi data secara hierarkis (LeCun dkk., 2015). Istilah *deep* merujuk pada keberadaan lapisan tersembunyi yang berjumlah banyak di antara lapisan masukan dan lapisan keluaran jaringan saraf (Goodfellow dkk., 2016). Struktur multi-lapis ini mentransformasikan data masukan mentah secara bertingkat melalui serangkaian fungsi non-linear menuju representasi abstraksi tingkat tinggi (Deng dan Yu, 2014). Posisi hierarkis *deep learning* dalam ranah kecerdasan buatan disajikan pada Gambar 2.4.

![Gambar 2.4 Hubungan Artificial Intelligence, Machine Learning, dan Deep Learning](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_4_hubungan_ai_ml_dl.png)

**Gambar 2.4 Hubungan Artificial Intelligence, Machine Learning, dan Deep Learning**

Gambar 2.4 mengilustrasikan relasi himpunan bersarang yang menegaskan bahwa *deep learning* merupakan spesialisasi dari *machine learning*, dengan keduanya bernaung di bawah payung disiplin *artificial intelligence*. Jaringan saraf tiruan pada *deep learning* tersusun atas simpul komputasi yang saling terhubung melintasi lapisan masukan, deretan lapisan tersembunyi, hingga lapisan keluaran akhir. Struktur berlapis ini memungkinkan jaringan memproses variasi data citra berdimensi tinggi secara adaptif.

Meskipun *deep learning* berada dalam naungan *machine learning*, kedua paradigma tersebut memiliki perbedaan mendasar pada metode ekstraksi fitur visual (Chollet, 2021). Perbandingan alur kerja rekayasa fitur antara pembelajaran mesin tradisional dan pembelajaran mendalam disajikan pada Gambar 2.5.

![Gambar 2.5 Perbandingan Alur Rekayasa Fitur Tradisional dan Deep Learning](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_5_perbandingan_ml_dl.png)

**Gambar 2.5 Perbandingan Alur Rekayasa Fitur Tradisional dan Deep Learning**

Bagan alir pada Gambar 2.5 memperlihatkan perbedaan alur komputasi kedua paradigma pada klasifikasi objek kemasan kosmetik. Pada pembelajaran mesin tradisional, alur kerja terpecah menjadi dua tahap terpisah yang menuntut campur tangan perancang manusia untuk mengekstraksi fitur visual manual (*feature extraction*) sebelum diumpankan ke algoritma pengklasifikasi (*classification*) guna menentukan kategori luaran produk. Keterbatasan utama pendekatan ini terletak pada ketergantungannya terhadap keahlian pakar serta kerentanan performa saat menghadapi variasi pencahayaan dan distorsi geometri kemasan. Sebaliknya, paradigma *deep learning* mengintegrasikan ekstraksi representasi fitur visual dan proses klasifikasi (*feature extraction + classification*) ke dalam satu arsitektur jaringan saraf mendalam secara terpadu (*end-to-end*) langsung dari data piksel masukan kemasan menuju prediksi kategori luaran *skincare*.

Prinsip kerja *deep learning* bertumpu pada kemampuan pembentukan hierarki representasi bertingkat secara mandiri (Alzubaidi dkk., 2021). Lapisan awal jaringan mempelajari fitur primitif lokal berfrekuensi spasial tinggi seperti orientasi garis tepi, titik sudut kontur, dan gradien intensitas luminansi. Lapisan perantara menggabungkan fitur primitif tersebut menjadi susunan tekstur permukaan wadah, pola kurvatur botol, dan kontur bentuk kemasan kosmetik. Pada lapisan terdalam, jaringan menyusun abstraksi semantik global yang komprehensif guna mengenali entitas objek utuh serta membedakan karakter teks label secara invarian terhadap variasi skala, rotasi, maupun distorsi perspektif.

Proses optimasi model *deep learning* dilakukan dengan meminimalkan fungsi kerugian melalui algoritma propagasi balik berbasis aturan rantai kalkulus diferensial parsial (Goodfellow dkk., 2016). Galat prediksi dihitung pada keluaran akhir jaringan terhadap target acuan, kemudian gradien kesalahan dipropagasikan mundur melintasi setiap lapisan guna memperbarui matriks bobot sinapsis menggunakan algoritma optimasi berbasis gradien adaptif seperti AdamW (Loshchilov dan Hutter, 2019). Pembelajaran representasi otomatis ini mengeliminasi bias subjektif perancangan fitur manual dan menjadi fondasi utama bagi model visi komputer seperti YOLOv11 dan PaddleOCR dalam menganalisis citra kemasan kosmetik katalog yang kompleks akibat pantulan cahaya studio dan variasi tipografi.

## 2.6 Jaringan Konvolusi

*Convolutional Neural Network* atau CNN merupakan arsitektur jaringan saraf tiruan yang memproses data berformat kisi dua dimensi seperti citra digital (Goodfellow dkk., 2016). Berbeda dengan jaringan saraf tiruan konvensional yang menghubungkan setiap simpul secara penuh, CNN menerapkan pembagian parameter dan koneksi lokal. Kedua prinsip tersebut mengurangi jumlah bobot yang harus dipelajari model serta menjaga ketahanan pengenalan objek dari pergeseran posisi pada citra kemasan.

Struktur arsitektur CNN terbagi menjadi dua bagian utama, yaitu tahap ekstraksi fitur dan tahap klasifikasi (LeCun dkk., 2015). Diagram arsitektur umum CNN disajikan pada Gambar 2.6.

![Gambar 2.6 Arsitektur Jaringan Saraf Tiruan Konvolusi](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_6_arsitektur_cnn.png)

**Gambar 2.6 Arsitektur Jaringan Saraf Tiruan Konvolusi (LeCun dkk., 2015)**

Gambar 2.6 memperlihatkan alur pemrosesan citra masukan berukuran W times H times C hingga menghasilkan nilai prediksi kelas objek. Tahap ekstraksi fitur mengambil informasi visual melalui lapisan konvolusi, fungsi aktivasi, dan lapisan *pooling*. Peta fitur yang dihasilkan kemudian diubah menjadi vektor satu dimensi pada tahap klasifikasi sebelum diproses oleh lapisan terhubung penuh dan dinormalisasi oleh fungsi *softmax*.

Operasi konvolusi dua dimensi bekerja dengan mengalikan matriks citra masukan dengan kernel penapis secara bergeser. Secara matematis, operasi konvolusi diskret antara matriks citra I dan kernel penapis K berukuran (2m+1) times (2n+1) dirumuskan pada Persamaan (2.7):



![Persamaan 2.7](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_7.png)



Simbol (i, j) menyatakan koordinat piksel pada peta fitur keluaran. Ukuran lebar dan tinggi keluaran peta fitur O dipengaruhi oleh ukuran masukan W, ukuran kernel K, penambahan batas *padding* P, serta jarak pergeseran *stride* S, sebagaimana dinyatakan pada Persamaan (2.8):



![Persamaan 2.8](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_8.png)



Keluaran dari operasi konvolusi diproses oleh fungsi aktivasi non-linear agar model mampu mengenali pola visual yang bervariasi (Nair dan Hinton, 2010). Fungsi *Rectified Linear Unit* atau ReLU merupakan fungsi aktivasi dasar yang mengubah seluruh nilai masukan negatif menjadi nol sesuai Persamaan (2.9):



![Persamaan 2.9](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_9.png)



Pada arsitektur YOLOv11, fungsi aktivasi menggunakan varian *Sigmoid-Weighted Linear Unit* atau SiLU agar turunan gradien tetap berjalan lancar dan mencegah simpul saraf berhenti memperbarui bobot (Elfwing dkk., 2018), sebagaimana dirumuskan pada Persamaan (2.10):



![Persamaan 2.10](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_10.png)



Lapisan *pooling* berfungsi memperkecil ukuran spasial peta fitur dan meringankan beban komputasi model (Goodfellow dkk., 2016). Operasi *Max Pooling* mengambil nilai angka terbesar pada area jendela lokal Omega dengan jarak pergeseran s, sebagaimana dinyatakan pada Persamaan (2.11):



![Persamaan 2.11](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_11.png)



Setelah melalui lapisan konvolusi dan *pooling*, peta fitur diubah menjadi vektor satu dimensi x. Vektor tersebut kemudian dihubungkan ke lapisan terhubung penuh melalui perkalian matriks bobot W dan penambahan bias b (Goodfellow dkk., 2016) sesuai Persamaan (2.12):



![Persamaan 2.12](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_12.png)



Pada bagian akhir, nilai luaran z diubah menjadi nilai probabilitas untuk setiap kategori kelas menggunakan fungsi *Softmax*, sebagaimana dirumuskan pada Persamaan (2.13):



![Persamaan 2.13](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_13.png)



Simbol C menyatakan jumlah total kelas objek. Prinsip kerja CNN ini digunakan sebagai pengekstraksi fitur visual pada model deteksi objek YOLOv11 dan model pengenal teks PaddleOCR.

## 2.7 Deteksi Objek

Deteksi objek merupakan cabang visi komputer yang menggabungkan dua tugas komputasi secara simultan: lokalisasi wilayah objek dan klasifikasi kategori objek. Berbeda dengan klasifikasi citra sederhana yang hanya memprediksi satu label global untuk satu citra utuh, deteksi objek mampu menentukan letak koordinat spasial beberapa objek sekaligus melalui representasi *bounding box*.

Secara representasional, sebuah kotak pembatas didefinisikan oleh empat parameter kontinu: (x_c, y_c, w, h), dengan (x_c, y_c) menyatakan koordinat pusat kotak, sedangkan w dan h menyatakan lebar dan tinggi kotak pembatas. Setiap kotak pembatas disertai dengan *confidence score* serta vektor probabilitas distribusi kelas objek.

Tingkat ketepatan lokalisasi kotak pembatas prediksi B_1 terhadap kotak pembatas acuan *ground truth* B_2 diukur menggunakan metrik *Intersection over Union* atau IoU. IoU menghitung rasio luas irisan persekutuan terhadap luas gabungan dari kedua kotak pembatas, sebagaimana dirumuskan pada Persamaan (2.14):



![Persamaan 2.14](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_14.png)



Nilai IoU bernilai antara 0 untuk kondisi tanpa tumpang tindih hingga 1 untuk tumpang tindih sempurna. Ambang batas IoU seperti IoU ge 0{,}50 digunakan sebagai kriteria verifikasi penentuan keberhasilan lokalisasi label kemasan.

## 2.8 Algoritma YOLO

*You Only Look Once* atau YOLO merupakan algoritma deteksi objek berbasis jaringan saraf tiruan yang dikembangkan oleh Joseph Redmon pada tahun 2016 (Redmon dkk., 2016). Berbeda dengan pendeteksi dua tahap seperti R-CNN yang memisahkan pembentukan usulan wilayah dan klasifikasi objek ke dalam tahapan terpisah, YOLO memperlakukan deteksi objek sebagai masalah regresi tunggal langsung dari data piksel citra menuju koordinat kotak pembatas dan probabilitas kelas objek (Satria, 2025). Pendekatan ini memungkinkan model memeriksa seluruh konteks citra dalam satu kali proses inferensi sehingga menghasilkan kecepatan pemrosesan yang tinggi (Fernando, 2024).

Prinsip kerja deteksi YOLO bertumpu pada pembagian citra masukan menjadi kisi-kisi spasial berukuran S times S (Redmon dkk., 2016). Jika titik pusat suatu objek berada di dalam suatu sel kisi, maka sel tersebut bertugas mendeteksi keberadaan objek terkait. Alur kerja mekanisme deteksi sistem YOLO disajikan pada Gambar 2.7.

![Gambar 2.7 Ilustrasi Mekanisme Deteksi Sistem YOLO](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_7_cara_kerja_yolo.png)

**Gambar 2.7 Ilustrasi Mekanisme Deteksi Sistem YOLO (Redmon dkk., 2016)**

Gambar 2.7 memperlihatkan proses prediksi dengan setiap sel kisi memperkirakan sejumlah B kotak pembatas beserta nilai skor keyakinan untuk setiap kotak. Skor keyakinan menunjukkan tingkat kepastian model bahwa kotak memuat objek dan mengukur ketepatan ukuran kotak prediksi terhadap kotak acuan, sebagaimana dirumuskan pada Persamaan (2.15):



![Persamaan 2.15](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_15.png)



Nilai skor keyakinan menjadi nol jika tidak terdapat objek di dalam sel kisi. Sebaliknya, skor keyakinan bernilai sama dengan nilai tumpang tindih antara kotak prediksi dan kotak acuan jika terdapat objek di dalam sel. Selain memprediksi kotak pembatas, setiap sel memperkirakan probabilitas kelas bersyarat Pr(Class_i mid Object). Pada tahap akhir, sistem mengalikan skor keyakinan dengan probabilitas kelas untuk memperoleh skor kelas spesifik, kemudian menyaring kotak pembatas yang bertumpukan menggunakan metode *Non-Maximum Suppression* atau NMS guna memperoleh hasil deteksi akhir yang akurat (Redmon dkk., 2016). Prinsip deteksi satu tahap ini menjadi dasar perancangan arsitektur YOLO hingga versi YOLOv11.

## 2.9 YOLOv11

YOLO merupakan kerangka kerja deteksi objek satu tahap yang memproses citra secara langsung dari piksel masukan menuju koordinat kotak pembatas dan kelas objek dalam satu lintasan inferensi tunggal (Redmon dkk., 2016). Generasi terbaru arsitektur ini, YOLOv11, dirancang oleh Ultralytics (2024) dengan memperkenalkan optimasi efisiensi parameter dan pemodelan fitur multiskala. Diagram arsitektur jaringan YOLOv11 disajikan pada Gambar 2.8.

![Gambar 2.8 Arsitektur Jaringan YOLOv11](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_1_arsitektur_yolov11.png)

**Gambar 2.8 Arsitektur Jaringan YOLOv11**

Gambar 2.8 memperlihatkan struktur modular YOLOv11 yang terdiri atas tiga komponen utama: *Backbone*, *Neck*, dan *Head*. Pada *Backbone*, modul C3k2 digunakan untuk mengekstrak fitur spasial kemasan secara efisien. Peta fitur kemudian diagregasi pada lapisan leher menggunakan modul SPPF dan jaringan piramida fitur terpadu, sebelum diteruskan ke kepala deteksi *anchor-free* untuk memprediksi kotak pembatas tiga atribut kemasan: `brand_name`, `net_content`, dan `product_type`.

Pelatihan model deteksi objek YOLOv11 mengoptimalkan fungsi kerugian terpadu L_YOLO yang mengintegrasikan galat regresi kotak pembatas dan galat klasifikasi kategori, sebagaimana dirumuskan pada Persamaan (2.16):



![Persamaan 2.16](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_16.png)



Komponen L_CIoU mengoptimalkan keselarasan spasial kotak pembatas dengan memperhitungkan jarak pusat Euclidean, rasio aspek proporsional, dan tumpang tindih luas irisan. Komponen L_DFL atau *Distribution Focal Loss* memodelkan batas koordinat sebagai distribusi probabilitas kontinu untuk menangani ketidakpastian tepi label kemasan yang kabur, sedangkan L_BCE mengevaluasi ketepatan prediksi kelas objek atribut kosmetik.

## 2.10 Rekognisi Teks

*Optical Character Recognition* (OCR) atau rekognisi teks merupakan teknologi dalam bidang visi komputer dan pengenalan pola yang berfungsi mengubah citra digital berisi tulisan menjadi representasi teks digital yang dapat dibaca dan diproses oleh komputer (Chen dkk., 2021). Dalam sistem deteksi terpadu, OCR berfungsi sebagai tahap pemrosesan lanjutan setelah model deteksi objek melokalisasi wilayah teks target. Setelah kotak pembatas objek teks berhasil dideteksi dan disegmentasi, modul OCR mengekstraksi karakter dari potongan citra tersebut menjadi format teks digital alfanumerik yang siap diolah lebih lanjut (Hanif dkk., 2023).

Mekanisme kerja sistem OCR melibatkan serangkaian tahapan komputasi yang terstruktur guna memastikan keakuratan pengenalan karakter dari citra yang diproses (Hanif dkk., 2023). Alur tahapan dan komponen sistem OCR disajikan pada Gambar 2.9.

![Gambar 2.9 Komponen Sistem Rekognisi Teks OCR](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_8_komponen_sistem_ocr.png)

**Gambar 2.9 Komponen Sistem Rekognisi Teks OCR**

Berdasarkan bagan alir pada Gambar 2.9, mekanisme kerja sistem OCR tersusun atas tujuh komponen pemrosesan berurutan (Hanif dkk., 2023):
1. *Optical Scanning*: Proses awal saat dokumen atau kemasan fisik ditangkap oleh sensor kamera digital untuk menghasilkan representasi matriks citra digital sebagai masukan bagi tahapan komputasi berikutnya.
2. *Binarization*: Tahap pengubahan citra berwarna atau derajat keabuan (*grayscale*) menjadi citra biner melalui teknik pengambangan (*thresholding*). Piksel dengan nilai intensitas di atas ambang batas diklasifikasikan sebagai putih (1) dan yang berada di bawah ambang batas diklasifikasikan sebagai hitam (0) guna menghasilkan representasi kontras yang sederhana dan terpisah dari latar belakang.
3. *Location Segmentation*: Tahap analisis wilayah citra biner untuk melokalisasi area yang memuat teks. Segmentasi lokasi ini bertujuan mengarahkan fokus pemrosesan sistem pada area teks yang relevan dan mengabaikan bagian kanvas yang tidak diperlukan.
4. *Preprocessing*: Rangkaian perbaikan kualitas kontur karakter teks yang mencakup:
   a. *Filling*: Mengisi area celah kosong di dalam badan karakter agar struktur karakter menjadi lebih pejal (*solid*).
   b. *Thinning*: Mereduksi ketebalan goresan garis karakter menjadi satu piksel guna mempermudah analisis topologi huruf.
   c. *Normalization*: Menyeragamkan ukuran dimensi dan orientasi karakter agar konsisten dengan skala acuan model.
   d. *Skew Correction*: Mengoreksi sudut kemiringan citra teks guna memastikan baris tulisan berada pada orientasi horizontal yang sejajar.
5. *Feature Extraction*: Tahap pengambilan fitur representatif dari karakter yang telah dipraproses. Fitur visual yang diekstraksi mencakup bentuk geometri, kurvatur, dan rasio kerapatan kontur menggunakan metode berbasis fitur (*feature-based*) maupun pencocokan pola (*template matching*).
6. *Classification*: Tahap inferensi saat algoritma klasifikasi memetakan fitur yang telah diekstraksi menuju identitas kelas karakter alfanumerik yang sesuai berdasarkan bobot model yang telah dilatih.
7. *Recognition Post-processing*: Tahap pascapemrosesan yang meliputi pengelompokan karakter terisolasi menjadi susunan kata dan kalimat serta penerapan deteksi kesalahan ortografi guna meningkatkan akurasi akhir transkripsi teks.

Dalam verifikasi katalog kosmetik, keakuratan rekognisi teks pada tingkat karakter menjadi faktor penentu. Karakteristik isi bersih seperti angka satuan "30 ml" dan "50 ml" atau perbedaan ejaan nama merek seperti "Innisfree" dan "Inisfree" hanya dibedakan oleh satu karakter. Kesalahan rekognisi pada tingkat satu karakter ini berdampak langsung pada keabsahan status verifikasi katalog.

## 2.11 PaddleOCR

PaddleOCR merupakan kerangka kerja pengenalan karakter optis berskala industri yang dikembangkan oleh Baidu (Du dkk., 2020). Sistem ini mengintegrasikan detektor teks berbasis kontur bebas bentuk dan rekognisi teks sekuensial berakurasi tinggi ke dalam satu alur kerja yang ringkas. Arsitektur sistem PaddleOCR disajikan pada Gambar 2.10.

![Gambar 2.10 Arsitektur Sistem PaddleOCR](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_3_arsitektur_paddleocr.png)

**Gambar 2.10 Arsitektur Sistem PaddleOCR**

Gambar 2.10 memperlihatkan alur kerja sistem PaddleOCR yang menggabungkan model deteksi teks DBNet++ dan model pengenal karakter sekuensial SVTR. Model deteksi teks melokalisasi poligon area teks kemasan secara adaptif, kemudian wilayah teks tersebut dipotong dan diluruskan posisinya sebelum diproses oleh modul rekognisi karakter SVTR guna menghasilkan transkripsi teks akhir.

Pada tahap deteksi teks, arsitektur DBNet++ berbasis *differentiable binarization* memecahkan kendala binarisasi citra tradisional dengan menyematkan operasi binarisasi terperinci langsung ke dalam fungsi diferensial jaringan saraf konvolusi. Nilai binarisasi terdiferensiasi hat{B}_{i,j} pada koordinat (i, j) dihitung terhadap peta probabilitas P dan peta ambang batas adaptif T sesuai Persamaan (2.17):



![Persamaan 2.17](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_17.png)



dengan faktor pengali kemiringan kurva k yang ditetapkan sebesar 50. Fungsi kerugian total detektor DBNet++ L_DB dirumuskan pada Persamaan (2.18):



![Persamaan 2.18](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_18.png)



dengan L_s menyatakan *binary cross-entropy loss* pada peta probabilitas, L_b menyatakan kerugian binarisasi terdiferensiasi, dan L_t menyatakan kerugian *smooth L1* pada peta ambang batas. Pada tahap rekognisi teks, arsitektur SVTR menguraikan citra karakter menjadi urutan token visual tanpa ketergantungan pada jaringan saraf berulang RNN. Pelatihan rekognisi dioptimalkan menggunakan fungsi kerugian CTC yang menghitung probabilitas urutan label bersyarat l terhadap matriks representasi visual H_{SVTR}, sebagaimana dinyatakan pada Persamaan (2.19):



![Persamaan 2.19](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_19.png)



## 2.12 Vision-Language

Model visi-bahasa atau *Vision-Language Model* merupakan arsitektur multimodal terpadu yang menggabungkan representasi visual citra dari ranah visi komputer dan representasi teks dari ranah pemrosesan bahasa alami ke dalam satu ruang semantik bersama (Wang dkk., 2022). Berbeda dengan sistem visi komputer konvensional yang memproses data citra secara terisolasi tanpa pemahaman konteks linguistik, integrasi visi-bahasa memungkinkan sistem melakukan penalaran komprehensif terhadap informasi visual dan teks secara simultan (Wang dkk., 2024).

Fondasi utama pengekstraksi fitur visual pada model visi-bahasa modern bertumpu pada arsitektur *Vision Transformer* atau ViT (Dosovitskiy dkk., 2020). Berbeda dengan *Convolutional Neural Network* yang menggunakan operasi penapisan kernel geser lokal, *Vision Transformer* memecah kanvas citra masukan menjadi sekumpulan blok petak berukuran tetap yang disebut *patch* (Guo dkk., 2022). Setiap *patch* citra diratakan (*flatten*) dan diproyeksikan secara linier menjadi vektor *embedding* satu dimensi yang diperlakukan layaknya token kata pada pemrosesan bahasa alami. Diagram arsitektur *Vision Transformer* disajikan pada Gambar 2.11.

![Gambar 2.11 Arsitektur Vision Transformer pada Model Visi-Bahasa](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_10_arsitektur_vision_transformer.png)

**Gambar 2.11 Arsitektur Vision Transformer pada Model Visi-Bahasa**

Berdasarkan struktur arsitektur pada Gambar 2.11, representasi citra diproses melalui blok *encoder* yang tersusun atas lapisan *Multi-Head Self-Attention* (MSA) dan blok *Multi-Layer Perceptron* (MLP) (Guo dkk., 2022). Setiap petak citra x_p in mathbb{R}^{P^2 times C} diproyeksikan menggunakan matriks bobot linier E serta digabungkan dengan token kelas x_{class} dan penanda posisi satu dimensi E_{pos} guna mempertahankan urutan spasial, sebagaimana dirumuskan pada Persamaan (2.20):



![Persamaan 2.20](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_20.png)



Aliran informasi pada setiap lapisan encoder ell = 1, dots, L dinormalisasi menggunakan *Layer Normalization* (LN) dan dihubungkan oleh koneksi residual melintasi mekanisme *Multi-Head Self-Attention*, sebagaimana dinyatakan pada Persamaan (2.21):



![Persamaan 2.21](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_21.png)



Vektor hasil atensi kemudian ditransformasikan kembali melalui blok *Multi-Layer Perceptron* dengan koneksi residual sesuai formulasi Persamaan (2.22):



![Persamaan 2.22](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_22.png)



Representasi akhir luaran visual y diperoleh dari normalisasi vektor representasi pada simpul token utama sesuai Persamaan (2.23):



![Persamaan 2.23](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_23.png)



Vektor representasi visual y tersebut selanjutnya diproyeksikan ke dalam ruang dimensi laten model bahasa melalui proyektor antarmuka multimodal. Melalui konvergensi ini, model visi-bahasa memiliki kapabilitas membaca teks padat (*dense text*) sekaligus memahami relasi semantik antara wujud visual fisik kemasan dan klaim atribut pada katalog niaga elektronik. Pada tugas verifikasi katalog kosmetik, integrasi ini memungkinkan model memvalidasi kesesuaian antara klaim nama sediaan pada teks judul dengan wujud fisik kemasan secara terpadu tanpa bergantung pada pemisahan modul deteksi dan pembaca teks yang rentan terhadap galat perambatan (*cascading error*).

## 2.13 Qwen2-VL

Qwen2-VL merupakan model fondasi visi-bahasa yang dikembangkan oleh tim riset Alibaba Cloud (Wang dkk., 2024). Arsitektur ini dirancang untuk mengatasi kelemahan model multimodal konvensional yang kerap merusak teks beresolusi mikro akibat distorsi penskalaan ukuran kanvas citra yang kaku. Diagram arsitektur penalaran terpadu Qwen2-VL disajikan pada Gambar 2.12.

![Gambar 2.12 Arsitektur Agentic MLLM Qwen2-VL ReAct](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_4_arsitektur_qwen2vl_react.png)

**Gambar 2.12 Arsitektur Agentic MLLM Qwen2-VL ReAct**

Gambar 2.12 memperlihatkan alur kerja model Qwen2-VL yang memanfaatkan mekanisme *Dynamic Resolution* untuk memproses citra kemasan pada rasio aspek aslinya tanpa distorsi penskalaan. Token visual yang diekstraksi oleh *Vision Transformer* disisipkan dengan koordinat posisi spasial-temporal 3D menggunakan M-RoPE, lalu diproses oleh blok transformator bahasa melalui siklus penalaran ReAct guna memverifikasi atribut kemasan kosmetik secara interaktif.

Inovasi utama pada Qwen2-VL terletak pada mekanisme penanganan resolusi dinamis atau *dynamic resolution*. Berbeda dengan arsitektur terdahulu yang memaksakan pemotongan citra ke dimensi kanvas statis seperti 224 × 224 atau 448 times 448 piksel, Qwen2-VL memetakan citra kemasan masukan menjadi sekumpulan token visual dengan jumlah dinamis yang proporsional terhadap ukuran asli objek. Pendekatan ini menjaga ketajaman karakter teks label mikro pada kemasan kosmetik.

Untuk menyelaraskan posisi spasial token visual terhadap posisi sekuensial token bahasa, Qwen2-VL menerapkan *Multimodal Rotary Position Embedding* atau M-RoPE tiga dimensi. M-RoPE menguraikan komponen posisi absolut menjadi tiga sumbu koordinat independen: sumbu temporal t, sumbu vertikal tinggi h, dan sumbu horizontal lebar w. Formulasi vektor kueri q setelah penyisipan M-RoPE dirumuskan pada Persamaan (2.24):



![Persamaan 2.24](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_24.png)



dengan R_{Theta, cdot}^{(cdot)} menyatakan matriks rotasi frekuensi harmonik ortogonal. Pengkodean posisi spasial 3D ini memungkinkan model mempertahankan integritas geometri teks kemasan dan mengenali orientasi karakter secara presisi.

## 2.14 Kuantisasi AWQ

Model visual bahasa Qwen2-VL dengan 7 miliar parameter membutuhkan memori GPU sekitar 15,2 GB pada format standar FP16. Kebutuhan memori tersebut menyulitkan penerapan model pada komputer atau server dengan kapasitas kartu grafis terbatas. Untuk mengatasi kendala tersebut, penelitian ini menerapkan metode kompresi bobot Activation-aware Weight Quantization atau AWQ ke dalam format 4-bit (Danendra, 2026; Lin dkk., 2024).

Kuantisasi bekerja dengan mengubah nilai bobot model dari bilangan riil presisi tinggi menjadi bilangan bulat presisi rendah agar ukuran berkas mengecil dan penggunaan daya komputasi lebih hemat. Perbandingan antara penurunan presisi, efisiensi energi, dan akurasi model disajikan pada Gambar 2.13.

![Gambar 2.13 Perbandingan Efisiensi Energi dan Retensi Akurasi pada Tingkat Kuantisasi](figures/gambar_2_kuantisasi_isenkul.png)

**Gambar 2.13 Perbandingan Efisiensi Energi dan Retensi Akurasi pada Tingkat Kuantisasi (Isenkul, 2025; Danendra, 2026)**

Pada Gambar 2.13 disajikan grafik hubungan antara penurunan presisi angka dengan efisiensi energi dan akurasi model. Penurunan format dari FP32 ke FP16 dan INT8 dapat meningkatkan kecepatan serta efisiensi pemrosesan dengan penurunan akurasi yang kecil. Namun, penurunan ke format 4-bit atau INT4 dapat menurunkan akurasi model jika dilakukan secara langsung tanpa perlakuan khusus. Pada model bahasa dan visi, penurunan akurasi tersebut terjadi karena sekitar 1% saluran aktivasi memiliki nilai yang jauh lebih besar dan membawa informasi penting bagi pemahaman model.

Metode AWQ mengatasi masalah tersebut dengan melindungi 1% bobot penting melalui penskalaan nilai saluran aktivasi masukan. Metode ini mengalikan bobot penting dengan nilai skala tertentu dan membagi aktivasi dengan nilai yang sama, sehingga hasil perkalian matriks tetap sama sesuai persamaan matematis Y = WX = (W cdot diag(s)) cdot (diag(s)^{-1} X). Nilai skala optimal s* dihitung menggunakan data contoh kecil tanpa memerlukan pelatihan ulang model, sebagaimana dirumuskan pada Persamaan (2.25):



![Persamaan 2.25](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_25.png)



Simbol Q(·) menyatakan fungsi pembulatan nilai ke bilangan bulat 4-bit INT4. Saat model dijalankan pada GPU, bobot disimpan dalam format INT4 di memori dan diubah kembali ke FP16 secara langsung saat proses perkalian matriks berlangsung bersama data masukan.

Perbandingan kebutuhan memori dan karakteristik model Qwen2-VL-7B-Instruct pada berbagai format presisi disajikan pada Tabel 2.2.

**Tabel 2.2 Perbandingan Format Presisi dan Penggunaan Memori GPU Model Qwen2-VL**

| Format Presisi | Jumlah Bit Bobot | Jumlah Bit Aktivasi | Ukuran Memori GPU | Kebutuhan Minimal GPU | Penurunan Akurasi |
| :--- | :---: | :---: | :---: | :--- | :---: |
| **FP16** | 16 bit | 16 bit | 15,2 GB | GPU 24 GB (A100 atau RTX 4090) | 0,0% |
| **INT8** | 8 bit | 16 bit | 8,1 GB | GPU 12 GB (RTX 3060) | Kurang dari 1,2% |
| **AWQ 4-bit** | **4 bit** | **16 bit** | **5,8 GB** | **GPU 8 GB (Tesla T4 atau RTX 3050)** | **Kurang dari 0,5%** |

Penerapan metode AWQ 4-bit berhasil menurunkan penggunaan memori GPU model Qwen2-VL-7B dari 15,2 GB menjadi 5,8 GB. Pengurangan ukuran memori ini memungkinkan model dijalankan secara stabil pada GPU NVIDIA Tesla T4 16 GB tanpa kendala kehabisan memori dan tetap mampu membaca teks pada kemasan produk dengan baik.

## 2.15 Siklus ReAct

Model visual bahasa sering menghasilkan kesalahan informasi atau halusinasi saat membaca teks berukuran kecil dalam satu proses inferensi langsung. Untuk mengatasi kendala tersebut, sistem menerapkan kerangka kerja ReAct yang memadukan proses penalaran dengan eksekusi tindakan secara bertahap (Yao dkk., 2023).

Kerangka kerja ReAct menghubungkan proses berpikir model dengan eksekusi alat bantu terprogram. Alur kerja ReAct pada agen visual Qwen2-VL disajikan pada Gambar 2.14.

![Gambar 2.14 Alur Siklus Penalaran ReAct pada Agen Visual](figures/gambar_2_14_siklus_react.png)

**Gambar 2.14 Alur Siklus Penalaran ReAct pada Agen Visual (Yao dkk., 2023)**

Gambar 2.14 memperlihatkan alur kerja sistem yang memproses citra fisik kemasan dan teks klaim katalog melalui perulangan bertahap hingga menghasilkan keputusan verifikasi akhir. Siklus ReAct tersusun atas tiga tahapan yang berjalan secara berulang:
1. Pemikiran: Model menganalisis status visual saat ini dan menentukan tindakan yang perlu diambil untuk mencari bukti atribut yang belum lengkap.
2. Tindakan: Model memanggil fungsi terprogram untuk memanipulasi citra, seperti memotong area teks tertentu atau meningkatkan ketajaman kontras label.
3. Pengamatan: Model menerima hasil potongan citra resolusi tinggi dari lingkungan eksekusi untuk memperbarui konteks pemahaman sebelum melanjutkan ke tahap berikutnya.

Kebijakan penalaran dan tindakan terpadu π_ReAct pada langkah ke-t terhadap riwayat konteks interaksi c_t dimodelkan melalui fungsi probabilitas gabungan sesuai Persamaan (2.26):



![Persamaan 2.26](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_26.png)



Simbol r_t menyatakan hasil pemikiran model, a_t menyatakan fungsi tindakan yang dipilih, dan c_t menyatakan riwayat konteks interaksi hingga langkah ke-t. Fungsi P_{Qwen2-VL}( r_t mid c_t ) menyatakan probabilitas pembentukan pemikiran berdasarkan riwayat konteks, sedangkan P_{tool}( a_t mid c_t, r_t ) menyatakan probabilitas pemilihan tindakan berdasarkan pemikiran yang terbentuk.

Pada penelitian ini, model Qwen2-VL memanggil tiga fungsi terprogram untuk memverifikasi atribut kemasan kosmetik:
1. Fungsi `crop_roi`: memotong area label tertentu pada koordinat kotak pembatas untuk memperbesar teks merek atau angka isi bersih yang berukuran kecil.
2. Fungsi `enhance_patch`: meningkatkan kontras lokal pada potongan citra menggunakan metode CLAHE untuk memperjelas teks yang terhalang pantulan cahaya.
3. Fungsi `finalize_verdict`: menghentikan siklus penalaran serta menetapkan status verifikasi akhir dan nilai atribut kemasan yang terdeteksi.

Sistem membatasi perulangan siklus ReAct maksimal sebanyak 5 langkah untuk menjaga efisiensi waktu komputasi. Proses verifikasi menghasilkan status cocok apabila nama merek, kuantitas isi bersih, dan tipe produk sesuai dengan klaim katalog. Sebaliknya, sistem menetapkan status tidak cocok apabila salah satu atribut terbukti bertolak belakang antara fisik kemasan dan klaim katalog.

## 2.16 Pencocokan Teks

Pencocokan teks berfungsi membandingkan string teks yang berhasil diekstraksi dari kemasan fisik terhadap teks klaim yang tercantum pada metadata katalog Sociolla. Dalam operasional niaga elektronik, perbedaan ejaan string sering dipicu oleh salah pengetikan aksara, variasi singkatan satuan seperti variasi penulisan 50 ml dan 50ml, atau penulisan tanda baca. Oleh karena itu, verifikasi teks tidak dapat mengandalkan perbandingan persis secara biner, melainkan memerlukan metrik keselarasan berbasis jarak ortografis.

Tingkat perbedaan ortografis antara dua untaian teks dihitung menggunakan algoritma jarak Levenshtein. Jarak Levenshtein D_Lev(i, j) antara dua string s₁ dan s₂ mengukur jumlah minimum operasi penyisipan, penghapusan, atau penggantian karakter yang diperlukan untuk mengubah string s₁ menjadi string s₂, sebagaimana dirumuskan pada Persamaan (2.27):



![Persamaan 2.27](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_27.png)



dengan I(·) menyatakan fungsi indikator biner bernilai 1 jika karakter tidak sama dan 0 jika karakter identik. Untuk membandingkan pasangan string secara proporsional, nilai jarak dinormalisasi menjadi skor kemiripan S_Lev(s₁, s₂) dengan rentang nilai antara 0 hingga 1 sesuai Persamaan (2.28):



![Persamaan 2.28](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_28.png)



Pada alur deteksi spasial YOLOv11 dan PaddleOCR, keterkaitan antara kotak pembatas atribut detektor dan kotak teks OCR ditentukan menggunakan rasio *Intersection over Area* atau IoA. IoA mengukur proporsi tumpang tindih luas kotak teks OCR B_OCR yang tercakup di dalam kotak label deteksi B_YOLO, dirumuskan pada Persamaan (2.29):



![Persamaan 2.29](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_29.png)



Teks OCR diasosiasikan secara sah ke dalam atribut label terkait apabila nilai IoA ge 0{,}50.

## 2.17 Metrik Evaluasi

Evaluasi performa sistem verifikasi katalog kosmetik diukur menggunakan dua dimensi evaluasi: kualitas transkripsi karakter teks fisik dan ketepatan klasifikasi keputusan verifikasi katalog.

Kualitas transkripsi teks diukur menggunakan metrik kesalahan karakter CER dan kesalahan kata WER. Formulasi CER dan WER dihitung berdasarkan agregasi operasi substitusi (S), penghapusan (D), penyisipan (I), serta total panjang karakter atau kata referensi acuan (N), sebagaimana dirumuskan pada Persamaan (2.30) dan Persamaan (2.31):



![Persamaan 2.30](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_30.png)





![Persamaan 2.31](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_31.png)



Pada dimensi evaluasi klasifikasi verifikasi, keputusan akhir model pada masing-masing atribut kemasan: `brand_name`, `net_content`, dan `product_type` diklasifikasikan ke dalam matriks konfusi: *True Positive*, *False Positive*, *False Negative*, dan *True Negative*. Formulasi metrik Akurasi, Presisi, *Recall*, dan *F1-Score* dirumuskan pada Persamaan (2.32), Persamaan (2.33), dan Persamaan (2.34):



![Persamaan 2.32](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_32.png)





![Persamaan 2.33](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_33.png)





![Persamaan 2.34](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_34.png)



Guna mengevaluasi performa agregat pada seluruh kelas atribut secara adil di tengah ketidakseimbangan frekuensi sampel, dihitung nilai *Macro-F1* dan *Micro-F1* sesuai Persamaan (2.35) dan Persamaan (2.36):



![Persamaan 2.35](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_35.png)





![Persamaan 2.36](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_36.png)



Selain metrik kualitas prediksi, efisiensi operasional sistem diuji berdasarkan latensi inferensi komputasi rata-rata per citra dalam satuan milidetik dan konsumsi puncak alokasi memori GPU VRAM dalam satuan megabita.

## 2.18 Uji McNemar

Untuk membuktikan apakah perbedaan performa verifikasi antara Pipeline Konvensional Hibrida YOLOv11m-PaddleOCR dan Pipeline Agentic MLLM Qwen2-VL bersifat nyata secara statistik atau sekadar terjadi secara kebetulan, diterapkan uji beda inferensial non-parametrik uji McNemar (McNemar, 1947). Uji McNemar dirancang khusus untuk menguji signifikansi perbedaan antara dua model klasifikasi yang diuji pada dataset nominal berpasangan yang identik.

Hasil pengujian kedua model dipetakan ke dalam tabel kontingensi 2 × 2 yang disajikan pada Tabel 2.3.

**Tabel 2.3 Tabel Kontingensi Uji McNemar**

| | Pipeline Agentic MLLM Benar | Pipeline Agentic MLLM Salah |
|:---|:---:|:---:|
| **Pipeline Konvensional Benar** | a | b |
| **Pipeline Konvensional Salah** | c | d |

Fokus analisis uji McNemar bertumpu pada sel diskordan, yaitu sel b , yaitu sampel yang diverifikasi benar oleh Pipeline Konvensional namun salah oleh Pipeline Agentic, dan sel c , yaitu sampel yang diverifikasi salah oleh Pipeline Konvensional namun benar oleh Pipeline Agentic,. Statistik uji Chi-kuadrat McNemar (chi^2) dengan koreksi kontinuitas Edwards dirumuskan pada Persamaan (2.37):



![Persamaan 2.37](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/formulas/eq_2_37.png)



Nilai statistik χ²_McNemar yang dihitung dibandingkan terhadap nilai kritis distribusi Chi-kuadrat pada derajat kebebasan df = 1 dengan taraf signifikansi alpha = 0{,}05, yaitu chi^2_{kritis} = 3{,}841. Jika nilai hitung chi^2 > 3{,}841 atau nilai signifikansi p-value < 0{,}05, maka perbedaan kinerja antara kedua pipeline terbukti signifikan secara statistik.

## 2.19 Model Konseptual

Model konseptual penelitian dirancang untuk menggambarkan kerangka pemikiran sistematis yang menghubungkan identifikasi permasalahan operasional katalog, pemilihan metode komparasi kecerdasan buatan, parameter pengujian empiris, hingga perancangan luaran sistem terapan. Diagram model konseptual disajikan pada Gambar 2.15.

![Gambar 2.15 Model Konseptual Penelitian](https://raw.githubusercontent.com/Alarave/skripsi-figures/main/gambar_2_1_kerangka_pemikiran.png)

**Gambar 2.15 Model Konseptual Penelitian**

Bagan alir pada Gambar 2.15 memvisualisasikan alur penelitian yang tersusun ke dalam empat komponen utama yang berkesinambungan:
1. Komponen Masalah Operasional: Berangkat dari fakta ketidaksesuaian spesifikasi katalog kosmetik terhadap kemasan fisik, kendala pantulan cahaya studio, karakter teks mikro, serta keterbatasan prosedur kurasi visual manual yang lambat dan berbiaya tinggi.
2. Komponen Intervensi Metode: Merancang komparasi terarah antara dua paradigma komputasi pada dataset 5.358 citra katalog Sociolla yang dipartisi bebas kebocoran merek dengan rasio 70:15:15:
   a. Pipeline Multimodal Konvensional Hibrida: Menggabungkan detektor objek YOLOv11m untuk melokalisasi area label dan mesin PaddleOCR PP-OCRv4 untuk membaca teks atribut secara deterministik.
   b. Pipeline Agentic MLLM: Mengonfigurasi model Qwen2-VL-7B-Instruct AWQ 4-bit berbasis siklus penalaran ReAct meliputi pemikiran, tindakan, dan pengamatan dan alat inspeksi visual mikro secara adaptif.
3. Komponen Evaluasi Empiris: Mengukur kinerja kedua model pada 804 data uji independen menggunakan metrik transkripsi CER dan WER, metrik klasifikasi verifikasi meliputi akurasi, presisi, *recall*, dan *F1-score*, efisiensi komputasi berupa latensi inferensi dan konsumsi VRAM, serta uji signifikansi statistik inferensial McNemar pada taraf α = 0,05.
4. Komponen Luaran Sistem: Mengimplementasikan model dengan efektivitas terbaik ke dalam aplikasi dasbor web Streamlit yang menyajikan visualisasi verifikasi berdampingan, jejak inspeksi penalaran, dan rekomendasi perbaikan penulisan katalog sesuai regulasi BPOM.

## 2.20 Hipotesis Penelitian

Berdasarkan tinjauan pustaka dan model konseptual yang telah diuraikan, hipotesis penelitian yang diajukan untuk diuji kebenarannya secara statistik dalam penelitian ini ditetapkan sebagai berikut:

1. Hipotesis Nol (H₀):
   Tidak terdapat perbedaan kinerja yang signifikan antara Pipeline Konvensional Hibrida YOLOv11m-PaddleOCR PP-OCRv4 dan Pipeline Agentic MLLM Qwen2-VL-7B-Instruct AWQ 4-bit dalam memverifikasi keselarasan atribut kemasan katalog kosmetik Sociolla berdasarkan uji statistik McNemar pada taraf signifikansi α = 0,05 (p ge 0,05).

2. Hipotesis Alternatif (H₁):
   Terdapat perbedaan kinerja yang signifikan antara Pipeline Konvensional Hibrida YOLOv11m-PaddleOCR PP-OCRv4 dan Pipeline Agentic MLLM Qwen2-VL-7B-Instruct AWQ 4-bit dalam memverifikasi keselarasan atribut kemasan katalog kosmetik Sociolla berdasarkan uji statistik McNemar pada taraf signifikansi α = 0,05 (p < 0,05).
