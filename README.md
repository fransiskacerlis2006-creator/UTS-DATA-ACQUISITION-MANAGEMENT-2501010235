# UTS-DATA-ACQUISITION-MANAGEMENT-2501010235

## Identitas Mahasiswa

- **Nama:** Fransiska Cerlis Oda
- **Program Studi:** Informatika
- **Angkatan:** 2025
- **Semester:*3*

## Judul Proyek

Eksplorasi Data Pariwisata Bali: Destinasi Wisata, Informasi Cuaca, dan Data Daya Tarik Wisata

### 1. Deskripsi Proyek
Proyek ini bertujuan untuk melakukan pengumpulan, pembersihan, pengolahan, dan penggabungan data pariwisata Bali dari tiga sumber, yaitu Download, API, dan Web Scraping.

### 2. Sumber Data
- **Download:** Data Daya Tarik Wisata Bali tahun 2024 dari Dinas Pariwisata Provinsi Bali.
- **API:** Data cuaca Bali dari Open-Meteo Archive API.
- **Web Scraping:** Data nama tempat wisata dari halaman Kabupaten Badung pada website Dinas Pariwisata Provinsi Bali.

### 3. Hasil Pengumpulan Data
- Data Download: 102 baris.
- Data API: 31 baris.
- Data Web Scraping: 12 nama tempat wisata.

### 4. Proses Pengolahan Data
1. Mengumpulkan data dari tiga sumber.
2. Membersihkan data dan memeriksa nilai kosong serta duplikat.
3. Mengolah data menggunakan Python dan Pandas.
4. Menggabungkan data Download dan Web Scraping berdasarkan nama tempat wisata.
5. Membuat dokumentasi sumber data dan checklist etika data.

### 5. Hasil Penggabungan
Hasil penggabungan memperoleh 4 tempat wisata yang cocok, yaitu:
- Pantai Kuta
- Pantai Nusa Dua
- Pantai Pandawa
- Garuda Wisnu Kencana

### 6. Tools dan Library
- Google Colab
- Python
- Pandas
- NumPy
- Requests
- BeautifulSoup

### 7. Struktur Folder
- `Data/Raw/Download`
- `Data/Raw/API`
- `Data/Raw/Scraping`
- `Data/Processed`

### 8. File Notebook
Notebook utama: `UTS_Eksplorasi_Data_Pariwisata_Bali.ipynb`

### 9. Tujuan
Proyek ini dibuat untuk memenuhi tugas Ujian Tengah Semester mata kuliah Data Acquisition and Management.
