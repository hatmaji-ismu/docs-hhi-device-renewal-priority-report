# Renewal Priority & Recommendation

## Daftar Prioritas Penggantian

Berdasarkan analisis komprehensif terhadap bukti teknis dan operasional, berikut adalah rekomendasi prioritas penggantian perangkat.

> **Catatan Penting:** Prioritas yang tertera dalam dokumen ini bersifat **saran awal** dan dapat disesuaikan berdasarkan:
> - **Kondisi operasional bisnis** yang sedang terjadi pada saat keputusan akan diambil
> - **Tingkat urgensi** penggunaan perangkat oleh masing-masing user
> - **Jabatan dan peran** user dalam organisasi — unit yang digunakan oleh pengguna dengan jabatan lebih tinggi atau peran yang lebih kritis secara bisnis dapat diprioritaskan lebih awal
>
> Daftar ini memerlukan **koreksi dan validasi final** dari manajemen berdasarkan kebijakan internal, ketersediaan anggaran, dan strategi organisasi.

### Kategori 1: Penggantian Segera (5 Unit)

Unit-unit ini menunjukkan kombinasi risiko yang membuat perbaikan parsial tidak lagi efisien atau efektif:

| Unit | Alasan Prioritas | Rekomendasi Tindakan | Timeline |
| :--- | :--- | :--- | :--- |
| **System Finance** | Platform sangat tua (i3-4160), Windows 10 32-bit, RAM efektif hanya ~3.5 GB, audio tidak terdeteksi | Ganti dengan desktop modern (min. i5 gen 10+, RAM 16 GB, SSD 512 GB, Windows 11 64-bit) | Batch 1 - Fase 1 |
| **Renaldi** | RAM kritis (87%), SSD health 85% dengan suhu 66°C, menggunakan reserved spare area, BSOD terjadi | Ganti dengan desktop performa tinggi (i5/i7 gen 12+, RAM 16 GB, NVMe SSD 512 GB, cooling adequate) | Batch 1 - Fase 1 |
| **Diana** | BSOD dan mati mendadak, gangguan Excel dan ORS Payroll, RAM kritis (85%), SSD panas (61°C) | Ganti dengan desktop untuk workload administrasi (i5 gen 12+, RAM 16 GB, SSD 512 GB, reliable PSU) | Batch 1 - Fase 1 |
| **Regina** | BSOD, chassis patah, baterai turun 50% dalam 15 menit, RAM 92%, SSD health 75% | Ganti dengan laptop business-grade (i5/i7 gen 12+, RAM 16 GB, SSD 512 GB, battery 8+ hours) | Batch 1 - Fase 1 |
| **Syela** | Storage hampir penuh (5.6 GB free), SSD health 78%, RAM kritis (87%), tekanan sistem tinggi | Ganti dengan desktop standar (i5 gen 11+, RAM 16 GB, SSD 512 GB, adequate storage) | Batch 1 - Fase 1 |

### Kategori 2: Penyegaran Prioritas Tinggi (4 Unit)

Unit-unit ini masih dapat digunakan sementara tetapi memerlukan penyegaran dalam batch berikutnya:

| Unit | Alasan Prioritas | Rekomendasi Tindakan | Timeline |
| :--- | :--- | :--- | :--- |
| **Christy** | Mikrofon & keyboard rusak, kebutuhan form factor berbeda, RAM tertekan (89%) | Ganti dengan laptop ultrabook (i5/i7 gen 12+, RAM 16 GB, SSD 1 TB, lightweight design) | Batch 2 - Fase 2 |
| **Yohana** | RAM sangat terbatas (92%), BSOD, gangguan input (kursor hilang), monitor terlalu kecil | Upgrade interim: tambah RAM ke 16 GB, ganti monitor 24"; investigasi BSOD dan siapkan penggantian desktop | Batch 2 - Fase 2 |
| **Hibab** | Platform mobile menua (i5-7200U), baterai degradasi, performa Outlook menurun | Ganti dengan laptop business (i5 gen 12+, RAM 16 GB, SSD 512 GB, good battery life) | Batch 2 - Fase 2 |
| **Devinta** | Platform mulai menua, tekanan multitasking tinggi, audio tidak terdeteksi | Upgrade interim: tambah RAM ke 16 GB, perbaiki audio; siapkan penggantian desktop | Batch 2 - Fase 2 |

### Kategori 3: Perbaikan/Upgrade Terlebih Dahulu (1 Unit)

Unit ini lebih tepat diperbaiki atau diupgrade terlebih dahulu:

| Unit | Alasan | Rekomendasi Tindakan | Timeline |
| :--- | :--- | :--- | :--- |
| **Wulan** | Masalah kemungkinan software-related, CPU masih memadai, SSD health 88% | Lakukan clean install OS, upgrade RAM ke 16 GB, monitor SSD health | Immediate - Maintenance |

### Kategori 4: Pertahankan (2 Unit)

Unit-unit ini masih memenuhi fungsi saat ini dan dapat dipertahankan:

| Unit | Alasan | Rekomendasi Tindakan | Timeline |
| :--- | :--- | :--- | :--- |
| **Robin** | Stabil, tidak ada keluhan signifikan, spesifikasi adequate untuk workload saat ini | Pertahankan; monitor performance; upgrade RAM opsional ke 16 GB | Ongoing - Monitor |
| **System Autocount** | Sistem siaga, fungsi terpenuhi, tidak urgent untuk penggantian | Pertahankan; upgrade RAM hanya jika beban kerja meningkat | Ongoing - Monitor |

## Strategi Peremajaan Bertahap (Phased Renewal Plan)

### Fase 1: Batch Pertama - Penggantian Segera
**Target:** 5 unit dengan risiko tertinggi
**Timeline:** Setelah persetujuan anggaran — Fase 1
**Fokus:** Mitigasi risiko operasional tertinggi (BSOD, mati mendadak, kegagalan storage)

**Unit Prioritas:**
1. Renaldi (risiko kehilangan data tertinggi)
2. Diana (BSOD, mati mendadak, gangguan aplikasi bisnis kritis)
3. Regina (kerusakan fisik dan mobilitas)
4. System Finance (platform sangat tua)
5. Syela (storage hampir penuh)

**Tindakan Pendukung:**
- Backup data prioritas sebelum penggantian
- Migrasi data dan konfigurasi terencana
- Pelatihan pengguna singkat untuk perangkat baru
- Disposal/pergantian perangkat lama sesuai policy

### Fase 2: Batch Kedua - Penyegaran Prioritas Tinggi
**Target:** 4 unit dengan produktivitas tertekan
**Timeline:** Setelah Fase 1 selesai — Fase 2
**Fokus:** Peningkatan produktivitas dan pengalaman pengguna

**Unit Prioritas:**
1. Christy (kesesuaian perangkat dengan peran)
2. Hibab (mobilitas dan konektivitas)
3. Yohana (BSOD, ergonomi dan performa)
4. Devinta (multitasking dan audio)

**Strategi Interim (sebelum penggantian):**
- Yohana & Devinta: Upgrade RAM ke 16 GB
- Semua unit: Optimasi sistem dan pembersihan
- Christy & Hibab: Perbaikan periferal sementara

### Fase 3: Pemeliharaan dan Optimasi
**Target:** 3 unit yang dipertahankan/diperbaiki
**Timeline:** Berkelanjutan
**Fokus:** Pemeliharaan preventif dan optimasi performa

**Tindakan:**
- Wulan: Clean install OS dan upgrade RAM
- Robin: Monitoring performa dan upgrade opsional
- System Autocount: Pemantauan fungsi siaga

## Rekomendasi Spesifikasi Standar

### Untuk Desktop (Workstation Harian)
- **Prosesor:** Intel Core i5 gen 12+ atau setara
- **Memori:** 16 GB DDR4/DDR5 (minimum)
- **Penyimpanan:** 512 GB NVMe SSD (minimum)
- **Sistem Operasi:** Windows 11 Pro 64-bit
- **Grafis:** Integrated graphics memadai atau discrete card jika diperlukan
- **Monitor:** 24" Full HD (minimum)
- **Garansi:** 3 tahun onsite service

### Untuk Laptop (Business Grade)
- **Prosesor:** Intel Core i5 gen 12+ atau setara
- **Memori:** 16 GB DDR4/DDR5
- **Penyimpanan:** 512 GB NVMe SSD
- **Layar:** 14" Full HD (minimum)
- **Baterai:** 8+ jam daya tahan
- **Bobot:** <1.5 kg untuk ultrabook, <2 kg untuk standard
- **Konektivitas:** WiFi 6, Bluetooth 5+, port memadai
- **Fitur:** Webcam HD, mikrofon array, keyboard backlit
- **Garansi:** 3 tahun dengan accidental damage protection

### Untuk Laptop (Ultrabook/Mobility)
- **Prosesor:** Intel Core i5/i7 gen 12+ U-series
- **Memori:** 16 GB LPDDR5
- **Penyimpanan:** 1 TB NVMe SSD
- **Layar:** 13-14" Full HD/2K
- **Baterai:** 10+ jam daya tahan
- **Bobot:** <1.2 kg
- **Build Quality:** Aluminum/magnesium alloy
- **Garansi:** 3 tahun premium support

## Pertimbangan Implementasi

### 1. Sequencing Penggantian
Prioritaskan urutan berdasarkan:
- **Risiko Operasional:** Unit dengan BSOD/mati mendadak pertama
- **Dampak Bisnis:** Unit yang mengganggu aplikasi kritis
- **Jabatan dan Peran User:** Pengguna dengan jabatan lebih tinggi atau peran yang lebih kritis secara bisnis diprioritaskan lebih awal
- **Ketersediaan Pengguna:** Koordinasi dengan schedule kerja
- **Logistik:** Pengelompokan berdasarkan lokasi/tim

### 2. Manajemen Transisi
- **Communication Plan:** Informasi jelas ke pengguna tentang timeline dan proses
- **Data Migration:** Strategi backup dan transfer data yang aman
- **User Training:** Orientasi singkat untuk fitur perangkat baru
- **Support Readiness:** Tim IT siap untuk onboarding dan troubleshooting

### 3. Disposal Perangkat Lama
- **Data Sanitization:** Penghapusan data sensitif sesuai standar
- **Asset Retirement:** Update inventory dan depresiasi
- **Environmental Compliance:** Pembuangan/recycling sesuai regulasi
- **Value Recovery:** Potensi penjualan/pergantian trade-in

### 4. Success Metrics
- **Reduction in Incident Tickets:** Penurunan laporan masalah hardware
- **User Satisfaction:** Survey kepuasan pengguna pasca-implementasi
- **Productivity Gains:** Pengukuran waktu penyelesaian task
- **System Stability:** Penurunan kejadian BSOD/downtime

## Rekomendasi Tambahan

### 1. Standardisasi Pembelian
- Tetapkan spesifikasi minimum berdasarkan role
- Konsolidasi vendor untuk volume discount
- Implementasi lifecycle management (3-4 tahun untuk laptop, 4-5 tahun untuk desktop)

### 2. Preventive Maintenance Program
- Regular health check setiap 6 bulan
- Cleaning dan optimization berkala
- Proactive component replacement (battery, storage)

### 3. User Education
- Best practices untuk perawatan perangkat
- Optimalisasi penggunaan sistem
- Reporting procedure untuk issues

### 4. Continuous Monitoring
- Implementasi basic monitoring untuk health metrics
- Regular review kebutuhan spesifikasi berdasarkan evolving workload
- Annual assessment untuk refresh planning

## Kesimpulan Rekomendasi

Program peremajaan bertahap dengan fokus pada **5 unit risiko tertinggi** dalam batch pertama memberikan dampak maksimal dengan sumber daya terbatas. Pendekatan ini:

1. **Mengurangi risiko operasional** segera untuk unit paling kritis
2. **Meningkatkan produktivitas** untuk unit dengan gangguan signifikan
3. **Mengoptimalkan investasi** melalui phased implementation
4. **Meminimalkan disruption** dengan transisi terencana
5. **Membangun foundation** untuk standarisasi masa depan

> **Penutup:** Rekomendasi prioritas dalam dokumen ini disusun berdasarkan bukti teknis dan operasional yang objektif. Namun, **keputusan akhir** mengenai urutan dan timeline penggantian tetap berada di tangan manajemen. Faktor-faktor seperti **jabatan pengguna, peran kritis dalam operasional bisnis, dan kebijakan organisasi** dapat memengaruhi prioritas final. Dokumen ini diajukan sebagai **bahan pertimbangan dan saran** yang memerlukan **persetujuan dari pihak berwenang** sebelum implementasi.