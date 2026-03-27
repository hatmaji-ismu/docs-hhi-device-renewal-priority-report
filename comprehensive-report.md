# Laporan Komprehensif Prioritas Penggantian Perangkat HHI

## Ringkasan Eksekutif
Laporan ini merupakan sintesis dari 12 laporan penilaian perangkat keras dan satu dokumen penilaian kualitatif pengguna. Tujuan utamanya adalah menyusun dasar keputusan penggantian perangkat yang tidak hanya bertumpu pada spesifikasi teknis, tetapi juga pada dampak nyata terhadap pekerjaan harian, seperti kelambatan sistem, pembekuan aplikasi, `BSOD`, mati mendadak, kerusakan fisik, penurunan kualitas baterai, serta gangguan terhadap rapat daring dan pekerjaan administrasi.

Berdasarkan penggabungan bukti teknis dan temuan operasional, distribusi prioritas armada saat ini adalah sebagai berikut:

| Kategori Prioritas | Jumlah Unit | Persentase | Makna Operasional |
| :--- | :---: | :---: | :--- |
| Penggantian segera | 5 | 41,7% | Unit sudah menunjukkan kombinasi hambatan kerja nyata, keterbatasan perangkat keras berat, dan/atau risiko kestabilan tinggi |
| Penyegaran prioritas tinggi | 4 | 33,3% | Unit masih dapat dipakai sementara, tetapi produktivitasnya sudah tertekan dan perlu tindakan dalam batch berikutnya |
| Perbaikan/upgrade terlebih dahulu | 1 | 8,3% | Masalah utama cenderung bersumber dari perangkat lunak, konfigurasi, atau komponen tertentu; inti perangkat masih memadai |
| Pertahankan | 2 | 16,7% | Unit masih memenuhi fungsi operasional saat ini dan belum membutuhkan penggantian langsung |

Ada empat kesimpulan utama yang menonjol dari keseluruhan armada. Pertama, RAM 4 GB masih menjadi akar masalah paling konsisten. Delapan dari dua belas unit masih berada pada kapasitas ini, dan hampir semuanya menunjukkan penggunaan memori tinggi, ketergantungan besar pada `page file`, serta gejala penurunan responsivitas. Kedua, risiko tidak merata di seluruh armada. Beberapa unit perlu segera diganti karena kombinasi gejala yang berat, sedangkan unit lain cukup di-upgrade atau dipantau. Ketiga, kondisi operasional pengguna memengaruhi urgensi secara signifikan. Unit yang secara spesifikasi tampak “cukup” dapat menjadi sangat prioritas bila dipakai untuk pekerjaan yang sensitif terhadap gangguan, atau ketika sudah muncul `BSOD`, mati mendadak, baterai bocor, dan kerusakan periferal. Keempat, penggantian tidak boleh dipukul rata. Masih ada unit lama yang tetap layak dipertahankan karena perannya terbatas, stabil, atau hanya berfungsi sebagai sistem siaga.

Dengan demikian, keputusan manajerial yang paling rasional adalah menjalankan program penggantian bertahap. Batch pertama perlu difokuskan pada lima unit dengan risiko tertinggi, sedangkan batch kedua diarahkan pada unit yang masih dapat dipertahankan sementara tetapi sudah menekan produktivitas secara konsisten. Pendekatan ini memberi keseimbangan antara kesinambungan operasional, efisiensi biaya, dan penurunan risiko `downtime`.

## Tujuan, Ruang Lingkup, dan Dokumen Sumber
Laporan ini disusun untuk menjawab tiga kebutuhan organisasi secara bersamaan. Pertama, memetakan kondisi aktual perangkat yang saat ini digunakan. Kedua, membedakan mana unit yang harus segera diganti, mana yang masih layak di-upgrade atau diperbaiki terlebih dahulu, dan mana yang cukup dipelihara. Ketiga, menerjemahkan data teknis ke dalam implikasi bisnis agar keputusan pengadaan tidak berhenti pada angka spesifikasi.

Ruang lingkup analisis mencakup 12 unit berikut:

1. System Finance
2. Renaldi
3. Diana
4. Regina
5. Syela
6. Christy
7. Yohana
8. Hibab
9. Devinta
10. Wulan
11. Robin
12. System Autocount

Dokumen sumber yang digunakan:

* `HHI Assestment/System Finance/System_Finance_Hardware_Report.md`
* `HHI Assestment/Renaldi/Renaldi_Hardware_Report.md`
* `HHI Assestment/Diana/Diana_Hardware_Report.md`
* `HHI Assestment/Regina/Regina_Hardware_Report.md`
* `HHI Assestment/Syela/Syela_Hardware_Report.md`
* `HHI Assestment/Christy/Christy_Hardware_Report.md`
* `HHI Assestment/Yohana/Yohana_Hardware_Report.md`
* `HHI Assestment/Hibab/Hibab_Hardware_Report.md`
* `HHI Assestment/Devinta/Devinta_Hardware_Report.md`
* `HHI Assestment/Wulan/Wulan_Hardware_Report.md`
* `HHI Assestment/Robin/Robin_Hardware_Report.md`
* `HHI Assestment/System Autocount/System_Autocount_Hardware_Report.md`
* `qualitative-assessment.md`

Seluruh analisis pada laporan ini dibatasi oleh bukti yang tersedia di folder pemeriksaan. Jika ada komponen yang belum didukung bukti kesehatan secara lengkap, seperti verifikasi `health` penyimpanan pada unit Yohana, maka rekomendasi disusun dengan prinsip kehati-hatian dan tidak mengasumsikan kondisi terbaik tanpa verifikasi tambahan.

## Metodologi dan Prinsip Penilaian
Penentuan prioritas tidak dilakukan hanya dari usia perangkat atau angka `health` penyimpanan. Setiap unit dinilai melalui dua lapis bukti yang saling melengkapi.

### 1. Bukti teknis
Bukti teknis diambil dari `DxDiag`, catatan spesifikasi, bukti penggunaan RAM, serta tangkapan kondisi media penyimpanan. Unsur yang dinilai meliputi:

* kelas dan usia prosesor
* kapasitas RAM terpasang dan tingkat utilisasinya
* penggunaan `page file` sebagai indikator tekanan memori
* kesehatan penyimpanan, suhu, dan sisa ruang kosong
* status audio, GPU, dan driver penting
* arsitektur sistem operasi serta relevansinya terhadap perangkat

### 2. Bukti operasional
Bukti operasional diambil dari penilaian kualitatif yang memotret pengalaman pengguna saat bekerja. Unsur yang dijadikan pertimbangan meliputi:

* keluhan `lag`, `freeze`, dan aplikasi `not responding`
* kejadian `BSOD` dan mati mendadak
* gangguan terhadap Excel, Outlook, browser, sistem payroll, dan aplikasi lain yang kritikal
* kendala rapat daring akibat tidak adanya webcam, rusaknya mikrofon, atau baterai yang cepat habis
* kerusakan fisik seperti chassis patah, layar bermasalah, keyboard rusak, atau perangkat input yang tidak stabil
* konteks penggunaan, misalnya unit aktif harian dibanding sistem siaga

### 3. Prinsip klasifikasi prioritas
Untuk menjaga konsistensi terminologi, laporan ini menggunakan empat kategori berikut:

* **Penggantian segera**: dipakai untuk unit yang sudah menampilkan gangguan kerja nyata, risiko stabilitas tinggi, atau kombinasi keterbatasan teknis dan kerusakan fisik yang membuat perbaikan parsial tidak lagi efisien.
* **Penyegaran prioritas tinggi**: dipakai untuk unit yang masih dapat digunakan dalam jangka pendek, tetapi sudah membatasi produktivitas, mobilitas, atau keandalan kerja dan perlu masuk batch pengadaan berikutnya.
* **Perbaikan/upgrade terlebih dahulu**: dipakai untuk unit yang inti perangkat kerasnya masih cukup memadai dan masalah utamanya lebih mungkin diselesaikan melalui perbaikan sistem, penggantian komponen tertentu, atau upgrade terbatas.
* **Pertahankan**: dipakai untuk unit yang masih memenuhi fungsi bisnis saat ini, tidak memunculkan keluhan besar, atau berperan sebagai sistem siaga yang tetap stabil.

Dengan metodologi ini, rekomendasi akhir tidak sekadar menjawab “perangkat ini tua atau tidak”, melainkan “apakah perangkat ini masih layak menopang kerja aktual dengan risiko yang bisa diterima”.

## Sintesis Prioritas Armada
Secara keseluruhan, sembilan dari dua belas unit, atau 75%, sudah berada pada kategori yang membutuhkan keputusan aktif, baik berupa penggantian segera maupun penyegaran prioritas tinggi. Ini menunjukkan bahwa persoalan armada tidak lagi bersifat sporadis, melainkan struktural.

Tabel berikut merangkum profil, alasan prioritas, dan tindakan yang disarankan untuk setiap unit.

| Unit | Profil Singkat | Temuan Teknis Utama | Temuan Operasional Utama | Dampak Bisnis | Tindakan Disarankan | Prioritas |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **System Finance** | i3-4160, RAM 4 GB, Windows 10 32-bit, HDD | Platform sangat tua, RAM efektif rendah, driver lama, audio playback tidak terdeteksi | Sangat lambat untuk WhatsApp dan browser; koneksi internet kadang harus dipulihkan dengan restart | Produktivitas dasar terganggu dan platform sudah tidak sejalan dengan kebutuhan kerja modern | Ganti unit; upgrade parsial hanya layak sebagai penahan sementara | Penggantian segera |
| **Renaldi** | i5-8400, RAM 4 GB, SSD berstatus peringatan | RAM kritis, SSD 85%, suhu 66 C, ruang kosong 18,1 GB, reserved spare area terpakai | `Lag`, `freeze`, `BSOD`, tidak ada webcam untuk rapat daring | Risiko gangguan kerja dan kehilangan data tinggi | Ganti unit dan lakukan `backup` segera | Penggantian segera |
| **Diana** | i5-8400, RAM 4 GB, SSD panas | RAM kritis, `page file` tinggi, SSD 85% pada 61 C, ruang kosong terbatas | Sering `hang`, error saat membuka lebih dari dua file Excel, sering mati mendadak, lambat di ORS Payroll | Gangguan langsung pada pekerjaan administrasi dan indikasi masalah stabilitas listrik/termal | Ganti unit; jangan hanya mengandalkan upgrade RAM | Penggantian segera |
| **Regina** | i5-8265U, RAM 4 GB, laptop, SSD 75% | RAM 92%, `page file` sangat tinggi, `health` SSD menurun, driver menua | Sangat lambat, sering `BSOD`, chassis patah, baterai turun 50% dalam 15 menit | Unit tidak lagi andal untuk kerja mobile maupun kerja rutin | Ganti unit sesegera mungkin | Penggantian segera |
| **Syela** | i5-8400, RAM 4 GB, SSD 78% | RAM kritis, ruang kosong hanya 5,6 GB, suhu 54 C, `health` storage menurun | Tidak ada keluhan kualitatif spesifik, tetapi bukti teknis sudah menunjukkan tekanan berat | Risiko penurunan kinerja dan instabilitas akan terus meningkat | Ganti unit; sementara itu lakukan pembersihan ruang penyimpanan | Penggantian segera |
| **Christy** | i5-10210U, RAM 8 GB, laptop | RAM 89%, `page file` tinggi, driver GPU menua, storage masih sehat | Mikrofon rusak, keyboard rusak, membutuhkan penyimpanan lebih besar, menginginkan laptop ringkas | Kualitas kerja dan kesesuaian perangkat dengan peran pengguna menurun | Siapkan laptop pengganti dengan spesifikasi yang sesuai peran | Penyegaran prioritas tinggi |
| **Yohana** | i5-8400, RAM 4 GB, SSD 256 GB | RAM 92%, `page file` sangat tinggi, kondisi `health` storage belum tervalidasi, audio playback tidak terdeteksi | Monitor terlalu kecil, kursor sering hilang, mulai lambat saat banyak aplikasi terbuka | Produktivitas harian terganggu, tetapi belum ada bukti kegagalan total | Upgrade RAM dan perbaiki input/monitor sambil disiapkan untuk batch berikutnya | Penyegaran prioritas tinggi |
| **Hibab** | i5-7200U, RAM 4 GB, laptop | RAM 90%, `page file` tinggi, platform mobile lama, SSD masih sehat | Outlook lambat, baterai cepat habis, pengalaman rapat daring menurun | Masih dapat dipakai sementara, tetapi mobilitas dan kenyamanan kerja sudah buruk | Ganti baterai dan tambah RAM jika ingin menunda; siapkan penggantian | Penyegaran prioritas tinggi |
| **Devinta** | i5-8400, RAM 8 GB, SSD sehat | `page file` sangat tinggi, platform mulai menua, audio playback tidak terdeteksi | Belum ada keluhan lapangan berat, tetapi bukti teknis menunjukkan tekanan multitugas | Risiko penurunan produktivitas muncul dalam jangka menengah | Upgrade RAM ke 16 GB dan perbaiki audio; masukkan ke batch penyegaran | Penyegaran prioritas tinggi |
| **Wulan** | i5-10400, RAM 8 GB, SSD 88% | CPU masih memadai, RAM mulai sempit, `health` SSD menurun moderat, audio playback tidak terdeteksi | `Not Responding` setelah mengunduh PDF; gejalanya mengarah ke masalah perangkat lunak | Replacement belum mendesak; perbaikan sistem berpotensi menyelesaikan inti masalah | Lakukan perbaikan sistem/instal ulang OS; upgrade RAM bila perlu | Perbaikan/upgrade terlebih dahulu |
| **Robin** | i5-10400, RAM 8 GB, SSD 93% | RAM mulai tertekan, `page file` tinggi, audio playback tidak terdeteksi | Tidak ada kendala operasional bermakna; stabil untuk Excel | Belum ada alasan bisnis kuat untuk penggantian langsung | Pertahankan; audit audio bila diperlukan dan upgrade RAM bersifat opsional | Pertahankan |
| **System Autocount** | i5-8400, RAM 4 GB, SSD + HDD sehat | RAM tetap di bawah standar, tetapi storage sehat dan `page file` masih relatif terkendali | Sistem siaga Autocount masih berjalan baik, tanpa keluhan lapangan | Belum perlu diprioritaskan karena fungsi perannya masih terpenuhi | Pertahankan; upgrade RAM hanya jika beban kerja meningkat | Pertahankan |

## Temuan Lintas Armada
### 1. RAM 4 GB sudah berada di bawah ambang kelayakan kerja
Temuan paling konsisten di seluruh armada adalah keterbatasan memori. Delapan unit masih menggunakan RAM 4 GB, dan hampir semuanya menunjukkan pola yang sama: penggunaan memori tinggi, `page file` besar, penurunan responsivitas saat membuka Excel, browser, Outlook, atau beberapa aplikasi sekaligus, serta ruang kerja sistem yang terlalu sempit untuk multitugas. Bahkan pada unit dengan RAM 8 GB, gejala tekanan memori sudah mulai terlihat, sehingga organisasi perlu menaikkan standar minimum baru ke 16 GB untuk perangkat kerja aktif.

### 2. Realitas operasional mengubah bobot keputusan
Dokumen kualitatif memperjelas bahwa spesifikasi teknis tidak cukup untuk menentukan urgensi. Renaldi dan Regina bukan hanya “berusia tua”, tetapi sudah mengalami `BSOD`. Diana menunjukkan mati mendadak, yang menandakan risiko kestabilan lebih serius daripada sekadar unit yang terasa lambat. Sebaliknya, System Autocount tetap dipertahankan meskipun hanya memiliki RAM 4 GB, karena perannya sebagai sistem siaga masih berjalan stabil. Dengan kata lain, tingkat urgensi harus dibaca bersama konteks pekerjaan, bukan hanya berdasarkan usia perangkat.

### 3. Risiko penyimpanan bersifat selektif, bukan menyeluruh
Tidak semua unit membutuhkan tindakan pada media penyimpanan. Risiko tertinggi terlihat pada Renaldi, karena SSD sudah memakai reserved spare area, suhu tinggi, dan ruang kosong rendah. Syela dan Regina juga perlu pengawasan ketat karena `health` storage menurun atau ruang kosong kritis. Wulan masih perlu dipantau, tetapi belum menunjukkan kegagalan langsung. Di sisi lain, storage pada Robin, Christy, Hibab, Devinta, dan System Autocount relatif masih sehat. Artinya, strategi penggantian disk harus selektif agar biaya tidak salah sasaran.

### 4. Kerusakan periferal dan fisik sama pentingnya dengan spesifikasi inti
Gangguan produktivitas tidak selalu berasal dari CPU atau storage. Kerusakan mikrofon, keyboard, baterai, chassis, audio playback, ukuran monitor, serta ketidakstabilan perangkat input dapat menghambat kerja harian secara langsung. Christy membutuhkan laptop yang lebih sesuai dengan kebutuhan mobilitas dan penyimpanan. Regina sudah menunjukkan kombinasi kerusakan fisik dan degradasi baterai yang serius. Yohana mengalami gangguan input dan ergonomi monitor. Karena itu, evaluasi penggantian harus selalu memasukkan kelayakan perangkat dari sisi pengalaman penggunaan, bukan hanya performa komputasi.

### 5. Strategi pengadaan perlu dibedakan antara penggantian, penyegaran, dan pemeliharaan
Laporan ini menegaskan bahwa organisasi tidak perlu mengganti seluruh armada sekaligus. Lima unit sudah berada pada posisi ketika perbaikan parsial akan memberikan hasil terbatas. Empat unit lain masih dapat dipertahankan sebentar dengan intervensi transisi. Satu unit lebih tepat diperbaiki terlebih dahulu, dan dua unit lainnya cukup dipelihara. Pembagian ini penting agar anggaran diarahkan ke titik yang paling berdampak terhadap produktivitas dan kesinambungan layanan.

## Analisis Detail Per Unit
### 1. System Finance
**Profil singkat:** Desktop Gigabyte H81M-DS2 dengan Intel Core i3-4160, RAM 4 GB, Windows 10 Pro 32-bit, Intel HD Graphics 4400, dan HDD 500 GB yang masih sehat.

**Status komponen:** CPU kritis, GPU kritis, memori kritis, storage sehat.

**Temuan utama:** Unit ini menghadapi persoalan struktural. Sistem operasi 32-bit membuat RAM 4 GB tidak dapat dimanfaatkan penuh, sehingga kapasitas efektif hanya sekitar 3,41-3,49 GB. `page file` sudah terpakai 2300 MB, menandakan tekanan memori mulai nyata. Di sisi lain, GPU dan platform prosesor sudah sangat tertinggal untuk standar kerja 2026. Meskipun HDD masih sehat, penggunaan HDD pada platform setua ini tidak cukup untuk menutup ketertinggalan inti perangkat. Temuan kualitatif memperkuat kondisi tersebut: perangkat terasa sangat lambat saat menjalankan WhatsApp dan browser, dan koneksi internet kadang baru pulih setelah restart manual.

**Analisis:** Pada unit ini, masalahnya bukan satu komponen yang rusak, melainkan keseluruhan platform yang sudah terlalu tua. Opsi seperti migrasi ke sistem 64-bit, penambahan RAM, atau migrasi ke SSD memang dapat memperbaiki sebagian gejala, tetapi membutuhkan intervensi berlapis pada perangkat yang secara dasar sudah melewati ambang ekonomis untuk diremajakan. Karena itu, penggantian lebih rasional dibanding retrofit besar.

**Rekomendasi:** Masukkan ke batch penggantian segera. Bila pengadaan belum dapat dilakukan langsung, batasi penggunaan hanya untuk kebutuhan paling sederhana, verifikasi fungsi audio, dan minimalkan aplikasi latar belakang sebagai langkah mitigasi jangka sangat pendek.

### 2. Renaldi
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB, dan monitor HP 19ka.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage kritis.

**Temuan utama:** Penggunaan memori mencapai 87% dengan `page file` 6252 MB. SSD hanya menyisakan ruang kosong 18,1 GB, berada pada `health` 85%, bersuhu 66 C, dan sudah menggunakan reserved spare area sebagai pengganti sektor bermasalah. Ini adalah sinyal penting bahwa perangkat penyimpanan mulai memakan cadangan keandalannya. Dari sisi operasional, pengguna mengalami `lag`, `freeze`, `BSOD`, serta tidak memiliki webcam untuk rapat daring bulanan.

**Analisis:** Unit ini memiliki kombinasi risiko yang paling lengkap: RAM terlalu kecil, media penyimpanan mulai memburuk, suhu tinggi, ruang kosong sempit, dan gejala kestabilan sistem sudah nyata. Dalam konteks bisnis, masalah ini bukan hanya menurunkan kenyamanan kerja, tetapi juga memperbesar kemungkinan kehilangan data dan terhentinya pekerjaan ketika perangkat gagal.

**Rekomendasi:** Ganti unit secepatnya dan lakukan `backup` data sebagai tindakan prioritas pertama. Selama masa transisi, bersihkan drive sistem, perbaiki aliran udara, dan sediakan solusi rapat daring sementara bila pekerjaan menuntutnya.

### 3. Diana
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB, dan monitor HP 19ka.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage peringatan.

**Temuan utama:** Penggunaan memori berada di 85% dengan hanya 583 MB tersedia dan `page file` 5972 MB. SSD masih berada di `health` 85%, tetapi suhu mencapai 61 C dan ruang kosong tersisa 30 GB. Temuan kualitatif jauh lebih serius: perangkat sering `hang`, error ketika membuka lebih dari dua file Excel, lambat saat mengakses ORS Payroll, dan bahkan sering mati mendadak.

**Analisis:** Mati mendadak menandakan risiko yang melampaui bottleneck RAM biasa. Kemungkinan sumbernya bisa berasal dari catu daya, termal, atau kestabilan sistem yang lebih dalam. Karena unit dipakai untuk pekerjaan administrasi yang menuntut kontinuitas, setiap gangguan seperti ini langsung menambah risiko kehilangan pekerjaan, pengulangan input, dan penurunan kepercayaan pengguna terhadap sistem.

**Rekomendasi:** Tempatkan dalam kategori penggantian segera. Upgrade RAM saja tidak memadai sebagai solusi akhir. Selama menunggu penggantian, lakukan pembersihan aplikasi startup, cek pendinginan, dan pastikan ada kebiasaan penyimpanan berkala untuk mengurangi dampak mati mendadak.

### 4. Regina
**Profil singkat:** Laptop HP 240 G7 dengan Intel Core i5-8265U, RAM 4 GB, SSD NVMe 256 GB, dan grafis Intel UHD 620.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage peringatan.

**Temuan utama:** Penggunaan memori mencapai 92% dengan sisa hanya 283 MB, sedangkan `page file` sudah menyentuh 12982 MB. SSD masih berstatus baik, tetapi `health` turun ke 75%, sehingga tidak lagi bisa dianggap prima untuk pemakaian jangka menengah. Dari sisi operasional, unit ini sangat lambat untuk Excel dan Outlook, sering mengalami `BSOD`, memiliki chassis yang patah, dan baterainya turun sekitar 50% hanya dalam 15 menit.

**Analisis:** Regina adalah contoh unit yang tidak hanya menua, tetapi juga mulai tidak aman dan tidak andal secara fisik. Kerusakan fisik, `BSOD`, dan degradasi baterai ekstrem membuatnya tidak pantas lagi dijadikan perangkat kerja utama, terutama bila mobilitas dan stabilitas kerja menjadi kebutuhan. Pada titik ini, mempertahankan perangkat justru memperbesar biaya tidak langsung berupa frustrasi pengguna, waktu henti, dan risiko kerusakan lanjutan.

**Rekomendasi:** Lakukan penggantian segera. Prioritaskan pemindahan data dan pengamanan kerja pengguna ke unit pengganti. Unit lama sebaiknya tidak lagi menjadi perangkat utama setelah penggantian tersedia.

### 5. Syela
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 4 GB, dan SSD NVMe 256 GB.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage kritis.

**Temuan utama:** Penggunaan memori mencapai 87% dengan `page file` 9198 MB. SSD tinggal menyisakan ruang kosong 5,6 GB, `health` turun ke 78%, suhu berada di 54 C, dan perangkat lunak pemantauan merekomendasikan `continuous monitoring`. Tidak ada keluhan kualitatif khusus pada dokumen pendukung, tetapi bukti teknis sudah menunjukkan tekanan yang sangat tinggi.

**Analisis:** Ketiadaan keluhan kualitatif tidak serta-merta berarti unit aman. Dalam kasus ini, justru bukti teknis menunjukkan perangkat sedang berada pada posisi rawan: RAM sangat terbatas, storage hampir penuh, dan kesehatan disk sudah menurun. Jika dipertahankan terlalu lama, unit ini berpotensi beralih dari “lambat” menjadi “gagal bekerja” tanpa banyak peringatan.

**Rekomendasi:** Masukkan ke kategori penggantian segera. Sebelum penggantian terlaksana, lakukan pembersihan drive C sesegera mungkin dan kurangi beban aplikasi latar belakang untuk menurunkan tekanan sistem.

### 6. Christy
**Profil singkat:** Laptop ASUS VivoBook X412FLC dengan Intel Core i5-10210U, RAM 8 GB, SSD NVMe 256 GB, HDD 1 TB, Intel UHD Graphics, dan NVIDIA GeForce MX250.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage sehat.

**Temuan utama:** Penggunaan memori berada di 89% dengan `page file` 7449 MB. SSD dan HDD masih sehat, sehingga penyimpanan bukan sumber masalah utama saat ini. Namun, driver GPU mulai menua. Dokumen kualitatif menambahkan konteks yang sangat relevan: mikrofon rusak, keyboard rusak, pengguna membutuhkan ruang penyimpanan yang lebih besar, dan lebih cocok menggunakan laptop yang ringkas.

**Analisis:** Berbeda dari unit yang perlu segera diganti karena gagal total, Christy masih memiliki inti storage yang sehat. Akan tetapi, perangkat ini sudah tidak lagi selaras dengan kebutuhan peran pengguna. Kombinasi RAM yang tertekan, periferal yang rusak, dan kebutuhan form factor yang berbeda membuat opsi perbaikan menjadi kurang menarik bila dihitung dari manfaat jangka menengah.

**Rekomendasi:** Masukkan ke batch penyegaran prioritas tinggi. Perangkat pengganti sebaiknya berupa laptop ringkas dengan RAM 16 GB dan kapasitas penyimpanan yang sesuai kebutuhan kerja pengguna. Jika pengadaan tertunda, upgrade RAM dan perbaikan mikrofon/keyboard hanya layak sebagai jembatan sementara.

### 7. Yohana
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 4 GB, dan SSD 256 GB yang bukti kesehatannya belum lengkap.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage peringatan.

**Temuan utama:** Penggunaan memori berada di 92% dengan hanya 317 MB tersedia dan `page file` 7697 MB. Audio playback tidak terdeteksi di `DxDiag`. Yang membedakan unit ini adalah tambahan temuan operasional: monitor dirasa terlalu kecil, kursor sering menghilang, dan performa mulai menurun saat banyak aplikasi berjalan bersamaan.

**Analisis:** Yohana menunjukkan gangguan yang sifatnya campuran: ada hambatan performa karena RAM 4 GB, tetapi ada juga hambatan ergonomi dan input yang langsung mengganggu alur kerja. Karena belum ada bukti kuat bahwa storage sudah rusak, dan belum ada gejala fatal seperti `BSOD` atau mati mendadak, unit ini masih dapat diposisikan satu tingkat di bawah kategori penggantian segera. Meski demikian, keluhan pengguna sudah cukup nyata untuk membuatnya tidak layak dibiarkan tanpa intervensi.

**Rekomendasi:** Lakukan upgrade RAM sebagai tindakan minimum, periksa perangkat input dan konektivitas monitor, serta verifikasi kesehatan storage dan audio. Masukkan unit ini ke batch penyegaran berikutnya agar pengguna tidak terus bekerja dalam kondisi yang mengganggu.

### 8. Hibab
**Profil singkat:** Laptop HP 240 G6 dengan Intel Core i5-7200U, RAM 4 GB, SSD NVMe 256 GB, Intel HD Graphics 620, dan AMD Radeon R5 M330.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage sehat.

**Temuan utama:** Penggunaan memori mencapai 90% dengan `page file` 7613 MB. SSD masih sehat di angka 94%, sehingga media penyimpanan bukan sumber utama hambatan. Dokumen kualitatif menyebut Outlook lambat, aplikasi produktivitas terasa berat, dan baterai cepat habis, terutama ketika dipakai untuk rapat daring.

**Analisis:** Unit ini masih bisa bekerja, tetapi kualitas pengalaman pakainya sudah menurun nyata. Hambatan utamanya ada pada kombinasi platform mobile yang menua, RAM terlalu kecil, dan baterai yang tidak lagi mendukung mobilitas. Bila peran pengguna mengandalkan rapat daring atau kerja berpindah tempat, unit ini akan semakin cepat terasa tidak memadai.

**Rekomendasi:** Masukkan ke kategori penyegaran prioritas tinggi. Jika organisasi ingin menunda penggantian, lakukan penggantian baterai dan upgrade RAM sebagai langkah sementara. Namun, persiapan penggantian tetap perlu dimulai karena platform dasarnya sudah tua.

### 9. Devinta
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 8 GB, Windows 10 IoT Enterprise LTSC 64-bit, dan SSD NVMe 256 GB yang sehat.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage sehat.

**Temuan utama:** Walaupun kapasitas RAM dua kali lebih besar daripada unit 4 GB, `DxDiag` menunjukkan `page file` sudah mencapai 8837 MB. Ini menandakan bahwa RAM 8 GB pun mulai sempit terhadap pola penggunaan aktual. Storage masih sehat, tetapi audio playback tidak terdeteksi. Tidak ada keluhan operasional yang sangat berat pada dokumen kualitatif, sehingga masalahnya lebih banyak terlihat dari tekanan teknis.

**Analisis:** Devinta adalah contoh unit yang belum “gagal”, tetapi sudah mendekati batas kelayakan produktivitas. Jika dibiarkan tanpa intervensi, unit semacam ini sering berubah dari cukup stabil menjadi lambat secara konsisten dalam waktu yang tidak lama, terutama ketika aplikasi bertambah atau kebutuhan multitugas meningkat. Karena storage masih sehat dan belum ada kerusakan fisik, strategi terbaik bukan penggantian mendadak, melainkan penyegaran terencana.

**Rekomendasi:** Upgrade RAM ke 16 GB dan perbaiki fungsi audio. Unit ini layak masuk batch penyegaran prioritas tinggi agar umur pakai efektifnya bisa diperpanjang tanpa menunggu gangguan operasional berat terlebih dahulu.

### 10. Wulan
**Profil singkat:** Desktop Dell Inspiron 3881 dengan Intel Core i5-10400, RAM 8 GB, SSD NVMe 512 GB, dan driver grafis yang relatif baru.

**Status komponen:** CPU sehat, GPU peringatan, memori peringatan, storage peringatan.

**Temuan utama:** Penggunaan memori berada di 82% dan `page file` 9700 MB. SSD masih memiliki performa 100% dan suhu 30 C, walaupun `health` turun ke 88%. Audio playback tidak terdeteksi. Temuan operasional paling menonjol adalah aplikasi menjadi `Not Responding` setelah proses unduh PDF, yang lebih menyerupai masalah sistem operasi, aplikasi, atau konfigurasi ketimbang kegagalan perangkat keras inti.

**Analisis:** Dibanding banyak unit lain, inti perangkat Wulan masih cukup baik. Prosesor generasi ke-10 masih relevan untuk pekerjaan kantor dasar hingga menengah. Karena itu, akan terlalu agresif bila unit ini langsung dimasukkan ke prioritas penggantian. Yang dibutuhkan terlebih dahulu adalah memastikan integritas sistem operasi, aplikasi, dan konfigurasi. Bila setelah perbaikan gejala masih berulang, barulah opsi penggantian bisa dinaikkan.

**Rekomendasi:** Terapkan strategi perbaikan/upgrade terlebih dahulu. Lakukan pemeriksaan perangkat lunak, pertimbangkan instal ulang sistem operasi, verifikasi audio playback, dan tambah RAM ke 16 GB bila beban multitugas memang tinggi.

### 11. Robin
**Profil singkat:** Desktop Dell Inspiron 3881 dengan Intel Core i5-10400, RAM 8 GB, Windows 11 Home, dan SSD NVMe 512 GB yang sehat.

**Status komponen:** CPU sehat, GPU peringatan, memori peringatan, storage sehat.

**Temuan utama:** Penggunaan memori berada di 81% dengan `page file` 8345 MB. SSD berada di `health` 93% dan suhu 31 C, sehingga masih tergolong sehat. Audio playback tidak terdeteksi pada `DxDiag`, tetapi tidak ada keluhan operasional berarti dari pengguna. Perangkat masih stabil untuk pekerjaan Excel dan input data.

**Analisis:** Robin menunjukkan kondisi yang relatif baik dibanding mayoritas armada. Tekanan memori memang mulai terlihat, tetapi belum disertai keluhan atau kegagalan nyata dalam pekerjaan harian. Ini menandakan bahwa penggantian belum menjadi prioritas anggaran yang paling berdampak saat ini. Namun, jika pola kerja berubah menjadi lebih berat, RAM 8 GB kemungkinan akan cepat menjadi batas berikutnya.

**Rekomendasi:** Pertahankan unit ini dan lakukan pemeliharaan rutin. Audit fungsi audio bila memang diperlukan oleh peran pengguna, serta pertimbangkan upgrade RAM ke 16 GB hanya jika penggunaan aplikasi bertambah atau performa mulai menurun.

### 12. System Autocount
**Profil singkat:** Desktop HP Slim Desktop 290-p0xxx dengan Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB, dan HDD 2 TB yang sehat.

**Status komponen:** CPU peringatan, GPU peringatan, memori peringatan, storage sehat.

**Temuan utama:** Penggunaan memori berada di 74% dengan `page file` 3294 MB. Angka ini menunjukkan RAM 4 GB tetap sempit, tetapi belum menimbulkan tekanan separah unit aktif lain. SSD berada di `health` 93% dan HDD sekunder berada di `health` 100%. Dokumen kualitatif menegaskan bahwa sistem ini masih berjalan baik sebagai unit siaga Autocount, tanpa keluhan operasional berarti.

**Analisis:** Inilah contoh unit yang secara spesifikasi tampak lemah, tetapi secara bisnis masih memadai karena fungsi perannya terbatas dan stabil. Mengganti unit seperti ini sebelum unit yang sudah sering `BSOD`, mati mendadak, atau merusak ritme kerja harian akan menghasilkan prioritas yang tidak efisien.

**Rekomendasi:** Pertahankan unit ini. Upgrade RAM hanya perlu dipertimbangkan jika sistem siaga berubah menjadi sistem aktif atau ada peningkatan beban aplikasi. Verifikasi audio playback dapat dilakukan saat jadwal pemeliharaan berkala.

## Prioritas Penggantian Final
### 1. Penggantian segera
Kategori ini ditempati oleh unit yang sudah memperlihatkan kombinasi kegagalan operasional nyata, keterbatasan teknis berat, dan/atau potensi risiko bisnis tinggi jika terus dipakai.

* System Finance
* Renaldi
* Diana
* Regina
* Syela

Alasan pengelompokan:

* perangkat sudah menghambat pekerjaan inti secara berulang
* ada indikasi `BSOD`, mati mendadak, atau degradasi fisik yang berat
* upgrade parsial berpotensi hanya memperpanjang masalah, bukan menyelesaikannya
* biaya tidak langsung akibat `downtime`, dukungan teknis, dan produktivitas yang hilang sudah mulai lebih besar daripada manfaat menunda penggantian

### 2. Penyegaran prioritas tinggi
Kategori ini menampung unit yang masih dapat dipakai sementara, tetapi sudah tidak lagi ideal untuk mendukung kinerja secara efisien dan andal.

* Christy
* Yohana
* Hibab
* Devinta

Alasan pengelompokan:

* keterbatasan RAM atau platform sudah mulai menekan kerja harian
* masalah periferal, baterai, atau form factor mulai menghambat pekerjaan
* masih ada ruang untuk tindakan transisi, tetapi penundaan terlalu lama akan menurunkan mutu kerja dan menambah beban dukungan

### 3. Perbaikan/upgrade terlebih dahulu
Kategori ini dipakai untuk unit yang inti perangkat kerasnya masih cukup baik dan gejala masalahnya lebih dekat ke isu perangkat lunak atau konfigurasi.

* Wulan

Alasan pengelompokan:

* prosesor dan storage masih cukup memadai
* keluhan operasional lebih cocok ditangani melalui perbaikan sistem
* penggantian langsung belum memberikan nilai tambah setinggi unit lain

### 4. Pertahankan
Kategori ini memuat unit yang masih memenuhi kebutuhan peran saat ini dan belum menimbulkan urgensi bisnis yang cukup kuat untuk penggantian.

* Robin
* System Autocount

Alasan pengelompokan:

* tidak ada keluhan operasional signifikan
* perangkat masih stabil untuk fungsinya masing-masing
* alokasi anggaran akan lebih berdampak bila difokuskan pada unit yang lebih kritis terlebih dahulu

## Rencana Tindakan Manajerial
### Tindakan segera: 0-30 hari
Fokus utama dalam 30 hari pertama adalah menurunkan risiko operasional paling besar sembari menyiapkan keputusan pengadaan.

* setujui batch penggantian pertama untuk System Finance, Renaldi, Diana, Regina, dan Syela
* lakukan `backup` prioritas pada Renaldi dan unit lain yang menunjukkan gejala storage atau kestabilan paling berat
* bersihkan ruang penyimpanan pada Syela dan Renaldi agar unit tidak jatuh ke kondisi gagal pakai sebelum penggantian tersedia
* identifikasi kebutuhan periferal sementara, seperti webcam untuk Renaldi atau solusi audio sementara pada unit yang membutuhkan komunikasi daring

### Tindakan lanjutan: 30-60 hari
Setelah batch pertama berjalan, organisasi perlu beralih ke unit yang masih dapat ditahan sebentar tetapi sudah jelas mengurangi kualitas kerja.

* siapkan batch penyegaran untuk Christy, Yohana, Hibab, dan Devinta
* jalankan strategi perbaikan sistem pada Wulan dan evaluasi ulang performanya setelah intervensi
* tetap pertahankan Robin dan System Autocount dengan pemantauan rutin

### Tindakan konsolidasi: 60-90 hari
Tahap ini bertujuan menstabilkan armada pasca-intervensi dan mencegah munculnya backlog baru.

* lakukan evaluasi ulang terhadap unit yang hanya di-upgrade, terutama Devinta, Yohana, dan Hibab
* pastikan seluruh perangkat pengganti sudah memenuhi kebutuhan periferal sesuai peran pengguna
* dokumentasikan baseline baru agar keputusan pengadaan berikutnya lebih seragam dan tidak kembali ke standar yang terlalu rendah

## Baseline Standar Perangkat 2026
Agar siklus pengadaan berikutnya tidak hanya menyelesaikan masalah jangka pendek, organisasi perlu menetapkan standar minimum yang lebih realistis untuk beban kerja saat ini.

| Komponen | Standar Minimum yang Disarankan | Catatan |
| :--- | :--- | :--- |
| Prosesor | Kelas setara Intel Core i5 generasi baru atau yang setara | Ditujukan untuk pekerjaan kantor aktif, multitugas, dan dukungan aplikasi modern |
| RAM | 16 GB | Menjadi baseline utama agar tidak kembali terjebak pada bottleneck memori |
| Penyimpanan | SSD/NVMe sehat | Untuk unit tertentu dapat dipertimbangkan kapasitas lebih besar sesuai kebutuhan data lokal |
| Sistem operasi | 64-bit dan masih didukung | Penting untuk kompatibilitas, keamanan, dan pemanfaatan memori yang optimal |
| Periferal | Audio, mikrofon, webcam, keyboard, dan baterai berfungsi baik | Kesesuaian periferal harus mengikuti peran pengguna, terutama untuk kerja mobile dan rapat daring |
| Tampilan kerja | Monitor atau layar yang memadai untuk peran | Perlu diperhatikan pada kasus yang terkait ergonomi dan kenyamanan visual |

## Rekomendasi Eksekutif Akhir
Kesimpulan akhir laporan ini dapat dirumuskan secara tegas. Organisasi tidak sedang menghadapi sekadar “beberapa komputer lambat”, tetapi sedang berhadapan dengan armada yang pada sebagian besar unit sudah menua secara struktural dan mulai menimbulkan dampak kerja yang nyata. Lima unit perlu diprioritaskan untuk penggantian segera karena biaya mempertahankannya akan terus meningkat dalam bentuk waktu henti, ketidakstabilan, dan produktivitas yang hilang. Empat unit lain masih dapat ditahan sementara, tetapi tidak layak dibiarkan terlalu lama tanpa penyegaran. Satu unit lebih tepat diperbaiki terlebih dahulu, dan dua unit lainnya masih cukup aman untuk dipertahankan.

Urutan keputusan yang paling rasional saat ini adalah sebagai berikut:

* **Penggantian segera:** System Finance, Renaldi, Diana, Regina, Syela
* **Penyegaran prioritas tinggi:** Christy, Yohana, Hibab, Devinta
* **Perbaikan/upgrade terlebih dahulu:** Wulan
* **Pertahankan:** Robin, System Autocount

Jika pendekatan ini diikuti, organisasi dapat menurunkan risiko operasional dengan cara yang lebih terukur. Penggantian dilakukan pada titik yang benar-benar kritis, penyegaran diarahkan ke unit yang mulai menghambat, dan anggaran tidak dihabiskan untuk unit yang masih stabil. Dengan demikian, program pengelolaan perangkat menjadi lebih efektif, lebih defensibel secara bisnis, dan lebih selaras dengan kebutuhan kerja nyata di lapangan.
