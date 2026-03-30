# Laporan Penilaian Kualitatif Infrastruktur Perangkat Keras HHI

Dokumen ini menyajikan analisis mendalam mengenai kondisi perangkat keras yang saat ini digunakan oleh staf. Penilaian mencakup kendala operasional (pain points), performa teknis, dan rekomendasi strategis untuk memastikan keberlangsungan produktivitas perusahaan.

---

## 1. Analisis Perangkat Keras Berdasarkan Pengguna

### 1.1. Unit Foxpro (PC System)
*   **Spesifikasi:** i3-4160 @ 3.60GHz, 4GB RAM, Windows 10 Pro 32-bit.
*   **Kendala Operasional:**
    *   Mengalami penurunan performa signifikan (sangat lambat) saat menjalankan aplikasi komunikasi (WhatsApp) dan peramban web.
    *   Ketidakstabilan koneksi internet yang mengharuskan perangkat di-restart secara manual agar berfungsi kembali.
*   **Analisis Teknis:** Arsitektur 32-bit membatasi penggunaan RAM secara efisien. Meskipun prosesor i3 generasi ke-4 masih fungsional, kapasitas RAM 4GB menjadi hambatan utama dalam menangani aplikasi modern yang haus sumber daya.
*   **Rekomendasi:** **Peningkatan RAM**. Mengingat efisiensi waktu setup dan biaya, serta kebutuhan fungsional yang terbatas pada pengecekan stok, disarankan menambah RAM hingga 12GB atau 16GB.

### 1.2. Unit Renaldi (PC System)
*   **Spesifikasi:** i5-8400 @ 2.80GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:**
    *   Sering terjadi hambatan (lag) dan pembekuan sistem (freeze) saat mengolah data Excel dalam jumlah banyak (multi-tab).
    *   Insiden Blue Screen of Death (BSOD) yang menunjukkan ketidakstabilan sistem atau kegagalan perangkat keras.
    *   Ketiadaan kamera web (webcam) menghambat partisipasi dalam rapat daring bulanan.
*   **Analisis Teknis:** Kesehatan penyimpan data (disk health) berada pada level kritis (85%). RAM 4GB sangat tidak memadai untuk multitasking intensif di Windows 10.
*   **Rekomendasi:** **Penggantian Unit (Replacement)**. Unit baru harus dilengkapi dengan minimal 16GB RAM, SSD yang sehat, dan kamera web terintegrasi untuk mendukung kebutuhan komunikasi.

### 1.3. Unit Renaldi - PC System Autocount
*   **Spesifikasi:** i5-8400 @ 2.80GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kondisi Saat Ini:** Berfungsi dengan baik sebagai sistem standby untuk aplikasi Autocount. Tidak ada kendala operasional yang dilaporkan.
*   **Rekomendasi:** **Pertahankan (No Replacement)**. Penambahan RAM bersifat opsional sesuai kebutuhan ekspansi sistem di masa depan.

### 1.4. Unit Diana (PC)
*   **Spesifikasi:** i5-8400 @ 2.80GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:**
    *   Kapasitas kerja terbatas; sistem mengalami kegagalan (hang/error) jika membuka lebih dari dua berkas Excel secara bersamaan.
    *   Insiden Blue Screen of Death (BSOD) dan sering mati secara mendadak.
    *   Performa sangat lambat saat mengakses basis data ORS Payroll (Microsoft Access).
*   **Analisis Teknis:** Insiden BSOD dan kematian mendadak sering kali mengindikasikan masalah pada unit catu daya (PSU), overheating, atau ketidakstabilan memori.
*   **Rekomendasi:** **Penggantian Unit (Replacement)**. Diperlukan perangkat dengan manajemen memori yang lebih baik untuk mendukung beban kerja administratif.

### 1.5. Unit Yohana (PC)
*   **Spesifikasi:** i5-8400 @ 2.80GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:**
    *   Keluhan ergonomis terkait dimensi layar yang terlalu kecil dibandingkan unit sebelumnya.
    *   Malfungsi input (kursor menghilang) yang menghambat alur kerja.
    *   Gejala penurunan kecepatan saat menjalankan banyak aplikasi simultan.
    *   Insiden Blue Screen of Death (BSOD) yang menunjukkan ketidakstabilan sistem.
*   **Rekomendasi:** Perbaikan perangkat input (mouse/konektor) dan evaluasi penggantian monitor ke dimensi yang lebih ergonomis. BSOD mengindikasikan risiko stabilitas sistem yang perlu ditangani segera.

### 1.6. Unit Hibab (Laptop)
*   **Spesifikasi:** i5-7200U @ 2.50GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:**
    *   Waktu tunggu yang lama saat membuka Outlook dan aplikasi produktivitas lainnya.
    *   Degradasi baterai: daya bertahan sangat singkat terutama saat digunakan untuk rapat daring.
*   **Rekomendasi:** Penggantian baterai dan peningkatan penyimpanan ke SSD (jika masih menggunakan HDD) serta penambahan RAM.

### 1.7. Unit Hibab - PC System Foxpro
*   **Kondisi Fisik:** Layar mengalami kerusakan visual (bergaris) dan baterai mengalami kebocoran total (harus selalu terhubung ke pengisi daya).
*   **Status Operasional:** Meskipun rusak secara fisik, fungsi sistem Foxpro sebagai alat standby masih berjalan tanpa kendala software yang berarti.
*   **Rekomendasi:** Monitoring ketat; penggantian hanya dilakukan jika kerusakan layar menghalangi visibilitas operasional.

### 1.8. Unit Regina (Laptop)
*   **Spesifikasi:** i5-8265U @ 1.60GHz, 4GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:**
    *   Performa ekstrem lambat untuk pengerjaan Excel dan Outlook.
    *   Ketidakstabilan sistem (sering BSOD).
    *   Kerusakan fisik (chassis/part patah) dan kebocoran baterai (daya berkurang 50% dalam 15 menit).
*   **Rekomendasi:** **Penggantian Unit Segera**. Kerusakan fisik dikombinasikan dengan kegagalan sistematis (BSOD) menunjukkan unit tidak lagi layak pakai.

### 1.9. Unit Foxpro Sales Support
*   **Kendala Fisik:** Tidak memiliki baterai dan keyboard mengalami malfungsi pada beberapa tombol.
*   **Performa:** Proses akses stok dan pengecekan sistem berjalan lambat.
*   **Rekomendasi:** Penyediaan keyboard eksternal sebagai solusi jangka pendek dan evaluasi penggantian ke unit yang lebih portabel.

### 1.10. Unit Wulan
*   **Spesifikasi:** i5-10400 @ 2.90GHz, 8GB RAM, Windows 10 Pro 64-bit.
*   **Kendala Operasional:** Terjadi pembekuan sistem (Not Responding) setelah melakukan unduhan dokumen (PDF).
*   **Analisis Teknis:** Memiliki spesifikasi yang cukup mumpuni (generasi ke-10, 8GB RAM). Masalah kemungkinan besar terletak pada korupsi sistem operasi atau gangguan pada perangkat lunak pihak ketiga.
*   **Rekomendasi:** Instalasi ulang sistem operasi atau pemeriksaan kesehatan media penyimpanan.

### 1.11. Unit Robin (PC)
*   **Spesifikasi:** i5-10400 @ 2.90GHz, 8GB RAM, Windows 11 Home 64-bit.
*   **Status:** Tidak ada kendala. Performa stabil untuk kebutuhan input data Excel.
*   **Rekomendasi:** Pertahankan pemeliharaan rutin.

### 1.12. Unit Christy (Laptop)
*   **Spesifikasi:** i5-10210U @ 1.60GHz, 8GB RAM, Windows 10 IoT Enterprise LTSC 64-bit.
*   **Kendala & Preferensi:**
    *   Kerusakan komponen audio (mic) dan kerusakan fisik pada keyboard.
    *   Kebutuhan akan penyimpanan yang lebih besar (target 1TB).
    *   Preferensi desain yang ringkas (simpel/tidak lebar).
*   **Rekomendasi:** Mengingat preferensi spesifik dan kerusakan perangkat input, disarankan penggantian ke laptop kategori *ultrabook* dengan kapasitas SSD 1TB.

---

## 2. Poin Utama & Ringkasan Hambatan (Bottlenecks)

1.  **Kapasitas RAM Kurang Memadai:** Mayoritas unit masih menggunakan RAM 4GB, yang merupakan ambang batas minimal untuk menjalankan Windows 10, sehingga menghambat efisiensi multitasking.
2.  **Degradasi Baterai & Fisik:** Sebagian besar laptop mengalami kebocoran baterai yang ekstrem dan kerusakan fisik (chassis patah, keyboard rusak), yang dapat menyebabkan gangguan keamanan kerja atau kebakaran arus pendek.
3.  **Hambatan Produktivitas:** Keluhan "lemot" dan "freeze" saat membuka Excel dan Outlook menunjukkan bahwa infrastruktur IT saat ini tidak lagi selaras dengan volume beban kerja staf.

## 3. Rekomendasi Strategis Umum

*   **Standardisasi RAM:** Menetapkan standar minimal RAM 16GB untuk staf dengan beban kerja Excel intensif.
*   **Transisi ke SSD:** Memastikan seluruh unit yang lambat telah menggunakan SSD sebagai media penyimpanan utama guna mengatasi masalah "loading lama".
*   **Audit Kesehatan Fisik berkala:** Melakukan pengecekan rutin terhadap kondisi baterai dan integritas fisik laptop untuk mencegah kerusakan yang lebih fatal.
