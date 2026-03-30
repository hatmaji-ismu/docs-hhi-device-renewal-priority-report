# Appendices

## Appendix A: Analisis Detail Per Unit

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

**Temuan utama:** Penggunaan memori berada di 85% dengan hanya 583 MB tersedia dan `page file` 5972 MB. SSD masih berada di `health` 85%, tetapi suhu mencapai 61 C dan ruang kosong tersisa 30 GB. Temuan kualitatif jauh lebih serius: perangkat sering `hang`, error ketika membuka lebih dari dua file Excel, lambat saat mengakses ORS Payroll, dan sering mengalami `BSOD` serta mati mendadak.

**Analisis:** Insiden `BSOD` dan mati mendadak menandakan risiko yang melampaui bottleneck RAM biasa. Kemungkinan sumbernya bisa berasal dari catu daya, termal, atau kestabilan sistem yang lebih dalam. Karena unit dipakai untuk pekerjaan administrasi yang menuntut kontinuitas, setiap gangguan seperti ini langsung menambah risiko kehilangan pekerjaan, pengulangan input, dan penurunan kepercayaan pengguna terhadap sistem.

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

**Analisis:** Ketiadaan keluhan kualitatif tidak serta-merta berarti unit aman. Dalam kasus ini, justru bukti teknis menunjukkan perangkat sedang berada pada posisi rawan: RAM sangat terbatas, storage hampir penuh, dan kesehatan disk sudah menurun. Jika dipertahankan terlalu lama, unit ini berpotensi beralih dari "lambat" menjadi "gagal bekerja" tanpa banyak peringatan.

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

**Temuan utama:** Penggunaan memori berada di 92% dengan hanya 317 MB tersedia dan `page file` 7697 MB. Audio playback tidak terdeteksi di `DxDiag`. Yang membedakan unit ini adalah tambahan temuan operasional: monitor dirasa terlalu kecil, kursor sering menghilang, performa mulai menurun saat banyak aplikasi berjalan bersamaan, dan insiden `BSOD` sudah dilaporkan oleh pengguna.

**Analisis:** Yohana menunjukkan gangguan yang sifatnya campuran: ada hambatan performa karena RAM 4 GB, tetapi ada juga hambatan ergonomi dan input yang langsung mengganggu alur kerja. Secara operasional, pengguna melaporkan insiden `BSOD` yang mengindikasikan risiko ketidakstabilan sistem. Meski storage belum menunjukkan bukti kerusakan yang kuat, BSOD tetap menjadi perhatian serius dan memerlukan investigasi. Keluhan pengguna sudah cukup nyata untuk membuatnya tidak layak dibiarkan tanpa intervensi.

**Rekomendasi:** Lakukan upgrade RAM ke 16 GB sebagai tindakan interim, perbaiki atau ganti monitor ke ukuran yang lebih sesuai, investigasi dan tangani insiden BSOD, dan verifikasi masalah input. Siapkan unit ini untuk masuk batch penyegaran prioritas tinggi dengan perhatian khusus pada kestabilan sistem.

### 8. Hibab
**Profil singkat:** Laptop dengan Intel Core i5-7200U, RAM 4 GB.

**Status komponen:** CPU peringatan, GPU peringatan, memori kritis, storage sehat.

**Temuan utama:** Penggunaan memori mencapai 90% dengan `page file` tinggi. Platform mobile sudah generasi lama (7th gen), tetapi SSD masih dalam kondisi sehat. Dari sisi operasional, Outlook berjalan lambat, baterai cepat habis, dan pengalaman rapat daring menurun.

**Analisis:** Unit ini masih dapat dipakai sementara, tetapi mobilitas dan kenyamanan kerja sudah buruk. Platform yang menua dikombinasikan dengan RAM terbatas membuatnya tidak ideal untuk kerja mobile yang membutuhkan daya tahan baterai dan performa responsif.

**Rekomendasi:** Ganti baterai dan tambah RAM jika ingin menunda penggantian lebih lama. Namun, siapkan penggantian laptop business-grade dengan spesifikasi yang sesuai untuk kerja mobile.

### 9. Devinta
**Profil singkat:** Desktop dengan Intel Core i5-8400, RAM 8 GB, SSD sehat.

**Status komponen:** CPU peringatan, GPU peringatan, memori mulai tertekan, storage sehat.

**Temuan utama:** `Page file` sangat tinggi menandakan tekanan multitasking, platform mulai menua (8th gen), dan audio playback tidak terdeteksi. Belum ada keluhan lapangan berat, tetapi bukti teknis menunjukkan sistem sedang bekerja di kapasitas tinggi.

**Analisis:** Risiko penurunan produktivitas muncul dalam jangka menengah. Unit ini masih memiliki fondasi yang cukup baik (SSD sehat, CPU masih capable), tetapi memerlukan intervensi untuk menjaga performa optimal.

**Rekomendasi:** Upgrade RAM ke 16 GB dan perbaiki audio. Masukkan unit ini ke batch penyegaran prioritas tinggi untuk penggantian dalam timeframe menengah.

### 10. Wulan
**Profil singkat:** Desktop dengan Intel Core i5-10400, RAM 8 GB, SSD 88%.

**Status komponen:** CPU masih memadai, RAM mulai sempit, `health` SSD menurun moderat, audio playback tidak terdeteksi.

**Temuan utama:** `Not Responding` setelah mengunduh PDF; gejalanya mengarah ke masalah perangkat lunak atau konfigurasi daripada kegagalan hardware mendasar.

**Analisis:** Replacement belum mendesak. Perbaikan sistem berpotensi menyelesaikan inti masalah tanpa perlu penggantian hardware besar.

**Rekomendasi:** Lakukan perbaikan sistem/instal ulang OS bersih. Upgrade RAM ke 16 GB bila diperlukan. Kategori: perbaikan/upgrade terlebih dahulu.

### 11. Robin
**Profil singkat:** Desktop dengan Intel Core i5-10400, RAM 8 GB, SSD 93%.

**Status komponen:** RAM mulai tertekan, `page file` tinggi, audio playback tidak terdeteksi.

**Temuan utama:** Tidak ada kendala operasional bermakna; stabil untuk Excel dan tugas rutin.

**Analisis:** Belum ada alasan bisnis kuat untuk penggantian langsung. Unit masih memadai untuk kebutuhan saat ini.

**Rekomendasi:** Pertahankan. Lakukan audit audio bila diperlukan dan upgrade RAM bersifat opsional untuk future-proofing.

### 12. System Autocount
**Profil singkat:** Desktop dengan Intel Core i5-8400, RAM 4 GB, SSD + HDD sehat.

**Status komponen:** RAM tetap di bawah standar, tetapi storage sehat dan `page file` masih relatif terkendali.

**Temuan utama:** Sistem siaga Autocount masih berjalan baik, tanpa keluhan lapangan.

**Analisis:** Belum perlu diprioritaskan karena fungsi perannya sebagai sistem siaga masih terpenuhi dengan baik.

**Rekomendasi:** Pertahankan. Upgrade RAM hanya jika beban kerja meningkat di masa depan.

## Appendix B: Dokumen Referensi

### Daftar Dokumen Sumber Lengkap

1. **Laporan Teknis Per Unit (Tersedia di `technical-reports/`):**
   - [System Finance Hardware Report](technical-reports/system-finance.md)
   - [Renaldi Hardware Report](technical-reports/renaldi.md)
   - [Diana Hardware Report](technical-reports/diana.md)
   - [Regina Hardware Report](technical-reports/regina.md)
   - [Syela Hardware Report](technical-reports/syela.md)
   - [Christy Hardware Report](technical-reports/christy.md)
   - [Yohana Hardware Report](technical-reports/yohana.md)
   - [Hibab Hardware Report](technical-reports/hibab.md)
   - [Devinta Hardware Report](technical-reports/devinta.md)
   - [Wulan Hardware Report](technical-reports/wulan.md)
   - [Robin Hardware Report](technical-reports/robin.md)
   - [System Autocount Hardware Report](technical-reports/system-autocount.md)

2. **Dokumen Sumber Asli:**
   - `raw-hardware-assessment-reports/System Finance/System_Finance_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Renaldi/Renaldi_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Diana/Diana_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Regina/Regina_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Syela/Syela_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Christy/Christy_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Yohana/Yohana_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Hibab/Hibab_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Devinta/Devinta_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Wulan/Wulan_Hardware_Report.md`
   - `raw-hardware-assessment-reports/Robin/Robin_Hardware_Report.md`
   - `raw-hardware-assessment-reports/System Autocount/System_Autocount_Hardware_Report.md`

3. **Penilaian Kualitatif Pengguna:**
   - `qualitative-assessment.md`

4. **Dokumen Sintesis:**
   - `stag-report-drafts/comprehensive-report-v0.4.md` (dokumen utama yang menjadi dasar laporan ini)

### Metodologi Assessment

Proses assessment mengikuti alur kerja berikut:

1. **Data Collection:** Pengumpulan bukti teknis dari DxDiag, system reports, dan hardware inspection
2. **User Feedback:** Dokumentasi pengalaman operasional dan keluhan pengguna
3. **Correlation Analysis:** Penyelarasan temuan teknis dengan pengalaman operasional
4. **Risk Assessment:** Evaluasi risiko berdasarkan kombinasi faktor teknis dan bisnis
5. **Priority Classification:** Kategorisasi berdasarkan kriteria yang telah ditetapkan
6. **Recommendation Development:** Penyusunan rekomendasi tindakan spesifik

### Definisi Istilah Teknis

- **BSOD (Blue Screen of Death):** Crash sistem Windows yang menampilkan layar biru dengan kode error
- **Page File:** Virtual memory di hard drive/SSD yang digunakan ketika RAM fisik penuh
- **SSD Health:** Persentase kesehatan solid-state drive berdasarkan wear level, bad sectors, dll.
- **Reserved Spare Area:** Area cadangan pada SSD yang digunakan ketika sector normal mulai rusak
- **DxDiag:** Diagnostic tool Windows untuk menampilkan informasi sistem dan driver
- **Unexpected Shutdown:** Mati mendadak tanpa proses shutdown normal
- **Lag/Freeze:** Kelambatan respons atau pembekuan sistem/aplikasi

### Asumsi dan Batasan

1. **Data Availability:** Analisis dibatasi oleh bukti yang tersedia dalam dokumen sumber
2. **Time Scope:** Kondisi yang dilaporkan merepresentasikan snapshot pada waktu assessment
3. **Methodology:** Pendekatan kualitatif berdasarkan bukti, bukan skor numerik HHI
4. **Validation:** Untuk komponen yang belum tervalidasi lengkap, rekomendasi menggunakan prinsip kehati-hatian
5. **Context:** Rekomendasi disusun dengan mempertimbangkan konteks organisasi dan resources yang tersedia

## Appendix C: Template untuk Future Assessments

### Hardware Assessment Template

```
# [Nama Unit] - Hardware Assessment Report

## Basic Information
- **User:** [Nama Pengguna]
- **Department:** [Departemen]
- **Device Type:** [Desktop/Laptop]
- **Assessment Date:** [Tanggal]

## Technical Specifications
- **Processor:** [Model, Generation]
- **Memory:** [Capacity, Type]
- **Storage:** [Type, Capacity, Health %]
- **Graphics:** [Integrated/Discrete, Model]
- **Operating System:** [Version, Architecture]

## System Performance Metrics
- **RAM Utilization:** [% used / available]
- **Page File Usage:** [Size in MB/GB]
- **Storage Health:** [% health, temperature, free space]
- **System Stability:** [BSOD incidents, unexpected shutdowns]

## Operational Findings
- **User Complaints:** [List of issues reported]
- **Application Performance:** [Specific apps with issues]
- **Physical Condition:** [Damage, wear and tear]
- **Peripheral Status:** [Keyboard, mouse, monitor, audio, etc.]

## Assessment Summary
- **Overall Condition:** [Healthy/Moderate/Critical]
- **Key Issues:** [Main problems identified]
- **Risk Level:** [Low/Medium/High]
- **Recommendation:** [Replace/Upgrade/Maintain]

## Action Plan
- **Immediate Actions:** [Steps to take now]
- **Short-term Plan:** [Next 1-3 months]
- **Long-term Recommendation:** [Future replacement/upgrade]
```

### Qualitative Assessment Template

```
# Qualitative User Assessment

## User Information
- **Name:** [Nama]
- **Role:** [Posisi]
- **Primary Applications:** [Aplikasi utama yang digunakan]

## Work Experience
- **Daily Workflow:** [Deskripsi alur kerja harian]
- **Performance Issues:** [Keluhan kinerja spesifik]
- **Stability Problems:** [Crash, freeze, BSOD]
- **Application-specific Issues:** [Masalah dengan aplikasi tertentu]

## Physical and Ergonomic
- **Device Condition:** [Kerusakan fisik, wear and tear]
- **Peripheral Issues:** [Keyboard, mouse, monitor, audio]
- **Mobility Needs:** [Kebutuhan mobilitas untuk laptop]
- **Ergonomics:** [Kenyamanan penggunaan]

## Future Needs
- **Workload Changes:** [Perubahan beban kerja yang diantisipasi]
- **Application Requirements:** [Kebutuhan aplikasi baru]
- **Form Factor Preferences:** [Preferensi ukuran/tipe perangkat]
- **Additional Requirements:** [Kebutuhan spesifik lainnya]

## Overall Satisfaction
- **Current Device Rating:** [1-10 scale]
- **Willingness to Continue Using:** [Yes/No/With improvements]
- **Priority for Replacement:** [Low/Medium/High/Urgent]
```

## Appendix D: Glossary of Terms

**Business Impact:** Dampak gangguan perangkat terhadap operasi bisnis, produktivitas, dan revenue.

**Critical Assets:** Perangkat dengan risiko tinggi terhadap kontinuitas bisnis jika mengalami kegagalan.

**Device Health Index (HHI):** Metrik untuk menilai kondisi kesehatan perangkat (konseptual dalam konteks ini).

**Downtime:** Waktu ketika sistem atau perangkat tidak tersedia untuk digunakan.

**Lifecycle Management:** Pendekatan terstruktur untuk mengelola aset TI dari procurement hingga disposal.

**Phased Renewal:** Strategi penggantian perangkat secara bertahap dalam beberapa batch.

**Preventive Maintenance:** Pemeliharaan rutin untuk mencegah kegagalan sebelum terjadi.

**ROI (Return on Investment):** Pengembalian investasi dari program peremajaan perangkat.

**Total Cost of Ownership (TCO):** Biaya total memiliki dan mengoperasikan perangkat selama lifecycle-nya.

**User Productivity:** Kemampuan pengguna untuk menyelesaikan tugas secara efisien dengan perangkat yang diberikan.

---

*Lampiran ini melengkapi laporan utama dengan detail analisis per unit, referensi dokumen, template untuk assessment masa depan, dan glosarium istilah. Semua informasi dalam lampiran didasarkan pada data yang tersedia dari dokumen sumber.*