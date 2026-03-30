# Assessment Methodology

## Pendekatan Penilaian Dua Lapis

Penentuan prioritas peremajaan perangkat dalam laporan ini tidak dilakukan hanya berdasarkan usia perangkat atau angka kesehatan penyimpanan semata. Setiap unit dinilai melalui dua lapis bukti yang saling melengkapi:

1. **Bukti Teknis** - Data objektif dari pemeriksaan hardware dan sistem
2. **Bukti Operasional** - Pengalaman subjektif pengguna dalam penggunaan sehari-hari

Kombinasi kedua lapis bukti ini memastikan rekomendasi tidak hanya menjawab "apakah perangkat ini tua atau tidak", melainkan "apakah perangkat ini masih layak menopang kerja aktual dengan risiko yang bisa diterima".

## Sumber Data dan Proses Pengumpulan

### 1. Sumber Data Teknis
- **DxDiag Reports:** Informasi sistem operasi, prosesor, memori, grafis, audio, dan driver
- **Hardware Inspection:** Spesifikasi teknis perangkat, usia komponen, kondisi fisik
- **System Monitoring Data:** Utilisasi RAM, penggunaan page file, kesehatan penyimpanan, suhu sistem
- **Performance Logs:** Catatan kinerja sistem dan indikator stabilitas

### 2. Sumber Data Operasional
- **User Feedback:** Keluhan langsung pengguna tentang pengalaman kerja
- **Qualitative Assessment:** Dokumen penilaian kualitatif yang memotret hambatan kerja
- **Incident Reports:** Catatan kejadian BSOD, mati mendadak, dan gangguan kritis
- **Workflow Analysis:** Dampak perangkat terhadap alur kerja spesifik pengguna

### 3. Proses Validasi Data
1. **Koleksi Data:** Pengumpulan bukti teknis dan operasional dari semua sumber yang tersedia
2. **Korelasi Bukti:** Penyelarasan temuan teknis dengan pengalaman operasional
3. **Verifikasi Silang:** Pemeriksaan konsistensi antar sumber data
4. **Konteksualisasi:** Penempatan temuan dalam konteks peran dan kebutuhan pengguna

## Parameter Penilaian Teknis

### 1. Prosesor (CPU)
- **Kelas dan Generasi:** Intel Core i3, i5, i7 dengan generasi spesifik
- **Usia Platform:** Berdasarkan tahun rilis dan dukungan vendor
- **Kecukupan untuk Beban Kerja:** Evaluasi terhadap kebutuhan aplikasi bisnis

### 2. Memori (RAM)
- **Kapasitas Terpasang:** 4 GB, 8 GB, atau lainnya
- **Utilisasi Aktual:** Persentase penggunaan RAM saat beban kerja normal
- **Page File Usage:** Indikator tekanan memori dan ketergantungan pada virtual memory
- **Memory Availability:** Sisa memori yang tersedia untuk multitasking

### 3. Penyimpanan (Storage)
- **Tipe Media:** HDD, SSD, NVMe SSD
- **Health Status:** Persentase kesehatan, suhu operasional, bad sectors
- **Available Space:** Ruang kosong yang tersedia untuk sistem dan data
- **Performance Indicators:** Kecepatan baca/tulis, latency

### 4. Komponen Pendukung
- **Grafis (GPU):** Kemampuan grafis terintegrasi atau diskrit
- **Audio:** Status driver dan fungsi playback/recording
- **Jaringan:** Konektivitas wired/wireless
- **Periferal:** Kondisi keyboard, mouse, monitor, webcam, mikrofon

### 5. Sistem Operasi
- **Versi dan Arsitektur:** Windows 10 32-bit vs 64-bit
- **Update Status:** Tingkat pembaruan keamanan dan fitur
- **Driver Compatibility:** Kesesuaian driver dengan hardware

## Parameter Penilaian Operasional

### 1. Gangguan Kinerja
- **Lag dan Freeze:** Kelambatan respons sistem
- **Application Not Responding:** Pembekuan aplikasi yang sering terjadi
- **Slow Boot/Shutdown:** Waktu startup/shutdown yang tidak normal

### 2. Masalah Stabilitas
- **BSOD (Blue Screen of Death):** Kejadian crash sistem
- **Unexpected Shutdown:** Mati mendadak tanpa peringatan
- **System Instability:** Ketidakstabilan umum sistem

### 3. Dampak terhadap Aplikasi Bisnis
- **Excel Performance:** Lambat saat membuka/memproses file besar
- **Outlook/Browser Issues:** Gangguan pada aplikasi komunikasi
- **Payroll System:** Kinerja sistem payroll yang terhambat
- **Meeting Applications:** Kendala pada aplikasi rapat daring

### 4. Kerusakan Fisik dan Ergonomi
- **Physical Damage:** Chassis patah, layar bermasalah, keyboard rusak
- **Battery Degradation:** Kapasitas baterai yang menurun drastis
- **Peripheral Failure:** Mikrofon, webcam, atau perangkat input yang tidak berfungsi
- **Ergonomics Issues:** Ukuran monitor tidak sesuai, kursor menghilang

### 5. Konteks Penggunaan
- **Workload Intensity:** Beban kerja harian vs penggunaan sesekali
- **Mobility Requirements:** Kebutuhan mobilitas untuk laptop
- **Role Specific Needs:** Kebutuhan spesifik berdasarkan peran pengguna
- **Business Criticality:** Tingkat kritisitas perangkat terhadap operasi bisnis

## Kategori Prioritas dan Definisi

Untuk menjaga konsistensi terminologi, laporan ini menggunakan empat kategori prioritas dengan definisi berikut:

### 1. Penggantian Segera
**Definisi:** Unit sudah menunjukkan kombinasi hambatan kerja nyata, keterbatasan perangkat keras berat, dan/atau risiko kestabilan tinggi yang membuat perbaikan parsial tidak lagi efisien.

**Indikator:**
- BSOD atau mati mendadak yang sering terjadi
- Kombinasi RAM 4 GB dengan utilisasi tinggi (>85%)
- Media penyimpanan dengan health status kritis (<80%)
- Kerusakan fisik serius (chassis patah, baterai bocor)
- Platform prosesor yang sangat tua dengan arsitektur terbatas

### 2. Penyegaran Prioritas Tinggi
**Definisi:** Unit masih dapat digunakan dalam jangka pendek, tetapi sudah membatasi produktivitas, mobilitas, atau keandalan kerja dan perlu masuk batch pengadaan berikutnya.

**Indikator:**
- RAM tertekan dengan page file tinggi
- Performa menurun untuk aplikasi bisnis kritis
- Kerusakan periferal yang mengganggu kerja (mikrofon, keyboard)
- Kebutuhan form factor atau spesifikasi yang lebih sesuai
- Platform mulai menua tetapi belum menunjukkan kegagalan kritis

### 3. Perbaikan/Upgrade Terlebih Dahulu
**Definisi:** Unit yang inti perangkat kerasnya masih cukup memadai dan masalah utamanya lebih mungkin diselesaikan melalui perbaikan sistem, penggantian komponen tertentu, atau upgrade terbatas.

**Indikator:**
- Masalah bersumber dari perangkat lunak atau konfigurasi
- Komponen tertentu yang dapat diupgrade (RAM, storage)
- Performa umum masih memadai dengan intervensi terbatas
- Tidak ada bukti kegagalan hardware mendasar

### 4. Pertahankan
**Definisi:** Unit yang masih memenuhi fungsi bisnis saat ini, tidak memunculkan keluhan besar, atau berperan sebagai sistem siaga yang tetap stabil.

**Indikator:**
- Performa memadai untuk kebutuhan saat ini
- Tidak ada keluhan operasional signifikan
- Peran sebagai sistem siaga atau backup
- Spesifikasi masih sesuai dengan beban kerja

## Prinsip Pengambilan Keputusan

### 1. Evidence-Based
Setiap rekomendasi didukung oleh bukti teknis dan/atau operasional yang terdokumentasi.

### 2. Risk-Adjusted
Tingkat urgensi disesuaikan dengan potensi dampak terhadap operasi bisnis.

### 3. Cost-Benefit Conscious
Pertimbangan efisiensi antara biaya perbaikan/upgrade vs penggantian.

### 4. User-Centric
Fokus pada dampak terhadap produktivitas dan pengalaman pengguna.

### 5. Future-Proofing
Pertimbangan kesiapan perangkat untuk tuntutan kerja dalam 4 tahun ke depan.

Metodologi ini memastikan bahwa rekomendasi akhir bersifat holistik, kontekstual, dan langsung terkait dengan dampak bisnis yang nyata.