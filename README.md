# Dataset-Narkotika_119_277

> Kumpulan putusan Pengadilan Negeri Gorontalo perkara **Narkotika** (Pidana Khusus), tahun 2023–2025, untuk riset dan praktikum **Temu Kembali Informasi (Information Retrieval)**.

![Format](https://img.shields.io/badge/format-PDF%20%2B%20XLSX-blue)
![Domain](https://img.shields.io/badge/domain-hukum-8a2be2)
![Bahasa](https://img.shields.io/badge/bahasa-Indonesia-red)
![Dokumen](https://img.shields.io/badge/dokumen-52%20PDF-green)

---

## Daftar Isi

1. [Tentang Dataset](#tentang-dataset)
2. [Sumber Data](#sumber-data)
3. [Kriteria Pengumpulan](#kriteria-pengumpulan)
4. [Struktur Repository](#struktur-repository)
5. [Isi Overview.xlsx](#isi-overviewxlsx)
6. [Penamaan File PDF](#penamaan-file-pdf)
7. [Cara Memakai](#cara-memakai)
8. [Contoh Kegunaan](#contoh-kegunaan)
9. [Anatomi Putusan Narkotika](#anatomi-putusan-narkotika)
10. [Etika dan Legalitas](#etika-dan-legalitas)
11. [Tim](#tim)

---

## Tentang Dataset

Putusan pengadilan adalah teks hukum yang panjang, formal, dan punya pola kalimat yang berulang. Sifat ini membuatnya cocok sebagai korpus untuk Temu Kembali Informasi: ada struktur yang bisa diekstraksi, kosakata yang khas, dan kebutuhan pencarian yang nyata (misalnya mencari putusan dengan barang bukti tertentu atau pidana tertentu).

Dataset ini berisi **52 berkas PDF** (`51` nomor perkara unik, dengan `1` perkara terduplikasi) yang seluruhnya berbasis teks (_searchable text_, total `1.397` halaman), ditambah satu berkas ringkasan `Overview.xlsx` yang memuat metadata dan dua bagian inti tiap putusan: **barang bukti** dan **amar putusan**.

| Item             | Keterangan                                                                      |
| ---------------- | ------------------------------------------------------------------------------- |
| Jumlah dokumen   | 52 berkas PDF (`51` perkara unik; `1` duplikasi pada `152/Pid.Sus/2023/PN Gto`) |
| Total halaman    | 1.397 halaman (`15`–`59` halaman/dokumen, rata-rata `26,87` halaman)            |
| Format dokumen   | PDF (`9.125.065` byte dalam arsip ZIP; `10.560.228` byte tidak terkompresi)     |
| Format ringkasan | XLSX (`Overview.xlsx`, `26.703` byte, `52` baris data × `5` kolom)              |
| Pengadilan       | PN Gorontalo (Pengadilan Negeri Gorontalo)                                      |
| Kategori         | Pidana Khusus (`Pid.Sus`), Narkotika                                            |
| Rentang tahun    | 2023–2025 (`2023`: 15 berkas/14 unik, `2024`: 9 berkas, `2025`: 28 berkas)      |
| Bahasa           | Indonesia                                                                       |

## Sumber Data

Seluruh putusan diunduh dari **Direktori Putusan Mahkamah Agung Republik Indonesia**:

- Portal: https://putusan3.mahkamahagung.go.id/direktori.html (tercantum pula `putusan.mahkamahagung.go.id` pada dokumen)
- Jalur penelusuran: Direktori → Pidana Khusus → Narkotika dan Psikotropika → PN Gorontalo → filter tahun (`2023`, `2024`, `2025`)

Pengunduhan dilakukan secara tertib pada tanggal 7 November 2026 (rentang timestamp `22:16:48`–`22:26:11`) agar tidak membebani server.

## Kriteria Pengumpulan

Dokumen dipilih dengan aturan berikut:

1. Berasal dari direktori **Pidana Khusus (`Pid.Sus`)** perkara narkotika.
2. Berasal dari **satu pengadilan negeri saja**, yaitu **PN Gorontalo**.
3. Berasal dari tahun putusan **2023, 2024, dan 2025**.
4. Berekstensi `.pdf` dan dapat dibaca langsung (seluruh 52 berkas merupakan PDF berbasis teks yang dapat diekstraksi).

## Struktur Repository

```text
Dataset-Narkotika_119_277/
├── Dataset/
│   └── Narkotika.zip        # 52 berkas putusan PN Gorontalo (*.pdf), 9.125.065 byte
├── Overview/
│   └── Overview.xlsx        # ringkasan 52 putusan (1 sheet: Overview), 26.703 byte
└── README.md
```

<details>
<summary>Daftar lengkap 52 berkas PDF di dalam <code>Dataset/Narkotika.zip</code></summary>

| No  | Nama File                                            | Ukuran (Byte) |
| :-: | :--------------------------------------------------- | ------------: |
|  1  | `putusan_10_pid.sus_2025_pn_gto_20261107222325.pdf`  |       250.268 |
|  2  | `putusan_12_pid.sus_2025_pn_gto_20261107222330.pdf`  |       268.100 |
|  3  | `putusan_14_pid.sus_2025_pn_gto_20261107222300.pdf`  |       273.883 |
|  4  | `putusan_16_pid.sus_2025_pn_gto_20261107222305.pdf`  |       165.722 |
|  5  | `putusan_17_pid.sus_2025_pn_gto_20261107222315.pdf`  |       165.405 |
|  6  | `putusan_24_pid.sus_2025_pn_gto_20261107222337.pdf`  |       229.733 |
|  7  | `putusan_34_pid.sus_2025_pn_gto_20261107222320.pdf`  |       203.201 |
|  8  | `putusan_39_pid.sus_2025_pn_gto_20261107222310.pdf`  |       186.087 |
|  9  | `putusan_43_pid.sus_2025_pn_gto_20261107222359.pdf`  |       189.566 |
| 10  | `putusan_44_pid.sus_2025_pn_gto_20261107222347.pdf`  |       144.166 |
| 11  | `putusan_45_pid.sus_2025_pn_gto_20261107222354.pdf`  |       551.415 |
| 12  | `putusan_46_pid.sus_2025_pn_gto_20261107222342.pdf`  |       155.324 |
| 13  | `putusan_54_pid.sus_2025_pn_gto_20261107222502.pdf`  |       218.092 |
| 14  | `putusan_55_pid.sus_2025_pn_gto_20261107222514.pdf`  |       183.136 |
| 15  | `putusan_57_pid.sus_2023_pn_gto_20261107221823.pdf`  |       240.519 |
| 16  | `putusan_69_pid.sus_2023_pn_gto_20261107221831.pdf`  |       164.434 |
| 17  | `putusan_84_pid.sus_2023_pn_gto_20261107221816.pdf`  |       163.042 |
| 18  | `putusan_87_pid.sus_2025_pn_gto_20261107222552.pdf`  |       228.392 |
| 19  | `putusan_88_pid.sus_2025_pn_gto_20261107222525.pdf`  |       231.171 |
| 20  | `putusan_90_pid.sus_2025_pn_gto_20261107222204.pdf`  |       152.931 |
| 21  | `putusan_93_pid.sus_2025_pn_gto_20261107222536.pdf`  |       201.387 |
| 22  | `putusan_94_pid.sus_2025_pn_gto_20261107222544.pdf`  |       188.338 |
| 23  | `putusan_95_pid.sus_2025_pn_gto_20261107222602.pdf`  |       173.971 |
| 24  | `putusan_97_pid.sus_2025_pn_gto_20261107222611.pdf`  |       143.184 |
| 25  | `putusan_98_pid.sus_2024_pn_gto_20261107222128.pdf`  |       192.853 |
| 26  | `putusan_99_pid.sus_2023_pn_gto_20261107221809.pdf`  |       229.111 |
| 27  | `putusan_101_pid.sus_2025_pn_gto_20261107222221.pdf` |       159.939 |
| 28  | `putusan_105_pid.sus_2024_pn_gto_20261107221943.pdf` |       191.295 |
| 29  | `putusan_108_pid.sus_2024_pn_gto_20261107221937.pdf` |       212.516 |
| 30  | `putusan_112_pid.sus_2024_pn_gto_20261107222015.pdf` |       190.591 |
| 31  | `putusan_117_pid.sus_2025_pn_gto_20261107222209.pdf` |       231.806 |
| 32  | `putusan_119_pid.sus_2024_pn_gto_20261107222039.pdf` |       238.790 |
| 33  | `putusan_127_pid.sus_2024_pn_gto_20261107222007.pdf` |       186.695 |
| 34  | `putusan_134_pid.sus_2025_pn_gto_20261107222226.pdf` |       235.094 |
| 35  | `putusan_137_pid.sus_2023_pn_gto_20261107221739.pdf` |       199.412 |
| 36  | `putusan_138_pid.sus_2025_pn_gto_20261107222243.pdf` |       143.596 |
| 37  | `putusan_146_pid.sus_2023_pn_gto_20261107221801.pdf` |       198.645 |
| 38  | `putusan_148_pid.sus_2025_pn_gto_20261107222215.pdf` |       127.732 |
| 39  | `putusan_149_pid.sus_2024_pn_gto_20261107222050.pdf` |       152.093 |
| 40  | `putusan_150_pid.sus_2025_pn_gto_20261107222231.pdf` |       173.834 |
| 41  | `putusan_151_pid.sus_2025_pn_gto_20261107222237.pdf` |       169.545 |
| 42  | `putusan_152_pid.sus_2023_pn_gto_20261107221745.pdf` |       122.391 |
| 43  | `putusan_152_pid.sus_2023_pn_gto_20261107221753.pdf` |       122.390 |
| 44  | `putusan_186_pid.sus_2023_pn_gto_20261107221716.pdf` |       307.041 |
| 45  | `putusan_187_pid.sus_2023_pn_gto_20261107221709.pdf` |       251.148 |
| 46  | `putusan_202_pid.sus_2023_pn_gto_20261107221648.pdf` |       163.784 |
| 47  | `putusan_241_pid.sus_2023_pn_gto_20261107222139.pdf` |       200.945 |
| 48  | `putusan_249_pid.sus_2024_pn_gto_20261107222249.pdf` |       223.784 |
| 49  | `putusan_253_pid.sus_2024_pn_gto_20261107222254.pdf` |       267.960 |
| 50  | `putusan_276_pid.sus_2023_pn_gto_20261107222133.pdf` |       218.788 |
| 51  | `putusan_302_pid.sus_2023_pn_gto_20261107222148.pdf` |       193.159 |
| 52  | `putusan_303_pid.sus_2023_pn_gto_20261107222143.pdf` |       183.824 |

</details>

## Isi Overview.xlsx

Workbook `Overview/Overview.xlsx` memiliki satu sheet bernama `Overview` dengan `53` baris (`1` baris header + `52` baris data, seluruhnya terisi tanpa sel kosong) yang berkorespondensi 1-ke-1 dengan 52 berkas PDF di dalam `Narkotika.zip`. Kolomnya:

| Kolom               | Isi                                                                                                                 |
| ------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `No`                | Nomor urut (`1`–`52`)                                                                                               |
| `No Putusan`        | Nomor perkara, misalnya `101/Pid.Sus/2025/PN.GTO` atau `105/Pid.Sus/2024/PN Gto`                                    |
| `Lembaga Peradilan` | Nama pengadilan (`PN Gorontalo` pada seluruh 52 baris)                                                              |
| `Barang Bukti`      | Daftar barang bukti yang ditetapkan dalam putusan                                                                   |
| `Amar Putusan`      | Bunyi amar putusan: pernyataan bersalah, pidana penjara/rehabilitasi, denda, status barang bukti, dan biaya perkara |

Contoh baris (cuplikan dari baris pertama `Overview.xlsx`):

| No  | No Putusan              | Lembaga Peradilan | Barang Bukti                                                                                                                       | Amar Putusan                                                                                                                                                                                  |
| --- | ----------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | 101/Pid.Sus/2025/PN.GTO | PN Gorontalo      | 1 buah pembungkus rokok CAMEL berisi 1 sachet plastik klip berisi diduga Narkotika Shabu; 1 Unit Handphone Samsung Galaxy J2 Prime | Menyatakan terdakwa terbukti secara sah dan meyakinkan bersalah ... pidana penjara selama 3 (tiga) tahun ... Rehabilitasi Medis dan Sosial selama 6 (enam) bulan ... biaya perkara Rp 5.000,- |

## Penamaan File PDF

Setiap PDF memakai pola:

```text
putusan_<nomor>_<jenis>_<tahun>_<pn>_<yyyymmddHHMMSS>.pdf
```

Contoh: `putusan_46_pid.sus_2025_pn_gto_20261107222342.pdf`

| Bagian           | Arti                                                       |
| ---------------- | ---------------------------------------------------------- |
| `nomor`          | Nomor urut perkara                                         |
| `jenis`          | Jenis perkara (`pid.sus`)                                  |
| `tahun`          | Tahun perkara (`2023`, `2024`, atau `2025`)                |
| `pn`             | Kode pengadilan (`pn_gto` untuk PN Gorontalo)              |
| `yyyymmddHHMMSS` | Waktu pengunduhan (`20261107221648` s.d. `20261107222611`) |

## Cara Memakai

Unduh atau masuk ke direktori dataset, lalu ekstrak arsip PDF:

```bash
git clone https://github.com/dafanusa/Dataset-Narkotika_119_277.git
cd Dataset-Narkotika_119_277
unzip Dataset/Narkotika.zip -d Dataset/pdf
```

Baca ringkasan dengan Python:

```python
import pandas as pd

df = pd.read_excel("Overview/Overview.xlsx")
print(df.shape)
print(df.head())
```

Baca teks dari PDF (setelah diekstrak ke `Dataset/pdf/`):

```python
from pypdf import PdfReader

reader = PdfReader("Dataset/pdf/putusan_46_pid.sus_2025_pn_gto_20261107222342.pdf")
teks = "\n".join(page.extract_text() or "" for page in reader.pages)
print(teks[:1000])
```

Alternatif baca langsung dari `Dataset/Narkotika.zip` tanpa mengekstrak ke disk:

```python
import zipfile
from io import BytesIO
from pypdf import PdfReader

with zipfile.ZipFile("Dataset/Narkotika.zip", "r") as zf:
    nama_file = sorted(zf.namelist())[0]
    reader = PdfReader(BytesIO(zf.read(nama_file)))
    teks = "\n".join(page.extract_text() or "" for page in reader.pages)
    print(nama_file, len(reader.pages))
```

## Contoh Kegunaan

- **Mesin pencari putusan.** Bangun indeks (TF-IDF, BM25) dan cari putusan berdasarkan kata kunci seperti `sabu`/`shabu`, `ganja`, `Pasal 112`, `Pasal 114`, atau `Pasal 127`.
- **Ekstraksi informasi.** Ambil barang bukti, lama pidana, dan besar denda dengan regex atau model NER.
- **Klasifikasi.** Kelompokkan putusan menurut jenis narkotika atau rentang pidana.
- **Evaluasi retrieval.** Susun query dan kunci relevansi sendiri untuk menghitung precision, recall, dan MAP.
- **Analisis teks hukum.** Teliti pola kalimat, istilah, dan struktur dokumen putusan.

## Anatomi Putusan Narkotika

Putusan pidana narkotika punya kerangka yang cukup konsisten (seluruh 52 dokumen memuat bagian `MENGADILI` dan penanda Mahkamah Agung RI):

1. **Kepala putusan:** nomor perkara, nama pengadilan (`Pengadilan Negeri Gorontalo`), identitas terdakwa.
2. **Dakwaan dan tuntutan:** pasal yang didakwakan dan tuntutan penuntut umum.
3. **Pertimbangan hukum:** fakta persidangan, alat bukti, unsur pasal.
4. **Amar putusan:** diawali kata `MENGADILI`; memuat vonis, pidana penjara/rehabilitasi, denda, dan status barang bukti.
5. **Penutup:** tanggal putusan, majelis hakim, panitera pengganti, serta blok _disclaimer_ Mahkamah Agung RI.

Kerangka ini membantu ekstraksi: barang bukti dan amar putusan dapat dikenali lewat penanda `barang bukti berupa` dan `MENGADILI`.

## Etika dan Legalitas

Putusan pengadilan adalah informasi publik yang dipublikasikan oleh Mahkamah Agung RI melalui portal resminya. Dataset ini dikumpulkan dari portal tersebut untuk tujuan pendidikan dan penelitian.

Mohon gunakan dengan bijak. Dokumen memuat nama pihak yang berperkara, jadi jangan dipakai untuk menyebarkan data pribadi atau menstigma pihak tertentu. Hak atas isi putusan tetap pada pihak yang berwenang; repositori ini tidak mengklaim kepemilikan atas dokumen asli.

## Tim

| Nama                                | NIM             | Peran                                             |
| ----------------------------------- | --------------- | ------------------------------------------------- |
| Rizqullah Atsir Dafa Childyasa Nusa | 202310370311119 | Pengumpulan, penyusunan dataset, dan dokumentasi  |
| Ayesha Fahrelia Ningrum             | 202310370311277 | Pengumpulan, pembuatan ringkasan, dan dokumentasi |

Mata kuliah Temu Kembali Informasi D, Semester Ganjil 2026/2027, Fakultas Teknik, Universitas Muhammadiyah Malang.
