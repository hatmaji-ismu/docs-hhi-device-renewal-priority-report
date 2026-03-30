# HHI Hardware Assessment Project

Project ini berisi dokumentasi dan analisis komprehensif untuk program penilaian dan peremajaan perangkat hardware (Device Health Index - HHI) organisasi.

## Overview

Project ini bertujuan untuk:
1. **Menilai kondisi teknis** 12 unit perangkat yang saat ini digunakan
2. **Menganalisis dampak operasional** terhadap produktivitas pengguna
3. **Menyusun rekomendasi prioritas** penggantian perangkat
4. **Menyediakan dasar keputusan** untuk program hardware refresh

## Struktur Folder

```
hhi-hardware-assessment/
├── README.md                          # Dokumen ini
├── .gitignore                         # File ignore untuk Git
├── raw-hardware-assessment-reports/    # Data assessment per unit
│   ├── System Finance/                # Assessment System Finance
│   │   └── System_Finance_Hardware_Report.md
│   ├── Renaldi/                       # Assessment Renaldi
│   │   └── Renaldi_Hardware_Report.md
│   ├── Diana/                         # Assessment Diana
│   │   └── Diana_Hardware_Report.md
│   ├── Regina/                        # Assessment Regina
│   │   └── Regina_Hardware_Report.md
│   ├── Syela/                         # Assessment Syela
│   │   └── Syela_Hardware_Report.md
│   ├── Christy/                       # Assessment Christy
│   │   └── Christy_Hardware_Report.md
│   ├── Yohana/                        # Assessment Yohana
│   │   └── Yohana_Hardware_Report.md
│   ├── Hibab/                         # Assessment Hibab
│   │   └── Hibab_Hardware_Report.md
│   ├── Devinta/                       # Assessment Devinta
│   │   └── Devinta_Hardware_Report.md
│   ├── Wulan/                         # Assessment Wulan
│   │   └── Wulan_Hardware_Report.md
│   ├── Robin/                         # Assessment Robin
│   │   └── Robin_Hardware_Report.md
│   └── System Autocount/              # Assessment System Autocount
│       └── System_Autocount_Hardware_Report.md
├── stag-report-drafts/                # Draft laporan
│   └── comprehensive-report-v0.4.md   # Draft laporan komprehensif
├── pub-report/                        # Laporan final published
│   ├── README.md                      # Panduan laporan
│   ├── 01-cover-page.md               # Halaman sampul
│   ├── 02-executive-summary.md        # Ringkasan eksekutif
│   ├── 03-background.md               # Latar belakang
│   ├── 04-assessment-methodology.md   # Metodologi assessment
│   ├── 05-analysis-results.md         # Hasil analisis
│   ├── 06-renewal-priority-recommendation.md # Rekomendasi prioritas
│   ├── 07-conclusion-management-summary.md   # Kesimpulan manajemen
│   ├── 08-appendices.md               # Lampiran
│   └── technical-reports/             # Laporan teknis lengkap
│       ├── README.md                  # Dokumentasi laporan teknis
│       ├── system-finance.md          # Laporan System Finance
│       ├── renaldi.md                 # Laporan Renaldi
│       ├── diana.md                   # Laporan Diana
│       ├── regina.md                  # Laporan Regina
│       ├── syela.md                   # Laporan Syela
│       ├── christy.md                 # Laporan Christy
│       ├── yohana.md                  # Laporan Yohana
│       ├── hibab.md                   # Laporan Hibab
│       ├── devinta.md                 # Laporan Devinta
│       ├── wulan.md                   # Laporan Wulan
│       ├── robin.md                   # Laporan Robin
│       └── system-autocount.md        # Laporan System Autocount
└── __notebook__/                      # Notebook untuk analisis data
```

## Konvensi Penamaan Folder

Project ini menggunakan konvensi penamaan folder yang konsisten:

### 1. **Raw Data Folders** (prefix `raw-`)
Folder dengan prefix `raw-` berisi data mentah/asli yang belum diproses:
- `raw-hardware-assessment-reports/` - Data assessment teknis original
- Format: `raw-` + `deskripsi-konten` (kebab-case)

### 2. **Staging/Intermediate Data** (prefix `stag-`)
Folder dengan prefix `stag-` berisi data intermediate/staging yang sedang dalam proses:
- `stag-report-drafts/` - Draft laporan dalam berbagai versi
- Format: `stag-` + `deskripsi-konten` (kebab-case)

### 3. **Published/Final Data** (prefix `pub-`)
Folder dengan prefix `pub-` berisi data final yang sudah siap dipublikasikan/digunakan:
- `pub-report/` - Laporan final terstruktur siap review
- Format: `pub-` + `deskripsi-konten` (kebab-case)

### 3. **Working/Experimental**
Folder dengan special naming:
- `__notebook__/` - Untuk analisis data dan eksperimen
- Format: `__nama__` (double underscore) untuk working folders

### 4. **Kebab-case Convention**
Semua nama folder menggunakan **kebab-case** (huruf kecil, dipisah dash):
- ✅ `raw-hardware-assessment-reports`
- ✅ `pub-report`
- ✅ `technical-reports`
- ❌ `Raw Hardware Assessment Reports`
- ❌ `report_per_bab`
- ❌ `technicalReports`
- **Laporan hardware** berisi spesifikasi teknis, health status, dan temuan
- **Data DxDiag** dan system metrics
- **Bukti teknis** untuk analisis kondisi

**12 Unit yang Dievaluasi:**
- System Finance, Renaldi, Diana, Regina, Syela, Christy
- Yohana, Hibab, Devinta, Wulan, Robin, System Autocount

### 2. `stag-report-drafts/`
Berisi draft awal laporan komprehensif:
- `comprehensive-report-v0.4.md` - Draft sintesis dari 12 laporan teknis + penilaian kualitatif

### 3. `pub-report/`
**Laporan final** yang siap untuk management review, terstruktur dalam 8 bagian:
- **01-08**: Bagian utama laporan dari cover page hingga appendices
- `technical-reports/`: Laporan teknis lengkap untuk referensi detail

### 4. `__notebook__/`
Folder untuk analisis data dan eksperimen (jika ada)

## Alur Kerja Project

### Phase 1: Data Collection
```
raw-hardware-assessment-reports/ → Technical Assessment → 12 laporan teknis per unit
```

### Phase 2: Analysis & Synthesis
```
12 laporan teknis + qualitative assessment → stag-report-drafts/comprehensive-report-v0.4.md
```

### Phase 3: Report Structuring
```
Draft laporan → Template struktur (dalam stag-report-drafts/)
```

### Phase 4: Final Report Preparation
```
Template + Data → pub-report/ (8 bagian laporan final)
```

### Phase 5: Technical Documentation
```
Laporan teknis asli → pub-report/technical-reports/ (referensi lengkap)
```

## Cara Menggunakan Project

### Untuk Technical Team:
1. **Data Assessment:** Lihat folder `raw-hardware-assessment-reports/` untuk data teknis per unit
2. **Technical Reports:** Akses `pub-report/technical-reports/` untuk laporan lengkap
3. **Methodology:** Baca `pub-report/04-assessment-methodology.md`

### Untuk Management/Decision Makers:
1. **Executive Summary:** Baca `pub-report/02-executive-summary.md`
2. **Priority Recommendations:** Lihat `pub-report/06-renewal-priority-recommendation.md`
3. **Management Summary:** Review `pub-report/07-conclusion-management-summary.md`

### Untuk Report Writers:
1. **Structure Reference:** Gunakan template di `stag-report-drafts/` sebagai referensi
2. **Draft Content:** Lihat `stag-report-drafts/comprehensive-report-v0.4.md` untuk konten
3. **Final Output:** Folder `pub-report/` sebagai model format final

## Status Project

### ✅ Selesai:
- [x] Data collection untuk 12 unit
- [x] Technical assessment reports
- [x] Draft laporan komprehensif (v0.4)
- [x] Final report structure
- [x] Laporan final per bab
- [x] Technical reports documentation

### 📋 Dalam Progress:
- [ ] Management review dan approval
- [ ] Implementation planning berdasarkan rekomendasi
- [ ] Monitoring dan evaluation framework

## Data dan Metodologi

### Sumber Data:
1. **Technical Data:** DxDiag reports, system metrics, hardware inspection
2. **Operational Data:** User feedback, qualitative assessment, incident reports
3. **Synthesis:** Analisis komparatif dari 12 unit

### Metodologi Assessment:
- **Two-layer approach:** Technical evidence + Operational impact
- **Priority Classification:** 4 kategori (Replace Immediately, High Priority Refresh, Repair/Upgrade First, Maintain)
- **Risk-based Decision Making:** Business impact analysis

### Unit yang Dievaluasi:
- **8 Desktop:** System Finance, Renaldi, Diana, Syela, Yohana, Devinta, Wulan, Robin, System Autocount
- **4 Laptop:** Regina, Christy, Hibab

## Kontribusi

### Cara Berkontribusi:
1. **Data Update:** Update laporan teknis di `raw-hardware-assessment-reports/`
2. **Report Revision:** Edit file di `pub-report/`
3. **Draft Improvement:** Update file di `stag-report-drafts/`
4. **Analysis Enhancement:** Work di `__notebook__/`

### Version Control:
- Gunakan Git untuk tracking changes
- Commit message yang deskriptif
- Branch untuk major revisions

## Lisensi dan Hak Cipta

Project ini merupakan dokumentasi internal organisasi. Hak cipta dan konten merupakan properti organisasi.

## Changelog

### Refactoring 28 Maret 2026
- **Folder rename:** `HHI Assestment/` → `raw-hardware-assessment-reports/`
- **Folder rename:** `report-draft/` → `stag-report-drafts/`
- **Folder rename:** `report-per-bab/` → `pub-report/`
- **Folder deleted:** `report/` (empty folder)
- **Rationale:**
  - Prefix `raw-` menandakan data mentah/original
  - Prefix `stag-` menandakan data staging/intermediate
  - Prefix `pub-` menandakan data final/published
  - Kebab-case untuk konsistensi penamaan
- **Impact:** Semua referensi dalam dokumen telah diupdate secara otomatis
- **Files updated:** 50+ file markdown dengan referensi ke folder lama