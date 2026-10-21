# Tugas Citra Digital

Tugas pemrosesan citra digital menggunakan Python dengan Library **NumPy**, **Pandas**,
**Pillow**, dan **Matplotlib**. Analisis dilakukan pada citra `JKW.jfif` untuk
mengidentifikasi format berkas, mode warna, dimensi, bentuk array, serta memverifikasi
kecocokan nilai piksel yang dibaca Pillow dengan nilai piksel pada array NumPy.

## Hasil Analisis

| Aspek                | Hasil                                   |
| -------------------- | --------------------------------------- |
| Nama berkas         | `JKW.jfif`                              |
| Format terdeteksi   | JPEG                                    |
| Mode warna asli     | RGB (3 kanal: R, G, B)                  |
| Dimensi citra       | 552 × 775 piksel (lebar × tinggi)      |
| Total piksel        | 427.800                                 |
| Bentuk array         | `(775, 552, 3)`                         |
| Tipe data            | `uint8`                                 |
| Rentang nilai       | 0 – 255                                 |
| Verifikasi piksel   | VALID (Pillow = NumPy pada semua titik) |

Visualisasi pada notebook mencakup citra asli, pemisahan kanal R/G/B, serta representasi
grayscale (mode `L`).

## Struktur Berkas

```
.
├── .gitignore
├── README.md
├── requirements.txt
├── Tugas_Citra_Digital.ipynb   # notebook analisis (lengkap dengan output)
└── data/
    └── JKW.jfif                 # citra sumber
```

## Cara Menjalankan

### Google Colab

1. Unggah `Tugas_Citra_Digital.ipynb` ke Google Colab.
2. Hubungkan Google Drive, lalu jalankan sel berikut untuk menyalin citra sumber:

   ```python
   !cp "/content/drive/MyDrive/citra digital/JKW.jfif" /content/JKW.jfif
   ```

3. Jalankan seluruh sel (`Runtime > Run all`).

Notebook mencari `JKW.jfif` secara otomatis pada lokasi berikut:

- `/content/drive/MyDrive/citra digital/JKW.jfif` (Google Colab)
- `data/JKW.jfif` (lokal, relatif terhadap folder notebook)
- `JKW.jfif` (lokal, folder kerja)

### Jupyter Notebook (lokal)

```bash
pip install -r requirements.txt
jupyter notebook
```

Buka `Tugas_Citra_Digital.ipynb` lalu jalankan seluruh sel.

## Teknologi

- Python 3
- NumPy
- Pandas
- Pillow
- Matplotlib
- Jupyter Notebook

## Penulis

Wildan — [okewildan647-dev](https://github.com/okewildan647-dev)
