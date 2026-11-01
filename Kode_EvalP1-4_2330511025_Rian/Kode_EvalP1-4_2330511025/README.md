# simuteh-2330511025
SIMUTEH: Sistem Pemeriksaan Mutu Daun Teh Berbasis Citra (Evaluasi Praktikum P1-P4 Computer Vision, UMMI).

- Nama: Rian | NIM: 2330511025 | **SEED: 1025** (4 digit terakhir NIM)

## Cara menjalankan
1. `pip install -r requirements.txt`
2. Buka notebook dari folder `notebook/` dan jalankan berurutan (*Restart & Run All*): `B1_lingkungan` (membuat dataset), `B2_citra_warna`, `B3_histogram`, `B4_penapisan`, `B5_praproses`.
3. Dataset dibuat oleh `python src/buat_dataset_sintetis.py` (dijalankan dari folder utama; sudah dipanggil di B1). Folder `data/` tidak perlu di-commit.

## Ringkasan hasil
- Kanal terbaik: R (KB tertinggi di kelima kondisi cahaya).
- Praproses final (`hasil/param_praproses.json`): CLAHE kanal V clip 1,0 tile 8, median 3x3, tanpa gamma dan tanpa penajaman.
- KB rata-rata pada 40 citra berbercak naik dari 6,67 menjadi 10,47; naik di semua kondisi cahaya.
- Uji bercak palsu pada 20 citra sehat: simpangan baku daun turun di semua kondisi.

Tag: `v0.1-praproses`
