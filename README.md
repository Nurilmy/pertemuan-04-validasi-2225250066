# Pertemuan 04 - Validasi dan Klasifikasi Python

## Identitas

- Nama: Nuril Ilmy
- NIM: 2225250066
- Kelas: 3E

## Tujuan

Tugas ini bertujuan untuk memahami:

1. Percabangan if, elif, dan else.
2. Validasi tipe data menggunakan try-except.
3. Validasi rentang nilai.
4. Klasifikasi data berdasarkan kondisi.
5. Pengujian program menggunakan beberapa kasus uji.

## Struktur Folder

```text
pertemuan-04-validasi-2225250066/
├── README.md
├── .gitignore
├── latihan/
│   ├── 01_predikat_nilai.py
│   ├── 02_kategori_bilangan.py
│   ├── 03_validasi_rentang.py
│   ├── 04_validasi_tipe.py
│   └── 05_klasifikasi_segitiga_sudut.py
└── praktik/
    └── validasi_klasifikasi_nilai.py
```

## Cara Menjalankan Program

Jalankan program melalui terminal VS Code:

```bash
python latihan/01_predikat_nilai.py
python latihan/02_kategori_bilangan.py
python latihan/03_validasi_rentang.py
python latihan/04_validasi_tipe.py
python latihan/05_klasifikasi_segitiga_sudut.py
python praktik/validasi_klasifikasi_nilai.py
```

## Ringkasan Latihan

### Latihan 1 - Predikat Nilai

Program menentukan predikat nilai berdasarkan ketentuan:

| Rentang Nilai | Predikat |
|---|---|
| >= 85 | A |
| >= 70 | B |
| >= 60 | C |
| >= 50 | D |
| < 50 | E |

### Latihan 2 - Kategori Bilangan

Program mengklasifikasikan bilangan menjadi:

- Bilangan negatif.
- Bilangan nol.
- Bilangan positif genap.
- Bilangan positif ganjil.

### Latihan 3 - Validasi Rentang

Program memeriksa besar sudut dan mengklasifikasikannya menjadi:

- Sudut lancip.
- Sudut siku-siku.
- Sudut tumpul.

### Latihan 4 - Validasi Tipe

Program menerima jumlah jawaban benar dari 20 soal.

Program memeriksa:

- Input berupa bilangan bulat.
- Nilai berada pada rentang 0 sampai 20.
- Persentase nilai.
- Status tuntas atau belum tuntas.

Batas ketuntasan adalah 75%.

### Latihan 5 - Klasifikasi Segitiga Berdasarkan Sudut

Program memeriksa:

- Setiap sudut harus lebih dari 0.
- Jumlah ketiga sudut harus 180 derajat.
- Klasifikasi berdasarkan sudut terbesar.

## Praktik 1 - Validasi dan Klasifikasi Nilai

Input yang digunakan:

1. Nilai ujian.
2. Nilai tugas.
3. Persentase kehadiran.

Rumus nilai akhir:

```text
Nilai akhir = (0.6 x nilai ujian) + (0.4 x nilai tugas)
```

Ketentuan:

- Semua input harus berupa angka.
- Nilai ujian berada pada rentang 0 sampai 100.
- Nilai tugas berada pada rentang 0 sampai 100.
- Persentase kehadiran berada pada rentang 0 sampai 100.
- Kehadiran di bawah 80% tidak memenuhi syarat.
- Predikat A, B, dan C dinyatakan Lulus.
- Predikat D dan E dinyatakan Belum lulus.

## Tabel Pengujian Praktik 1

| No | Ujian | Tugas | Kehadiran | Hasil |
|---|---:|---:|---:|---|
| 1 | 90 | 80 | 95 | 86.00, A, Lulus |
| 2 | 75 | 70 | 85 | 73.00, B, Lulus |
| 3 | 60 | 60 | 80 | 60.00, C, Lulus |
| 4 | 55 | 50 | 90 | 53.00, D, Belum lulus |
| 5 | 40 | 30 | 100 | 36.00, E, Belum lulus |
| 6 | 90 | 90 | 75 | Tidak memenuhi syarat kehadiran |
| 7 | 105 | 80 | 90 | Nilai ujian di luar rentang |
| 8 | 80 | -5 | 90 | Nilai tugas di luar rentang |
| 9 | 80 | 80 | abc | Input harus berupa angka |

## Refleksi

1. Validasi tipe data digunakan agar program tidak berhenti ketika input salah.
2. Validasi rentang digunakan agar data sesuai dengan ketentuan.
3. Percabangan if-elif-else digunakan untuk memilih hasil berdasarkan kondisi.
4. Pengujian dilakukan menggunakan data normal, batas, dan data tidak valid.

## Contoh Commit Git

```bash
git add latihan
git commit -m "feat: menyelesaikan lima latihan validasi dan klasifikasi"

git add praktik/validasi_klasifikasi_nilai.py
git commit -m "feat: menyelesaikan praktik 1 validasi dan klasifikasi"

git add README.md .gitignore
git commit -m "docs: menambahkan README dan gitignore"

git push
```
