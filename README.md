
# Eksplorasi Data Pariwisata Bali

## 1. Identitas Mahasiswa
- **Nama:** Fransiska Cerlis Oda
- **NIM:** 2501010235
- **Program Studi:** Informatika
- **Semester/Kelas:** 3 / F
- **Mata Kuliah:** Akuisisi dan Manajemen Data
- **Dosen Pengampu:** Dr. I Gede Totok Suryawan, S.Kom., M.T.

## 2. Deskripsi Proyek
Proyek ini bertujuan untuk melakukan akuisisi dan pengelolaan data pariwisata Bali melalui beberapa sumber data, yaitu data daya tarik wisata, data hasil scraping informasi wisata, dan data cuaca.
## 3. Sumber Data

| No. | Nama Dataset | Sumber | Link Sumber |
|:---:|---|---|---|
| 1 | Data Daya Tarik Wisata (DTW) | Dinas Pariwisata Provinsi Bali | [Klik di sini](https://disparda.baliprov.go.id/daya-tarik-wisata) |
| 2 | Data Wisata Badung | Dinas Pariwisata Provinsi Bali | [Klik di sini](https://disparda.baliprov.go.id/badung) |
| 3 | Data Informasi Wisata Bali | Direktori Pariwisata | [Klik di sini](https://www.direktoripariwisata.id/kawasan/prov/Bali) |
| 4 | Data Cuaca Bali | Open-Meteo Archive API | [Klik di sini](https://archive-api.open-meteo.com/v1/archive) |

**Metode pengumpulan data:**
1. Download data Excel.
2. Web scraping.
3. Pengambilan data melalui API.

**Keterangan:** Data dikumpulkan melalui proses pengunduhan, web scraping, dan pengambilan data menggunakan API. Selanjutnya data dibersihkan dan diolah menggunakan Python di Google Colab.

### A. Data Daya Tarik Wisata (DTW)
- **Instansi sumber:** Dinas Pariwisata Provinsi Bali.
- **Format sumber:** Excel.
- **Nama file:** `2024-DATA-DTW-update-sesuai-SK-1.xlsx`.
- **Pengolahan:** Data dibersihkan menggunakan Python dan Pandas.

### B. Data Informasi Wisata (Web Scraping)
Data dikumpulkan melalui proses scraping dari:
1. Dinas Pariwisata Provinsi Bali: https://disparda.baliprov.go.id/badung
2. Direktori Pariwisata: https://www.direktoripariwisata.id/kawasan/prov/Bali

### C. Data Cuaca (API)
- **Sumber:** Open-Meteo Archive API.
- **Alamat API:** https://archive-api.open-meteo.com/v1/archive
- **Periode data:** 1 Juli 2026 sampai 31 Oktober 2026.
- **Variabel:** Tanggal, suhu maksimum, suhu minimum, dan curah hujan.

## 4. Jumlah Data

| Dataset | Jumlah Data |
|---|---:|
| Data DTW setelah dibersihkan | 102 baris |
| Data hasil scraping | 238 baris |
| Data cuaca | 123 baris |
| Data gabungan (left join) | 102 baris |
| Nama wisata yang cocok | 24 data |

**Catatan:** Data gabungan menggunakan metode left join. Terdapat 24 nama wisata yang cocok berdasarkan pencocokan nama.

## 5. Struktur Folder

```text
data/
├── raw/
│   ├── api/
│   ├── download/
│   └── scraping/
└── processed/
    ├── data_wisata_gabungan_102.csv
    └── data_cuaca_bali.csv

notebooks/
└── uts_pariwisata_bali.ipynb
```

## 6. Proses Pengolahan Data
1. Mengunduh data DTW dari sumber instansi.
2. Mengambil data informasi wisata melalui web scraping.
3. Mengambil data cuaca melalui Open-Meteo Archive API.
4. Membersihkan data dari nilai kosong dan duplikasi.
5. Menggabungkan data DTW dengan data hasil scraping.
6. Menyimpan data mentah dan hasil pengolahan ke dalam folder yang sesuai.

## 7. Tools yang Digunakan
- Google Colab
- Python
- Pandas
- Requests
- BeautifulSoup
- GitHub

## 8. Kesimpulan
Proyek ini menghasilkan dataset pariwisata Bali dari beberapa sumber. Data dikumpulkan, dibersihkan, dan diolah untuk mendukung eksplorasi informasi pariwisata dan cuaca.
