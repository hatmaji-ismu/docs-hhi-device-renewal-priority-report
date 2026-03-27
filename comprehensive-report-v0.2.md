# Comprehensive Hardware Replacement Report / Laporan Komprehensif Penggantian Perangkat

## Executive Summary / Ringkasan Eksekutif
Laporan ini merupakan kompilasi **12 hardware assessment report** yang diperkuat dengan **qualitative-assessment.md** agar keputusan penggantian perangkat tidak hanya berbasis `specification` dan `disk health`, tetapi juga berbasis **pain point operasional nyata** di lapangan seperti `lag`, `freeze`, `BSOD`, kerusakan fisik, baterai bocor, dan hambatan meeting online.

Setelah menggabungkan **evidence teknis** dan **dampak operasional**, urgensi armada perangkat direvisi menjadi:

* **5 unit**: **Replace Now / Ganti Segera**
* **4 unit**: **High Priority Refresh / Prioritas Tinggi**
* **1 unit**: **Upgrade/Repair First / Perbaiki atau Upgrade Dulu**
* **2 unit**: **Maintain / No Replacement Now / Pertahankan**

Temuan utama:

* Masalah paling dominan tetap **RAM 4 GB**, yang secara konsisten menyebabkan `high memory utilization`, `Page File` tinggi, dan penurunan responsivitas.
* Sejumlah unit kini naik urgensinya karena ditemukan **BSOD**, **shutdown mendadak**, **kerusakan fisik**, **baterai bocor**, atau `workflow disruption` yang tidak sepenuhnya terlihat dari laporan hardware saja.
* Sebaliknya, ada unit yang secara teknis masih lama tetapi **fungsi operasionalnya masih stabil**, sehingga tidak perlu diprioritaskan untuk penggantian segera.

Kesimpulan manajerial:

* Organisasi sebaiknya menjalankan **replacement program bertahap**, dimulai dari unit yang sudah menunjukkan kombinasi **kegagalan operasional nyata + keterbatasan hardware**.
* Unit yang masih sehat namun mulai sempit di RAM dapat dipertahankan sementara melalui **upgrade RAM ke 16 GB** dan perbaikan minor.
* Unit yang sudah menimbulkan gangguan kerja rutin sebaiknya **tidak lagi dipertahankan terlalu lama**, karena biaya `downtime`, support, dan hilangnya produktivitas akan lebih tinggi daripada biaya refresh.

## Basis Penilaian / Assessment Basis
Prioritas pada laporan ini disusun dari dua lapis evidence:

* **Technical findings** dari laporan hardware per unit
* **Qualitative findings** dari `qualitative-assessment.md`

Qualitative findings digunakan untuk menaikkan atau menurunkan urgensi jika ditemukan:

* `BSOD`
* `freeze`
* `sudden shutdown`
* baterai bocor atau rusak berat
* kerusakan layar, keyboard, chassis, audio, webcam, atau perangkat input
* unit standby yang masih berfungsi baik

## Dokumen Sumber / Source Documents
Laporan ini mengompilasi:

* `HHI Assestment/Yohana/Yohana_Hardware_Report.md`
* `HHI Assestment/Wulan/Wulan_Hardware_Report.md`
* `HHI Assestment/System Finance/System_Finance_Hardware_Report.md`
* `HHI Assestment/System Autocount/System_Autocount_Hardware_Report.md`
* `HHI Assestment/Syela/Syela_Hardware_Report.md`
* `HHI Assestment/Robin/Robin_Hardware_Report.md`
* `HHI Assestment/Renaldi/Renaldi_Hardware_Report.md`
* `HHI Assestment/Regina/Regina_Hardware_Report.md`
* `HHI Assestment/Hibab/Hibab_Hardware_Report.md`
* `HHI Assestment/Diana/Diana_Hardware_Report.md`
* `HHI Assestment/Devinta/Devinta_Hardware_Report.md`
* `HHI Assestment/Christy/Christy_Hardware_Report.md`
* `qualitative-assessment.md`

## Fleet Summary / Ringkasan Armada Perangkat

| Kategori | Jumlah | Makna Operasional |
| :--- | :---: | :--- |
| Replace Now / Ganti Segera | 5 | Gangguan kerja nyata, risiko kerusakan/ketidakstabilan tinggi, atau platform sudah terlalu tua |
| High Priority Refresh / Prioritas Tinggi | 4 | Masih bisa dipakai sementara, tetapi sangat membatasi produktivitas dan butuh tindakan cepat |
| Upgrade/Repair First / Upgrade atau Perbaiki Dulu | 1 | Perangkat inti masih memadai, masalah lebih condong ke software atau komponen tertentu |
| Maintain / No Replacement Now / Pertahankan | 2 | Tidak ada kendala operasional berarti atau hanya perlu pemeliharaan ringan |

## Actionable Table / Tabel Tindakan Prioritas

| Unit | Device Profile | Technical Risk | Qualitative Pain Point | Dampak Bisnis / Business Impact | Recommended Action | Urgency |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **System Finance** | i3-4160, 4 GB RAM, Windows 10 32-bit, HDD | Platform usang, usable RAM rendah, driver lama | Sangat lambat untuk WhatsApp dan browser, internet kadang harus restart manual | Produktivitas rendah dan platform sudah tidak layak untuk beban kerja modern | **Replace unit**. Upgrade parsial tidak lagi rasional secara ekonomi | **Replace Now** |
| **Renaldi** | i5-8400, 4 GB RAM, SSD warning | RAM kritis, SSD spare area terpakai, suhu tinggi | `Lag`, `freeze`, `BSOD`, tidak ada webcam untuk meeting | Risiko operasional tinggi, potensi data loss dan gangguan kerja nyata | **Replace unit**. Lakukan `backup` segera sambil menunggu replacement | **Replace Now** |
| **Diana** | i5-8400, 4 GB RAM, SSD panas | RAM kritis, SSD 61 C, free space terbatas | Sering `hang`, error saat buka >2 file Excel, sering mati mendadak, lambat di ORS Payroll | Ada indikasi masalah stabilitas/power/overheating, mengganggu pekerjaan administrasi | **Replace unit**. Jangan hanya mengandalkan upgrade RAM | **Replace Now** |
| **Regina** | i5-8265U, 4 GB RAM, SSD 75% | RAM kritis, SSD wear, driver tua | Sangat lambat, sering `BSOD`, chassis patah, baterai drop 50% dalam 15 menit | Kombinasi kerusakan fisik + ketidakstabilan sistem membuat unit tidak layak pakai | **Immediate replacement** | **Replace Now** |
| **Syela** | i5-8400, 4 GB RAM, SSD 78% | RAM kritis, SSD hampir penuh, health turun, suhu 54 C | Tidak ada input kualitatif khusus, tetapi bukti teknis menunjukkan risiko tinggi | Performa tertekan konsisten dan storage sudah sempit untuk operasi stabil | **Replace unit** lebih aman daripada hanya perbaikan parsial | **Replace Now** |
| **Christy** | i5-10210U, 8 GB RAM, laptop | RAM mulai berat, driver GPU menua | Mic rusak, keyboard rusak, butuh SSD 1 TB, preferensi laptop ringkas | Masih usable, tetapi kebutuhan kerja dan kondisi perangkat mengarah ke refresh | **High priority laptop replacement** sesuai kebutuhan role | **High Priority Refresh** |
| **Yohana** | i5-8400, 4 GB RAM, SSD 256 GB | RAM 92%, storage health belum tervalidasi | Monitor terlalu kecil, kursor sering hilang, mulai lambat saat banyak aplikasi | Produktivitas harian terganggu, tetapi belum ada bukti kerusakan fatal total | **Upgrade RAM + perbaiki input/monitor**, masuk refresh batch berikutnya | **High Priority Refresh** |
| **Hibab** | i5-7200U, 4 GB RAM, laptop | RAM kritis, platform lama | Outlook lambat, baterai cepat habis, perangkat lama untuk meeting | Masih bisa dipertahankan pendek, tetapi user experience sudah buruk | **Ganti baterai + upgrade RAM** jika ingin menunda, namun siapkan replacement | **High Priority Refresh** |
| **Devinta** | i5-8400, 8 GB RAM, SSD sehat | RAM mulai sempit, platform menua, audio issue | Belum ada pain point lapangan tambahan, tetapi hardware report sudah menunjukkan pressure | Layak dipertahankan sementara, namun performa multitasking mulai tertahan | **Upgrade RAM ke 16 GB** dan perbaiki audio | **High Priority Refresh** |
| **Wulan** | i5-10400, 8 GB RAM, SSD 88% | RAM 82%, SSD wear moderat | `Not Responding` setelah download PDF; indikasi lebih dekat ke software issue | Perangkat inti masih cukup baik, replacement belum mendesak | **Repair/OS reinstall first**, upgrade RAM jika perlu | **Upgrade/Repair First** |
| **Robin** | i5-10400, 8 GB RAM, SSD sehat | RAM mulai sempit, audio playback issue pada DxDiag | Tidak ada kendala operasional, performa stabil untuk Excel | Belum ada alasan bisnis kuat untuk replacement segera | **Maintain**, perbaiki audio bila memang dibutuhkan, upgrade RAM opsional | **Maintain / No Replacement Now** |
| **System Autocount** | i5-8400, 4 GB RAM, SSD + HDD sehat | RAM 4 GB, audio playback issue | Sistem standby Autocount masih berjalan baik, tidak ada keluhan operasional | Fungsi role masih terpenuhi, tidak perlu diprioritaskan untuk replacement | **Maintain**, upgrade RAM hanya jika kebutuhan sistem bertambah | **Maintain / No Replacement Now** |

## Revised Replacement Priority / Prioritas Penggantian Revisi

### 1. Replace Now / Ganti Segera
Unit di kategori ini memiliki kombinasi **gangguan operasional nyata**, **hardware limitation berat**, dan/atau **risiko kestabilan tinggi**.

* **System Finance**
* **Renaldi**
* **Diana**
* **Regina**
* **Syela**

Alasan bisnis:

* `Downtime` atau `freeze` sudah memengaruhi kerja
* Ada `BSOD`, shutdown mendadak, atau kerusakan fisik
* Biaya support akan terus meningkat
* Upgrade parsial berisiko tidak menyelesaikan akar masalah

### 2. High Priority Refresh / Prioritas Tinggi
Unit masih bisa digunakan sementara, tetapi sudah jelas tidak lagi nyaman atau efisien untuk beban kerja modern.

* **Christy**
* **Yohana**
* **Hibab**
* **Devinta**

Alasan bisnis:

* Bottleneck RAM atau kerusakan periferal sudah terasa
* Perangkat mulai tidak sesuai dengan kebutuhan kerja aktual
* Masih ada ruang untuk tindakan transisi, tetapi sebaiknya tidak ditunda terlalu lama

### 3. Upgrade/Repair First / Upgrade atau Perbaiki Dulu
Unit di kategori ini masih punya inti hardware yang cukup baik dan problem utamanya belum mengarah langsung ke replacement.

* **Wulan**

Alasan bisnis:

* Spesifikasi inti masih cukup memadai
* Gejala lebih mirip `software issue` atau gangguan OS/app
* Masih layak dicoba `repair-first strategy`

### 4. Maintain / No Replacement Now / Pertahankan
Unit masih memenuhi fungsi operasional dan tidak ada urgensi bisnis untuk penggantian langsung.

* **Robin**
* **System Autocount**

Alasan bisnis:

* Tidak ada keluhan operasional signifikan
* Perangkat masih cukup stabil untuk role saat ini
* Penggantian saat ini belum memberi ROI setinggi unit lain

## Key Cross-Fleet Themes / Tema Umum Seluruh Armada

### 1. RAM 4 GB Sudah Tidak Layak / 4 GB RAM Is Below Business Baseline
Mayoritas masalah performa paling nyata berasal dari memori yang terlalu kecil.

* Semua unit **4 GB RAM** menunjukkan bottleneck nyata atau ruang kerja yang sangat sempit
* Bahkan unit **8 GB RAM** sudah mulai menunjukkan pressure
* Baseline organisasi untuk 2026 sebaiknya dinaikkan ke **16 GB RAM**

### 2. Operational Reality Matters / Realitas Operasional Sangat Menentukan
Qualitative assessment menunjukkan bahwa keputusan replacement tidak bisa hanya berbasis spesifikasi.

Contoh:

* **System Autocount** secara teknis tua, tetapi masih efektif untuk role standby
* **Wulan** terlihat lebih cocok diperbaiki dulu daripada diganti
* **Regina** dan **Diana** harus dinaikkan urgensinya karena `BSOD`, baterai rusak, atau shutdown mendadak

### 3. Audio and Peripheral Reliability / Keandalan Audio dan Periferal
Masalah `audio playback`, keyboard, mic, mouse, layar, dan baterai terbukti menjadi penghambat kerja yang tidak kalah penting dibanding CPU/RAM.

Implikasi:

* Meeting dan komunikasi terganggu
* Produktivitas turun meskipun CPU/storage masih cukup
* `End-user frustration` meningkat

### 4. Storage Risk Is Selective / Risiko Storage Tidak Merata
Tidak semua unit perlu penggantian disk. Fokus storage sebaiknya diarahkan pada:

* **Renaldi**
* **Syela**
* **Regina**
* **Diana**
* Pemantauan moderat untuk **Wulan**

## Recommended Management Actions / Rekomendasi Tindakan Manajerial

### Immediate Actions / Tindakan Segera
* Setujui **replacement batch pertama** untuk `System Finance`, `Renaldi`, `Diana`, `Regina`, dan `Syela`
* Lakukan `backup` prioritas pada unit yang storage-nya sudah berisiko, terutama `Renaldi` dan `Syela`
* Selesaikan isu **audio/peripheral** yang paling mengganggu sambil menunggu proses replacement

### 30-60 Day Plan / Rencana 30-60 Hari
* Siapkan **refresh batch kedua** untuk `Christy`, `Yohana`, `Hibab`, dan `Devinta`
* Jalankan `repair-first strategy` untuk `Wulan`
* Pertahankan `Robin` dan `System Autocount` dengan monitoring rutin

### Standard Baseline 2026 / Standar Minimum 2026
Untuk unit pengganti baru, baseline minimum yang disarankan:

* **CPU**: minimal kelas modern setara Intel Core i5 generasi baru
* **Memory**: **16 GB RAM**
* **Storage**: SSD/NVMe sehat
* **OS**: 64-bit modern dan supported
* **Peripherals**: audio, webcam, keyboard, dan baterai harus siap pakai sesuai role pengguna

## Final Executive Recommendation / Rekomendasi Eksekutif Akhir
Dengan tambahan `qualitative-assessment.md`, urgensi penggantian perangkat menjadi lebih jelas:

* **Prioritaskan replacement** untuk unit yang sudah mengganggu kerja nyata, bukan hanya yang spesifikasinya tua
* **Jangan samakan semua unit lama**. Beberapa masih layak dipertahankan jika fungsi bisnisnya masih stabil
* **Gunakan pendekatan bertahap**: replace yang paling kritis, refresh yang menghambat produktivitas, dan pertahankan unit yang masih stabil

Keputusan paling rasional saat ini adalah:

* **Replace Now**: `System Finance`, `Renaldi`, `Diana`, `Regina`, `Syela`
* **High Priority Refresh**: `Christy`, `Yohana`, `Hibab`, `Devinta`
* **Repair First**: `Wulan`
* **Maintain**: `Robin`, `System Autocount`

Dengan pendekatan ini, organisasi bisa menekan `downtime`, mengurangi frustrasi pengguna, dan meningkatkan ROI dari program refresh perangkat secara lebih terarah.
