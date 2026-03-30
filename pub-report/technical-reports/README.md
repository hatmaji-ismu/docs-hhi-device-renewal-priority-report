# Technical Reports

Folder ini berisi laporan teknis lengkap untuk setiap unit perangkat yang dievaluasi dalam program peremajaan hardware. Laporan-laporan ini merupakan dasar analisis untuk rekomendasi prioritas penggantian perangkat.

## Daftar Laporan Teknis

| File | Unit | Tipe Perangkat | Prioritas |
| :--- | :--- | :--- | :--- |
| [system-finance.md](system-finance.md) | System Finance | Desktop | Penggantian Segera |
| [renaldi.md](renaldi.md) | Renaldi | Desktop | Penggantian Segera |
| [diana.md](diana.md) | Diana | Desktop | Penggantian Segera |
| [regina.md](regina.md) | Regina | Laptop | Penggantian Segera |
| [syela.md](syela.md) | Syela | Desktop | Penggantian Segera |
| [christy.md](christy.md) | Christy | Laptop | Penyegaran Prioritas Tinggi |
| [yohana.md](yohana.md) | Yohana | Desktop | Penyegaran Prioritas Tinggi |
| [hibab.md](hibab.md) | Hibab | Laptop | Penyegaran Prioritas Tinggi |
| [devinta.md](devinta.md) | Devinta | Desktop | Penyegaran Prioritas Tinggi |
| [wulan.md](wulan.md) | Wulan | Desktop | Perbaikan/Upgrade Terlebih Dahulu |
| [robin.md](robin.md) | Robin | Desktop | Pertahankan |
| [system-autocount.md](system-autocount.md) | System Autocount | Desktop | Pertahankan |

## Format Laporan

Setiap laporan teknis berisi informasi berikut:

### 1. Informasi Dasar
- Nama pengguna dan departemen
- Tipe perangkat (desktop/laptop)
- Tanggal assessment

### 2. Spesifikasi Teknis
- **Prosesor:** Model, generasi, kecepatan
- **Memori:** Kapasitas, tipe, utilisasi
- **Penyimpanan:** Tipe media, kapasitas, health status
- **Grafis:** GPU terintegrasi/diskrit
- **Sistem Operasi:** Versi, arsitektur

### 3. Metrik Performa Sistem
- **Utilisasi RAM:** Persentase penggunaan memori
- **Page File Usage:** Penggunaan virtual memory
- **Storage Health:** Persentase kesehatan media penyimpanan
- **Suhu Sistem:** Temperatur operasional komponen
- **Ruang Kosong:** Available space pada drive sistem

### 4. Status Komponen
- **CPU Status:** Healthy/Warning/Critical
- **GPU Status:** Healthy/Warning/Critical
- **Memory Status:** Healthy/Warning/Critical
- **Storage Status:** Healthy/Warning/Critical

### 5. Temuan dan Analisis
- Masalah teknis yang teridentifikasi
- Analisis akar penyebab
- Dampak terhadap performa sistem
- Rekomendasi teknis

### 6. Bukti Pendukung
- Screenshot DxDiag
- Tangkapan layar system metrics
- Catatan insiden (BSOD, crash, dll.)

## Penggunaan

Laporan-laporan ini digunakan untuk:
1. **Analisis Kondisi Aktual:** Memahami state teknis setiap perangkat
2. **Penentuan Prioritas:** Dasar untuk klasifikasi urgensi penggantian
3. **Perencanaan Teknis:** Informasi untuk spesifikasi perangkat pengganti
4. **Documentation:** Catatan historis kondisi aset TI

## Sumber Data

Laporan teknis dikumpulkan dari:
- **DxDiag Reports:** Informasi sistem Windows
- **Hardware Monitoring Tools:** Software untuk tracking health komponen
- **Manual Inspection:** Pemeriksaan fisik perangkat
- **System Logs:** Catatan error dan performance issues

## Keterkaitan dengan Laporan Utama

Informasi dalam laporan teknis ini disintesis menjadi:
- **Tabel Sintesis Prioritas** di [05-analysis-results.md](../05-analysis-results.md)
- **Analisis Detail Per Unit** di [08-appendices.md](../08-appendices.md)
- **Rekomendasi Tindakan Spesifik** di [06-renewal-priority-recommendation.md](../06-renewal-priority-recommendation.md)

## Update dan Maintenance

Laporan teknis ini merupakan snapshot kondisi pada waktu assessment. Untuk assessment berkala di masa depan:
1. Gunakan template yang sama untuk konsistensi
2. Catat tanggal assessment secara jelas
3. Simpan bukti pendukung (screenshot, logs)
4. Update prioritas berdasarkan perubahan kondisi

---

*Folder ini merupakan bagian dari Laporan Prioritas Peremajaan Perangkat HHI. Lihat [README utama](../README.md) untuk informasi lebih lanjut tentang struktur dokumen.*