
# Eksplorasi Data Pariwisata Bali

## Deskripsi
Proyek ini mengumpulkan dan mengolah data pariwisata Bali dari tiga sumber:
1. Data DTW dari file Excel.
2. Data cuaca dari Open-Meteo API.
3. Data wisata melalui teknik web scraping.

## Jumlah Data
- Data DTW: 102 baris.
- Data scraping: 238 baris.
- Data cuaca: 123 baris.
- Data gabungan DTW dan scraping: 102 baris.
- Nama DTW yang cocok pada proses penggabungan: 24.

## Struktur Folder
- data/raw/download: data Excel asli.
- data/raw/api: data JSON dari API.
- data/raw/scraping: data hasil scraping.
- data/processed: data yang sudah diolah.

## Pengolahan Data
Data diperiksa untuk mengetahui data kosong dan duplikat.
Penggabungan DTW dan scraping menggunakan metode left join.

## Sumber Data
- Data DTW: Dinas Pariwisata Provinsi Bali.
- Data cuaca: Open-Meteo Archive API.
- Data scraping: sumber informasi pariwisata Bali.
