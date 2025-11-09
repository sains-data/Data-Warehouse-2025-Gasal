# 📊 Tugas Besar Pergudangan Data (SD25-31007)



**Institut Teknologi Sumatera – Program Studi Sains Data**  
**Mata Kuliah:** Pergudangan Data (3 SKS)  
**Tahun Ajaran:** 2025  
**Bobot Tugas Besar:** 30% dari nilai akhir  

---

## 🧭 Deskripsi Proyek

Tugas besar ini merupakan proyek **kelompok** untuk merancang, membangun, dan mengimplementasikan **Data Mart** sebagai bagian dari arsitektur *Data Warehouse* ITERA.  
Setiap kelompok bertanggung jawab atas satu domain/unit kerja, dan akan melewati **tiga misi utama**:

1. **Misi 1 – Desain Konseptual & Logikal**  
2. **Misi 2 – Desain Fisikal & Development**  
3. **Misi 3 – Implementasi Produksi & Dashboard BI**

---

## 🎯 Tujuan Pembelajaran

- Menerapkan konsep desain konseptual, logikal, dan fisikal gudang data.  
- Mengimplementasikan ETL dan Data Mart menggunakan SQL Server di Azure.  
- Membangun dashboard analitik dengan Power BI atau Tableau.  
- Menerapkan *best practices* pengembangan data warehouse.  
- Mengembangkan kolaborasi tim dan dokumentasi profesional.

---

## 🧩 Teknologi & Tools

| Kategori | Teknologi |
|-----------|------------|
| **Database Platform** | SQL Server 2019 on Azure VM |
| **ETL Tools** | SQL Server Integration Services (SSIS) |
| **BI Tools** | Power BI Desktop / Tableau |
| **Modeling** | Draw.io, ERDPlus, Lucidchart |
| **Version Control** | GitHub (repository kelompok) |
| **Documentation** | Markdown (`README.md`), LaTeX (report) |

---

## 🧱 Arsitektur

Pendekatan utama: **Kimball Dimensional Modeling**

```

Fact Table     → menyimpan data transaksi atau metrik bisnis
Dimension Table → menyimpan atribut deskriptif (Who, What, Where, When, Why)
Star Schema     → Fact di pusat dikelilingi oleh Dimensi

````

---

## 🧮 Struktur Repository

```plaintext
├── README.md
├── docs/
│   ├── 01-requirements/
│   │   ├── business-requirements.md
│   │   └── data-sources.md
│   ├── 02-design/
│   │   ├── ERD.png
│   │   ├── dimensional-model.png
│   │   └── data-dictionary.xlsx
│   ├── 03-implementation/
│   │   ├── etl-documentation.md
│   │   ├── user-manual.pdf
│   │   └── operations-manual.pdf
│   └── presentations/
├── sql/
│   ├── 01_Create_Database.sql
│   ├── 02_Create_Dimensions.sql
│   ├── 03_Create_Facts.sql
│   ├── 04_Create_Indexes.sql
│   ├── 05_Create_Partitions.sql
│   └── 06_Create_Staging.sql
├── etl/
│   ├── packages/
│   └── scripts/
├── dashboards/
│   └── PowerBI files
└── tests/
    └── test scripts
````

---

## 🧠 Misi Proyek

### 🚀 MISI 1 – Desain Konseptual & Logikal

* Analisis kebutuhan bisnis dan KPI
* Identifikasi sumber data (OLTP, Excel, API)
* Desain ERD & model dimensional
* Buat Data Dictionary
* Siapkan repository GitHub dan dokumentasi

**Deliverables:** Business Requirements, ERD, Dimensional Model, Data Dictionary, README.md

---

### ⚙️ MISI 2 – Desain Fisikal & Development

* Implementasi schema ke SQL Server
* Pengembangan ETL (SSIS/T-SQL)
* Optimasi dengan indexing & partitioning
* Validasi kualitas data dan performa

**Deliverables:** SQL scripts, ETL packages, Data Quality Report, Performance Test Report

---

### 🏁 MISI 3 – Implementasi Produksi

* Deployment database di Azure VM
* Pengembangan dashboard Power BI
* Implementasi keamanan (RBAC, data masking)
* UAT (User Acceptance Testing)
* Final documentation & presentation

**Deliverables:** Production DB, Dashboard, Security Scripts, UAT Report, Final Presentation

---

## 📊 Contoh KPI

| Domain      | KPI Utama                                                |
| ----------- | -------------------------------------------------------- |
| Akademik    | Jumlah Mahasiswa Aktif, Rata-rata IPK, Tingkat Kelulusan |
| Keuangan    | Total Pemasukan, Rata-rata Pembayaran, Piutang Aktif     |
| Kepegawaian | Rasio Dosen:Mahasiswa, Produktivitas Penelitian          |
| Sarpras     | Pemanfaatan Ruangan, Jadwal Maintenance                  |

---

## 👥 Konvensi GitHub

### Branching

* `main` → production-ready
* `develop` → integrasi antar fitur
* `feature/[name]` → pengembangan fitur

### Commit Message

```
Add: Fact_Enrollment table  
Fix: ETL null handling issue  
Docs: Add data dictionary
```

### .gitignore

```
*.mdf
*.ldf
*.bak
*.pbix.tmp
**/bin/
**/obj/
**/config/
```

---

## 📆 Timeline Proyek

| Misi   | Kegiatan Utama         | Estimasi Waktu |
| ------ | ---------------------- | -------------- |
| Misi 1 | Analisis & Desain      | Minggu 1   |
| Misi 2 | Development & ETL      | Minggu 2   |
| Misi 3 | Deployment & Dashboard | Minggu 3 |

---

## 👥 Tim Pengembang

| NIM       | Nama   | Role               | Email                                         |
| --------- | ------ | ------------------ | --------------------------------------------- |
| 12xxxxxxx | Nama 1 | Project Lead / DBA | [email@example.com](mailto:email@example.com) |
| 12xxxxxxx | Nama 2 | ETL Developer      | [email@example.com](mailto:email@example.com) |
| 12xxxxxxx | Nama 3 | BI Developer       | [email@example.com](mailto:email@example.com) |
| 12xxxxxxx | Nama 4 | QA & Documentation | [email@example.com](mailto:email@example.com) |

---

## 📜 Lisensi

Repositori ini dikembangkan untuk keperluan akademik mata kuliah
**Pergudangan Data (SD25-31007)** – Program Studi Sains Data, Fakultas Sains, Institut Teknologi Sumatera.

---

> *“Turning raw data into actionable insight — through collaboration, modeling, and analytics.”*
> **Kelompok Tugas Besar Pergudangan Data 2025**

