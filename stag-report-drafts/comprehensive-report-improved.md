# Laporan Prioritas Peremajaan Perangkat HHI

**Versi:** 2.0 (improved)  
**Tanggal dokumen:** 27 Maret 2026  
**Sumber utama:** `comprehensive-report.md`  
**Tujuan:** Menyediakan dokumen yang lebih ringkas, konsisten, dan siap dipakai sebagai dasar pengambilan keputusan manajerial untuk penggantian, penyegaran, atau pemeliharaan perangkat kerja.

---

## Daftar Isi
1. [Ringkasan Eksekutif](#ringkasan-eksekutif)
2. [Tujuan dan Ruang Lingkup](#tujuan-dan-ruang-lingkup)
3. [Metodologi Penilaian](#metodologi-penilaian)
4. [Kriteria Klasifikasi Prioritas](#kriteria-klasifikasi-prioritas)
5. [Ringkasan Prioritas Armada](#ringkasan-prioritas-armada)
6. [Temuan Lintas Armada](#temuan-lintas-armada)
7. [Analisis dan Rekomendasi Per Unit](#analisis-dan-rekomendasi-per-unit)
8. [Rencana Tindakan Manajerial](#rencana-tindakan-manajerial)
9. [Baseline Standar Perangkat 2026](#baseline-standar-perangkat-2026)
10. [Asumsi, Keterbatasan, dan Catatan Validasi](#asumsi-keterbatasan-dan-catatan-validasi)
11. [Kesimpulan Akhir](#kesimpulan-akhir)
12. [Lampiran A — Ringkasan Data Sumber](#lampiran-a--ringkasan-data-sumber)

---

## Ringkasan Eksekutif

Laporan ini merupakan versi yang telah dirapikan dari dokumen assessment perangkat keras HHI yang mencakup **12 unit perangkat** dan **1 dokumen penilaian kualitatif pengguna**. Fokus utama laporan adalah mengubah data teknis menjadi keputusan yang dapat langsung digunakan untuk **penganggaran, prioritisasi procurement, dan mitigasi risiko operasional**.

Secara umum, kondisi armada menunjukkan bahwa masalah utama bukan hanya usia perangkat, melainkan kombinasi antara:
- keterbatasan RAM (terutama **4 GB**),
- penurunan kesehatan storage pada sebagian unit,
- gangguan kestabilan seperti **freeze**, **BSOD**, dan **mati mendadak**,
- kerusakan fisik/periferal,
- serta ketidaksesuaian perangkat dengan kebutuhan kerja aktual pengguna.

### Distribusi Prioritas Armada

| Kategori | Jumlah Unit | Persentase | Makna Operasional |
|---|---:|---:|---|
| **[SEGERA GANTI]** | 5 | 41,7% | Risiko produktivitas dan stabilitas sudah tinggi; perbaikan parsial tidak lagi ekonomis sebagai solusi utama |
| **[PENYEGARAN PRIORITAS TINGGI]** | 4 | 33,3% | Masih dapat dipakai sementara, tetapi sudah konsisten menekan mutu kerja dan perlu masuk batch berikutnya |
| **[PERBAIKAN/UPGRADE TERLEBIH DAHULU]** | 1 | 8,3% | Inti perangkat masih cukup baik; gejala dominan mengarah ke isu software, konfigurasi, atau bottleneck yang masih bisa diperbaiki |
| **[TETAP GUNAKAN]** | 2 | 16,7% | Unit masih stabil untuk peran saat ini; cukup dipelihara dan dipantau |

### Kesimpulan Manajerial Utama

1. **Program penggantian batch pertama perlu segera dijalankan** untuk lima unit berisiko tertinggi: **System Finance, Renaldi, Diana, Regina, dan Syela**.
2. **Empat unit** berikutnya layak masuk **batch penyegaran**: **Christy, Yohana, Hibab, dan Devinta**.
3. **Wulan** sebaiknya **diperbaiki/di-upgrade terlebih dahulu** sebelum dipertimbangkan untuk replacement.
4. **Robin** dan **System Autocount** masih dapat **dipertahankan** dengan monitoring rutin.
5. Standar minimum perangkat kerja aktif ke depan perlu dinaikkan ke **RAM 16 GB**, **OS 64-bit**, dan **SSD sehat** sebagai baseline baru.

---

## Tujuan dan Ruang Lingkup

### Tujuan
Laporan ini disusun untuk menjawab tiga kebutuhan organisasi secara simultan:
1. Memetakan kondisi teknis dan operasional perangkat yang sedang digunakan.
2. Menentukan prioritas tindakan: **ganti**, **refresh**, **upgrade/perbaikan**, atau **pertahankan**.
3. Menyediakan dasar keputusan pengadaan yang dapat dipertanggungjawabkan secara operasional dan bisnis.

### Ruang Lingkup Unit yang Dinilai
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

### Dokumen Sumber
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
- `qualitative-assessment.md`

---

## Metodologi Penilaian

Penentuan prioritas pada laporan ini tidak hanya berdasarkan usia perangkat. Setiap unit dianalisis melalui **dua lapis bukti**:

### 1) Bukti Teknis
Aspek yang dianalisis:
- kelas dan generasi prosesor,
- kapasitas RAM dan tingkat utilisasinya,
- penggunaan `page file` sebagai indikator tekanan memori,
- kesehatan storage, suhu, dan sisa ruang kosong,
- status driver penting,
- kondisi audio, GPU, dan komponen pendukung lainnya,
- relevansi arsitektur OS terhadap perangkat.

### 2) Bukti Operasional
Aspek yang dianalisis:
- keluhan `lag`, `freeze`, `not responding`, `BSOD`, atau mati mendadak,
- hambatan kerja pada Excel, Outlook, browser, payroll, meeting online, dan aplikasi harian lain,
- kerusakan fisik seperti layar, chassis, keyboard, engsel, atau baterai,
- gangguan periferal seperti audio, mikrofon, webcam, mouse, dan monitor,
- konteks penggunaan (aktif harian vs standby/siaga).

### Prinsip Analisis
Laporan ini menggunakan prinsip berikut:
- **Produktivitas nyata** lebih penting daripada sekadar “perangkat masih menyala”.
- **Perbaikan parsial** hanya direkomendasikan bila masih ekonomis dan masih memberikan manfaat operasional yang masuk akal.
- **Konteks pengguna** memengaruhi urgensi; perangkat yang tampak “cukup” di atas kertas bisa menjadi prioritas tinggi bila sudah mengganggu pekerjaan harian.
- **Kehati-hatian** diterapkan bila bukti health storage atau kondisi komponen belum lengkap.

---

## Kriteria Klasifikasi Prioritas

Agar konsisten, klasifikasi pada dokumen ini distandarkan sebagai berikut:

### **[SEGERA GANTI]**
Digunakan bila unit menunjukkan satu atau lebih kondisi berikut:
- gangguan kerja nyata dan berulang,
- risiko stabilitas tinggi (`BSOD`, mati mendadak, gagal boot, freeze berat),
- kerusakan fisik serius,
- storage atau platform inti sudah berada pada kondisi yang tidak ekonomis untuk dipertahankan,
- upgrade parsial hanya akan menunda masalah, bukan menyelesaikannya.

### **[PENYEGARAN PRIORITAS TINGGI]**
Digunakan bila unit:
- masih dapat dipakai dalam jangka pendek,
- namun sudah menekan mutu kerja, keandalan, atau mobilitas,
- dan layak masuk batch procurement berikutnya.

### **[PERBAIKAN/UPGRADE TERLEBIH DAHULU]**
Digunakan bila:
- CPU dan storage inti masih memadai,
- gejala lebih dekat ke masalah software, konfigurasi, atau bottleneck yang masih dapat diatasi,
- upgrade (misalnya RAM) berpotensi memperpanjang umur pakai secara rasional.

### **[TETAP GUNAKAN]**
Digunakan bila:
- perangkat masih stabil untuk fungsi bisnis saat ini,
- tidak ada keluhan operasional signifikan,
- dan alokasi anggaran akan lebih berdampak jika difokuskan ke unit lain yang lebih kritis.

---

## Ringkasan Prioritas Armada

| Unit | Profil Singkat | Temuan Kunci | Dampak Bisnis | Rekomendasi | Prioritas |
|---|---|---|---|---|---|
| **System Finance** | i3-4160, RAM 4 GB, Windows 10 32-bit, HDD | Platform sangat tua, RAM efektif rendah, OS 32-bit, audio playback tidak terdeteksi | Produktivitas dasar terganggu; tidak sejalan dengan kebutuhan kerja modern | Ganti unit; retrofit besar tidak ekonomis | **[SEGERA GANTI]** |
| **Renaldi** | i5-8400, RAM 4 GB, SSD warning | RAM kritis, SSD 85%, suhu 66°C, reserved spare area terpakai, `BSOD`, tidak ada webcam | Risiko kehilangan data, downtime, dan gangguan kerja tinggi | Ganti unit dan backup data segera | **[SEGERA GANTI]** |
| **Diana** | i5-8400, RAM 4 GB, SSD panas | RAM kritis, `page file` tinggi, SSD 85% pada 61°C, sering `hang`, mati mendadak | Gangguan langsung pada pekerjaan administrasi | Ganti unit; jangan hanya upgrade RAM | **[SEGERA GANTI]** |
| **Regina** | i5-8265U, RAM 4 GB, laptop | RAM 92%, `page file` sangat tinggi, SSD 75%, `BSOD`, chassis patah, baterai drop ekstrem | Tidak andal untuk kerja rutin maupun mobile | Ganti unit sesegera mungkin | **[SEGERA GANTI]** |
| **Syela** | i5-8400, RAM 4 GB, SSD 78% | RAM kritis, ruang kosong 5,6 GB, suhu 54°C, wear storage meningkat | Risiko instabilitas dan penurunan performa tinggi | Ganti unit; bersihkan storage sebagai mitigasi sementara | **[SEGERA GANTI]** |
| **Christy** | i5-10210U, RAM 8 GB, laptop | RAM 89%, storage sehat, mikrofon rusak, keyboard rusak, kebutuhan kapasitas lebih besar | Perangkat sudah tidak cocok dengan kebutuhan peran pengguna | Siapkan laptop pengganti yang lebih sesuai | **[PENYEGARAN PRIORITAS TINGGI]** |
| **Yohana** | i5-8400, RAM 4 GB, SSD 256 GB | RAM 92%, `page file` tinggi, audio playback tidak terdeteksi, bukti health storage belum lengkap, isu monitor & input | Produktivitas terganggu tetapi belum ada bukti failure total | Upgrade RAM, perbaiki input/monitor, siapkan refresh batch berikutnya | **[PENYEGARAN PRIORITAS TINGGI]** |
| **Hibab** | i5-7200U, RAM 4 GB, laptop | RAM 90%, storage sehat, Outlook lambat, baterai cepat habis | Masih usable, tetapi mobilitas dan kenyamanan kerja menurun | Ganti baterai + tambah RAM bila menunda; siapkan refresh | **[PENYEGARAN PRIORITAS TINGGI]** |
| **Devinta** | i5-8400, RAM 8 GB, SSD sehat | `page file` sangat tinggi, platform mulai menua, audio playback tidak terdeteksi | Risiko penurunan produktivitas jangka menengah | Upgrade RAM ke 16 GB dan perbaiki audio | **[PENYEGARAN PRIORITAS TINGGI]** |
| **Wulan** | i5-10400, RAM 8 GB, SSD 88% | CPU masih layak, gejala `Not Responding` cenderung software-related, audio playback tidak terdeteksi | Replacement belum paling mendesak | Perbaikan sistem/instal ulang OS, evaluasi ulang, upgrade RAM bila perlu | **[PERBAIKAN/UPGRADE TERLEBIH DAHULU]** |
| **Robin** | i5-10400, RAM 8 GB, SSD 93% | Stabil untuk kerja harian; tekanan RAM mulai terlihat | Belum ada alasan bisnis kuat untuk replacement | Pertahankan; upgrade RAM opsional | **[TETAP GUNAKAN]** |
| **System Autocount** | i5-8400, RAM 4 GB, SSD + HDD sehat | RAM di bawah standar, tetapi fungsi standby masih stabil | Peran bisnis masih terpenuhi | Pertahankan; upgrade RAM hanya jika beban meningkat | **[TETAP GUNAKAN]** |

---

## Temuan Lintas Armada

### 1) RAM 4 GB sudah tidak layak sebagai baseline kerja aktif
Temuan paling konsisten adalah bottleneck memori. Sebagian besar unit 4 GB menunjukkan pola yang sama:
- utilisasi memori sangat tinggi,
- `page file` besar,
- penurunan responsivitas saat multitasking,
- keluhan lambat pada Excel, Outlook, browser, dan aplikasi kerja lain.

**Implikasi:** organisasi perlu menetapkan **16 GB** sebagai baseline baru untuk perangkat kerja aktif.

### 2) Tidak semua perangkat tua harus dipukul rata
Ada unit lama yang memang perlu diganti segera, tetapi ada juga yang masih layak dipertahankan karena perannya terbatas atau hanya sebagai sistem standby.

**Implikasi:** keputusan procurement harus berbasis **fungsi bisnis aktual**, bukan sekadar usia atau spesifikasi mentah.

### 3) Gejala operasional mengubah prioritas secara signifikan
Kasus `BSOD`, mati mendadak, battery drain ekstrem, dan kerusakan fisik memiliki bobot prioritas tinggi karena berdampak langsung pada continuity of work.

**Contoh:**
- **Renaldi** dan **Regina** bukan sekadar lambat; keduanya sudah menunjukkan gejala stabilitas berat.
- **Diana** menghadapi mati mendadak, yang memperbesar risiko kehilangan pekerjaan yang belum tersimpan.

### 4) Risiko storage bersifat selektif
Tidak semua unit memiliki masalah storage. Risiko tertinggi terlihat pada:
- **Renaldi** (reserved spare area sudah terpakai, suhu tinggi, ruang kosong rendah),
- **Syela** (wear meningkat dan storage hampir penuh),
- **Regina** (health SSD 75%).

Sementara itu, beberapa unit lain masih memiliki storage yang cukup sehat sehingga investasi tidak perlu diarahkan ke penggantian disk terlebih dahulu.

### 5) Periferal dan kerusakan fisik sama pentingnya dengan CPU/RAM
Kualitas kerja juga ditentukan oleh:
- kondisi keyboard,
- mikrofon,
- webcam,
- monitor,
- mouse/input,
- baterai,
- chassis,
- dan audio playback.

Artinya, evaluasi kelayakan perangkat harus selalu melihat **experience of use**, bukan hanya compute performance.

---

## Analisis dan Rekomendasi Per Unit

### 1. System Finance
**Profil singkat**  
Desktop dengan Intel Core i3-4160, RAM 4 GB, Windows 10 Pro 32-bit, Intel HD Graphics 4400, dan HDD 500 GB.

**Diagnosis**  
Unit ini menghadapi masalah struktural: platform lama, OS 32-bit, RAM efektif rendah, driver tua, dan performa yang tertinggal. Walaupun HDD masih sehat, kombinasi CPU lama + RAM 4 GB + OS 32-bit menjadikan perangkat ini tidak lagi rasional untuk menopang pekerjaan modern.

**Rekomendasi**  
**[SEGERA GANTI]**  
Jika replacement belum tersedia, batasi hanya untuk kebutuhan sangat ringan. Upgrade parsial (OS 64-bit, RAM, SSD) secara teknis mungkin dilakukan, tetapi kurang ekonomis dibanding penggantian unit baru.

---

### 2. Renaldi
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB.

**Diagnosis**  
Unit ini memiliki kombinasi risiko paling berat: RAM sangat terbatas, SSD sudah menampilkan warning kesehatan, suhu storage tinggi, ruang kosong sempit, ada gejala `freeze`, `lag`, dan `BSOD`, serta kebutuhan meeting terkendala webcam.

**Rekomendasi**  
**[SEGERA GANTI]**  
Lakukan **backup data segera**. Tindakan sementara hanya bersifat mitigasi singkat (pembersihan drive, perbaikan airflow, dan solusi meeting sementara).

---

### 3. Diana
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB.

**Diagnosis**  
Masalah utama tidak hanya pada bottleneck RAM, tetapi juga gejala **mati mendadak** dan **hang** saat pekerjaan administratif berjalan. Hal ini mengindikasikan risiko stabilitas sistem yang lebih serius daripada sekadar keterbatasan memori.

**Rekomendasi**  
**[SEGERA GANTI]**  
Upgrade RAM saja tidak memadai. Selama masa transisi, cek pendinginan, startup apps, dan biasakan autosave/penyimpanan berkala.

---

### 4. Regina
**Profil singkat**  
Laptop HP 240 G7, Intel Core i5-8265U, RAM 4 GB, SSD NVMe 256 GB.

**Diagnosis**  
Unit ini sudah tidak andal secara teknis maupun fisik. Gejalanya mencakup RAM sangat tertekan, `page file` ekstrem, `BSOD`, chassis patah, dan baterai yang turun drastis dalam waktu singkat. Ini bukan lagi isu tuning, melainkan isu kelayakan perangkat.

**Rekomendasi**  
**[SEGERA GANTI]**  
Prioritaskan pemindahan data dan pengamanan pekerjaan pengguna ke perangkat pengganti.

---

### 5. Syela
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB.

**Diagnosis**  
Walaupun tidak ada keluhan kualitatif paling berat, bukti teknis sudah cukup untuk menempatkan unit ini pada risiko tinggi: RAM sempit, SSD nyaris penuh, health menurun, suhu meningkat, dan monitoring disarankan terus-menerus.

**Rekomendasi**  
**[SEGERA GANTI]**  
Sebelum replacement tiba, lakukan pembersihan storage dan kurangi beban background agar unit tidak jatuh ke kondisi gagal pakai.

---

### 6. Christy
**Profil singkat**  
Laptop ASUS VivoBook X412FLC, Intel Core i5-10210U, RAM 8 GB, SSD NVMe 256 GB, HDD 1 TB.

**Diagnosis**  
Storage masih sehat, tetapi perangkat sudah tidak lagi sesuai dengan kebutuhan peran pengguna. Masalah mikrofon, keyboard, kebutuhan storage yang lebih besar, dan kebutuhan form factor yang lebih ringkas membuat opsi replacement lebih masuk akal daripada sekadar repair parsial.

**Rekomendasi**  
**[PENYEGARAN PRIORITAS TINGGI]**  
Arahkan penggantian ke laptop ringkas dengan **RAM 16 GB** dan kapasitas storage yang sesuai kebutuhan kerja.

---

### 7. Yohana
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 4 GB, SSD 256 GB.

**Diagnosis**  
Unit ini menunjukkan campuran masalah performa dan ergonomi: RAM sangat terbatas, `page file` tinggi, audio playback tidak terdeteksi, isu monitor terlalu kecil, dan gangguan input/kursor. Karena bukti health storage belum lengkap dan belum ada gejala failure total, unit ini belum naik ke kategori paling kritis.

**Rekomendasi**  
**[PENYEGARAN PRIORITAS TINGGI]**  
Naikkan RAM sebagai tindakan minimum, perbaiki input/monitor, dan lengkapi validasi storage. Masukkan ke batch penyegaran berikutnya.

---

### 8. Hibab
**Profil singkat**  
Laptop HP 240 G6, Intel Core i5-7200U, RAM 4 GB, SSD NVMe 256 GB.

**Diagnosis**  
Storage masih sehat, tetapi laptop sudah menua dan RAM 4 GB tidak lagi memadai. Keluhan Outlook lambat, aplikasi terasa berat, dan baterai cepat habis membuat perangkat ini masih bisa bekerja, namun kualitas penggunaannya sudah menurun nyata.

**Rekomendasi**  
**[PENYEGARAN PRIORITAS TINGGI]**  
Jika replacement belum bisa dilakukan, ganti baterai dan tambahkan RAM sebagai langkah transisi.

---

### 9. Devinta
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 8 GB, Windows 10 IoT Enterprise LTSC, SSD NVMe 256 GB.

**Diagnosis**  
Unit ini belum menunjukkan failure berat, tetapi `page file` yang sangat tinggi membuktikan bahwa RAM 8 GB sudah mulai sempit terhadap pola kerja aktual. Storage masih sehat, sehingga tindakan terbaik bukan replacement mendadak, melainkan refresh terencana.

**Rekomendasi**  
**[PENYEGARAN PRIORITAS TINGGI]**  
Upgrade RAM ke **16 GB** dan verifikasi/perbaiki audio playback.

---

### 10. Wulan
**Profil singkat**  
Desktop Dell Inspiron 3881, Intel Core i5-10400, RAM 8 GB, SSD NVMe 512 GB.

**Diagnosis**  
CPU masih memadai dan storage belum menunjukkan risiko mendesak. Gejala utama berupa `Not Responding` setelah aktivitas tertentu lebih mengarah ke isu software, konfigurasi, atau integritas OS, bukan failure hardware inti.

**Rekomendasi**  
**[PERBAIKAN/UPGRADE TERLEBIH DAHULU]**  
Lakukan troubleshooting software, pertimbangkan instal ulang OS, verifikasi audio, dan evaluasi kebutuhan upgrade RAM ke **16 GB**.

---

### 11. Robin
**Profil singkat**  
Desktop Dell Inspiron 3881, Intel Core i5-10400, RAM 8 GB, Windows 11 Home, SSD NVMe 512 GB.

**Diagnosis**  
Dibanding mayoritas armada, unit ini berada pada kondisi yang relatif baik. Bottleneck RAM mulai muncul, tetapi belum diikuti keluhan lapangan yang signifikan. Storage juga masih sehat.

**Rekomendasi**  
**[TETAP GUNAKAN]**  
Lanjutkan pemeliharaan rutin. Upgrade RAM ke **16 GB** bersifat opsional bila pola kerja makin berat.

---

### 12. System Autocount
**Profil singkat**  
Desktop HP Slim Desktop 290-p0xxx, Intel Core i5-8400, RAM 4 GB, SSD NVMe 256 GB, HDD 2 TB.

**Diagnosis**  
Meskipun spesifikasinya terbatas, unit ini masih berfungsi baik sebagai **sistem standby**. Dalam konteks bisnis, status perannya membuat replacement belum menjadi prioritas dibanding unit lain yang lebih kritis.

**Rekomendasi**  
**[TETAP GUNAKAN]**  
Pertahankan unit ini. Upgrade RAM hanya bila beban kerja berubah atau sistem siaga beralih menjadi sistem aktif.

---

## Rencana Tindakan Manajerial

### Horizon 0–30 Hari
Fokus utama adalah menurunkan risiko terbesar sambil menyiapkan pengadaan.

**Tindakan:**
- Setujui batch replacement pertama untuk: **System Finance, Renaldi, Diana, Regina, Syela**.
- Lakukan **backup prioritas** untuk unit dengan indikasi storage/stabilitas paling berat, terutama **Renaldi**.
- Kosongkan ruang storage pada **Syela** dan **Renaldi** agar unit tetap bertahan selama masa transisi.
- Sediakan solusi periferal sementara bila dibutuhkan (misalnya webcam, audio, keyboard eksternal).

### Horizon 30–60 Hari
Fokus pada unit yang masih dapat bertahan sementara tetapi sudah jelas menekan kualitas kerja.

**Tindakan:**
- Jalankan batch penyegaran untuk: **Christy, Yohana, Hibab, Devinta**.
- Eksekusi strategi perbaikan sistem pada **Wulan** dan lakukan evaluasi ulang pasca intervensi.
- Pertahankan **Robin** dan **System Autocount** dengan monitoring berkala.

### Horizon 60–90 Hari
Fokus pada stabilisasi armada pasca intervensi.

**Tindakan:**
- Review kembali unit yang hanya di-upgrade (terutama **Devinta, Yohana, Hibab**).
- Pastikan perangkat pengganti memenuhi kebutuhan periferal sesuai peran pengguna.
- Dokumentasikan baseline baru pengadaan agar keputusan berikutnya lebih seragam dan tidak kembali ke standar terlalu rendah.

---

## Baseline Standar Perangkat 2026

Agar siklus pengadaan berikutnya tidak hanya menyelesaikan masalah jangka pendek, organisasi perlu menetapkan baseline minimum berikut untuk perangkat kerja aktif.

| Komponen | Standar Minimum yang Disarankan | Catatan |
|---|---|---|
| **Prosesor** | Kelas setara Intel Core i5 generasi lebih baru atau setara | Memadai untuk pekerjaan kantor aktif dan multitasking |
| **RAM** | **16 GB** | Baseline utama agar tidak kembali terjebak pada bottleneck memori |
| **Penyimpanan** | SSD/NVMe sehat | Kapasitas disesuaikan dengan kebutuhan data lokal pengguna |
| **Sistem Operasi** | 64-bit dan masih didukung | Penting untuk keamanan, kompatibilitas, dan pemanfaatan memori |
| **Periferal** | Audio, mic, webcam, keyboard, baterai berfungsi baik | Wajib disesuaikan dengan peran pengguna |
| **Tampilan** | Monitor/layar yang memadai | Penting untuk ergonomi dan kenyamanan visual |

### Baseline Berdasarkan Jenis Pengguna (opsional untuk procurement)
- **Staf administrasi/office umum:** i5 setara, 16 GB RAM, SSD 512 GB, webcam/mic standar.
- **Pengguna mobile/laptop:** 16 GB RAM, SSD 512 GB–1 TB, baterai sehat, bobot ringan, keyboard dan audio yang andal.
- **Sistem standby/khusus:** dapat menggunakan spek lebih rendah selama stabil, aman, dan role-nya memang terbatas.

---

## Asumsi, Keterbatasan, dan Catatan Validasi

### Asumsi
- Analisis ini mengikuti bukti yang tersedia pada folder assessment.
- Keputusan replacement mempertimbangkan produktivitas, kestabilan, dan kelayakan operasional — bukan semata usia perangkat.

### Keterbatasan
- Tidak semua unit memiliki bukti health storage yang lengkap.
- Tidak semua masalah audio/periferal dapat dipastikan sebagai kerusakan hardware; sebagian bisa berupa issue driver, device detection, atau konfigurasi.
- Dokumen ini tidak memasukkan estimasi biaya procurement karena data harga/paket pengadaan belum tersedia.

### Catatan Validasi Penting
- **Yohana:** health storage belum tervalidasi penuh karena bukti visual S.M.A.R.T./health tidak tersedia.
- Beberapa unit melaporkan **audio playback tidak terdeteksi** di `DxDiag`; temuan ini perlu diverifikasi ulang secara fisik dan pada level driver/device manager.
- Pada **Christy**, storage masih sehat sehingga replacement lebih dipengaruhi oleh kesesuaian perangkat terhadap kebutuhan pengguna daripada failure storage.

---

## Kesimpulan Akhir

Organisasi saat ini tidak hanya menghadapi beberapa komputer yang lambat, tetapi sebuah armada yang pada sebagian besar unit sudah mulai menua secara struktural dan menimbulkan hambatan kerja nyata.

### Prioritas Final

#### **[SEGERA GANTI]**
- System Finance
- Renaldi
- Diana
- Regina
- Syela

#### **[PENYEGARAN PRIORITAS TINGGI]**
- Christy
- Yohana
- Hibab
- Devinta

#### **[PERBAIKAN/UPGRADE TERLEBIH DAHULU]**
- Wulan

#### **[TETAP GUNAKAN]**
- Robin
- System Autocount

### Pernyataan Eksekutif
Urutan keputusan yang paling rasional adalah:
1. Ganti lebih dulu unit yang sudah menimbulkan **downtime, instabilitas, atau risiko failure tinggi**.
2. Segarkan unit yang masih bisa dipakai sementara tetapi sudah **menekan produktivitas**.
3. Hindari penggunaan anggaran pada unit yang masih stabil bila ada unit lain yang lebih kritis.
4. Jadikan **16 GB RAM + SSD sehat + OS 64-bit** sebagai baseline baru agar masalah yang sama tidak berulang pada siklus berikutnya.

Dengan pendekatan ini, organisasi dapat menurunkan risiko operasional secara terukur, mengarahkan anggaran ke titik yang paling berdampak, dan menjaga kesinambungan kerja dengan keputusan yang lebih defensible secara teknis maupun bisnis.

---

## Lampiran A — Ringkasan Data Sumber

### Daftar Unit per Kategori

**Kategori [SEGERA GANTI]**
- System Finance
- Renaldi
- Diana
- Regina
- Syela

**Kategori [PENYEGARAN PRIORITAS TINGGI]**
- Christy
- Yohana
- Hibab
- Devinta

**Kategori [PERBAIKAN/UPGRADE TERLEBIH DAHULU]**
- Wulan

**Kategori [TETAP GUNAKAN]**
- Robin
- System Autocount

### Ringkasan Temuan Dominan Armada
- Mayoritas bottleneck berasal dari **RAM 4 GB**.
- Beberapa unit menunjukkan gejala stabilitas berat: `BSOD`, `freeze`, `hang`, mati mendadak.
- Risiko storage paling menonjol terdapat pada **Renaldi**, **Syela**, dan **Regina**.
- Kerusakan periferal/fisik menonjol pada **Christy**, **Regina**, **Hibab**, dan beberapa kasus input/audio lainnya.
- Tidak semua perangkat lama harus diganti; beberapa masih layak dipertahankan berdasarkan fungsi bisnis aktual.

---

## Catatan Perbaikan Dokumen dari Versi Sebelumnya

Perbaikan yang diterapkan pada versi ini:
1. **Struktur diperjelas** menjadi format eksekutif yang lebih mudah dibaca manajemen.
2. **Terminologi distandarkan** agar kategori keputusan konsisten di seluruh dokumen.
3. **Duplikasi konten dikurangi** dengan merangkum laporan detail menjadi analisis yang langsung dapat ditindaklanjuti.
4. **Pemecahan bagian diperbaiki** agar pembaca dapat bergerak dari ringkasan → prioritas → tindakan → baseline.
5. **Fokus bisnis diperkuat** sehingga dokumen tidak berhenti pada data teknis, tetapi jelas mengarah ke keputusan pengadaan dan mitigasi risiko.
