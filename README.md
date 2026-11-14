# Dataset-Narkotika_119_277

> Kumpulan putusan Pengadilan Negeri Gorontalo perkara narkotika (Pidana Khusus), tahun 2023-2025, untuk riset dan praktikum Temu Kembali Informasi (Information Retrieval).

![Format](https://img.shields.io/badge/format-PDF%20%2B%20XLSX-blue)
![Domain](https://img.shields.io/badge/domain-hukum-8a2be2)
![Bahasa](https://img.shields.io/badge/bahasa-Indonesia-red)
![Dokumen](https://img.shields.io/badge/dokumen-63%20PDF-green)

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

Putusan pengadilan adalah teks hukum yang panjang, formal, dan memiliki pola kalimat berulang. Dataset ini disiapkan sebagai korpus untuk Temu Kembali Informasi, ekstraksi informasi, klasifikasi, dan analisis teks hukum.

Arsip terbaru memuat **63 berkas PDF** yang mewakili **61 nomor perkara unik** (nomor dan tahun). Dua nomor perkara tercatat dua kali: `152/Pid.Sus/2023/PN Gto` dan `190/Pid.Sus/2025/PN Gto`. Workbook `Overview.xlsx` memuat satu baris untuk setiap PDF.

| Item | Keterangan |
| --- | --- |
| Jumlah dokumen | 63 berkas PDF; 61 nomor perkara unik, dengan dua nomor perkara yang masing-masing memiliki entri ganda |
| Total halaman | 1.672 halaman; 15-59 halaman per PDF, rata-rata 26,54 halaman |
| Ukuran PDF | 12.547.325 byte total ukuran PDF sebelum kompresi |
| Ukuran arsip | `Dataset/Narkotika.zip`, 10.840.239 byte |
| Format ringkasan | `Overview/Overview.xlsx`, 29.868 byte; 64 baris (1 header + 63 data) x 5 kolom |
| Pengadilan | PN Gorontalo (Pengadilan Negeri Gorontalo) |
| Kategori | Pidana Khusus (`Pid.Sus`), Narkotika |
| Rentang tahun | 2023-2025: 2023 (16 PDF / 15 perkara unik), 2024 (10 / 10), 2025 (37 / 36) |
| Bahasa | Indonesia |

## Sumber Data

Putusan diunduh dari **Direktori Putusan Mahkamah Agung Republik Indonesia**:

- Portal: https://putusan3.mahkamahagung.go.id/direktori.html
- Jalur penelusuran: Direktori > Pidana Khusus > Narkotika dan Psikotropika > PN Gorontalo > filter tahun 2023, 2024, dan 2025.
- Nama file menunjukkan tanggal pengunduhan 14 November 2026, dengan waktu pada nama file dari `11:44:55` sampai `12:05:48`.

## Kriteria Pengumpulan

1. Berasal dari direktori **Pidana Khusus (`Pid.Sus`)** perkara narkotika.
2. Berasal dari **Pengadilan Negeri Gorontalo**.
3. Tahun putusan berada pada rentang **2023-2025**.
4. Dokumen putusan disimpan dalam format `.pdf` dan diringkas di `Overview.xlsx`.

## Struktur Repository

```text
Dataset-Narkotika_119_277/
|-- Dataset/
|   `-- Narkotika.zip        # 63 PDF, ukuran arsip 10.840.239 byte
|-- Overview/
|   `-- Overview.xlsx        # 63 baris data, 5 kolom
`-- README.md
```

<details>
<summary>Daftar lengkap PDF di dalam <code>Dataset/Narkotika.zip</code></summary>

| No | Nama File | Ukuran (Byte) |
| :-: | :--- | ---: |
| 1 | `putusan_101_pid.sus_2025_pn_gto_20261114115532.pdf` | 159,939 |
| 2 | `putusan_104_pid.sus_2025_pn_gto_20261114120414.pdf` | 208,097 |
| 3 | `putusan_105_pid.sus_2024_pn_gto_20261114114930.pdf` | 191,295 |
| 4 | `putusan_108_pid.sus_2024_pn_gto_20261114114914.pdf` | 212,516 |
| 5 | `putusan_10_pid.sus_2025_pn_gto_20261114115900.pdf` | 250,268 |
| 6 | `putusan_112_pid.sus_2024_pn_gto_20261114115031.pdf` | 190,591 |
| 7 | `putusan_117_pid.sus_2025_pn_gto_20261114115458.pdf` | 231,806 |
| 8 | `putusan_119_pid.sus_2024_pn_gto_20261114115114.pdf` | 238,790 |
| 9 | `putusan_127_pid.sus_2024_pn_gto_20261114115015.pdf` | 186,695 |
| 10 | `putusan_127_pid.sus_2025_pn_gto_20261114120512.pdf` | 164,180 |
| 11 | `putusan_12_pid.sus_2025_pn_gto_20261114115912.pdf` | 268,100 |
| 12 | `putusan_134_pid.sus_2025_pn_gto_20261114115558.pdf` | 235,094 |
| 13 | `putusan_135_pid.sus_2025_pn_gto_20261114120437.pdf` | 143,044 |
| 14 | `putusan_137_pid.sus_2023_pn_gto_20261114114542.pdf` | 199,412 |
| 15 | `putusan_138_pid.sus_2025_pn_gto_20261114115657.pdf` | 143,596 |
| 16 | `putusan_146_pid.sus_2023_pn_gto_20261114114617.pdf` | 198,645 |
| 17 | `putusan_148_pid.sus_2025_pn_gto_20261114115511.pdf` | 127,732 |
| 18 | `putusan_149_pid.sus_2024_pn_gto_20261114115131.pdf` | 152,093 |
| 19 | `putusan_14_pid.sus_2025_pn_gto_20261114115736.pdf` | 273,883 |
| 20 | `putusan_150_pid.sus_2025_pn_gto_20261114115611.pdf` | 173,834 |
| 21 | `putusan_151_pid.sus_2025_pn_gto_20261114115632.pdf` | 169,545 |
| 22 | `putusan_152_pid.sus_2023_pn_gto_20261114114551.pdf` | 122,391 |
| 23 | `putusan_152_pid.sus_2023_pn_gto_20261114114604.pdf` | 122,390 |
| 24 | `putusan_16_pid.sus_2025_pn_gto_20261114115747.pdf` | 165,722 |
| 25 | `putusan_17_pid.sus_2024_pn_gto_20261114115232.pdf` | 141,503 |
| 26 | `putusan_17_pid.sus_2025_pn_gto_20261114115822.pdf` | 165,405 |
| 27 | `putusan_186_pid.sus_2023_pn_gto_20261114114516.pdf` | 307,041 |
| 28 | `putusan_187_pid.sus_2023_pn_gto_20261114114508.pdf` | 251,148 |
| 29 | `putusan_190_pid.sus_2025_pn_gto_20261114120449.pdf` | 167,205 |
| 30 | `putusan_190_pid.sus_2025_pn_gto_20261114120526.pdf` | 167,199 |
| 31 | `putusan_202_pid.sus_2023_pn_gto_20261114114455.pdf` | 163,784 |
| 32 | `putusan_225_pid.sus_2023_pn_gto_20261114114502.pdf` | 150,023 |
| 33 | `putusan_241_pid.sus_2023_pn_gto_20261114115321.pdf` | 200,945 |
| 34 | `putusan_249_pid.sus_2024_pn_gto_20261114115713.pdf` | 223,784 |
| 35 | `putusan_24_pid.sus_2025_pn_gto_20261114115936.pdf` | 229,733 |
| 36 | `putusan_253_pid.sus_2024_pn_gto_20261114115724.pdf` | 267,960 |
| 37 | `putusan_276_pid.sus_2023_pn_gto_20261114115256.pdf` | 218,788 |
| 38 | `putusan_302_pid.sus_2023_pn_gto_20261114115408.pdf` | 193,159 |
| 39 | `putusan_303_pid.sus_2023_pn_gto_20261114115344.pdf` | 183,824 |
| 40 | `putusan_34_pid.sus_2025_pn_gto_20261114115846.pdf` | 203,201 |
| 41 | `putusan_39_pid.sus_2025_pn_gto_20261114115759.pdf` | 186,087 |
| 42 | `putusan_40_pid.sus_2025_pn_gto_20261114120548.pdf` | 249,494 |
| 43 | `putusan_43_pid.sus_2025_pn_gto_20261114120045.pdf` | 189,566 |
| 44 | `putusan_44_pid.sus_2025_pn_gto_20261114120012.pdf` | 144,166 |
| 45 | `putusan_45_pid.sus_2025_pn_gto_20261114120025.pdf` | 551,415 |
| 46 | `putusan_46_pid.sus_2025_pn_gto_20261114115956.pdf` | 155,324 |
| 47 | `putusan_54_pid.sus_2025_pn_gto_20261114120100.pdf` | 218,092 |
| 48 | `putusan_55_pid.sus_2025_pn_gto_20261114120112.pdf` | 183,136 |
| 49 | `putusan_57_pid.sus_2023_pn_gto_20261114114650.pdf` | 240,519 |
| 50 | `putusan_69_pid.sus_2023_pn_gto_20261114114659.pdf` | 164,434 |
| 51 | `putusan_84_pid.sus_2023_pn_gto_20261114114638.pdf` | 163,042 |
| 52 | `putusan_87_pid.sus_2025_pn_gto_20261114120200.pdf` | 228,392 |
| 53 | `putusan_88_pid.sus_2025_pn_gto_20261114120124.pdf` | 231,171 |
| 54 | `putusan_90_pid.sus_2025_pn_gto_20261114115438.pdf` | 152,931 |
| 55 | `putusan_92_pid.sus_2025_pn_gto_20261114120347.pdf` | 189,680 |
| 56 | `putusan_93_pid.sus_2025_pn_gto_20261114120136.pdf` | 201,387 |
| 57 | `putusan_94_pid.sus_2025_pn_gto_20261114120149.pdf` | 188,338 |
| 58 | `putusan_95_pid.sus_2025_pn_gto_20261114120214.pdf` | 173,971 |
| 59 | `putusan_96_pid.sus_2025_pn_gto_20261114120312.pdf` | 172,271 |
| 60 | `putusan_97_pid.sus_2025_pn_gto_20261114120235.pdf` | 143,184 |
| 61 | `putusan_98_pid.sus_2024_pn_gto_20261114115213.pdf` | 192,853 |
| 62 | `putusan_99_pid.sus_2023_pn_gto_20261114114628.pdf` | 229,111 |
| 63 | `putusan_99_pid.sus_2025_pn_gto_20261114120250.pdf` | 234,401 |

</details>

## Isi Overview.xlsx

`Overview/Overview.xlsx` memiliki satu sheet bernama `Sheet1`, dengan 64 baris (1 baris header dan 63 baris data) serta 5 kolom. Seluruh 63 baris data berkorespondensi dengan PDF di dalam ZIP; seluruh sel data terisi.

| Kolom | Isi |
| --- | --- |
| `No` | Nomor urut data (1-63) |
| `No Putusan` | Nomor perkara, misalnya `101/Pid.Sus/2025/PN.GTO` atau `104/Pid.Sus/2025/PN Gto` |
| `Lembaga Peradilan` | Nama pengadilan; semua baris berisi PN Gorontalo |
| `Barang Bukti` | Daftar barang bukti dalam putusan |
| `Amar Putusan` | Amar putusan, termasuk pidana, denda, status barang bukti, dan biaya perkara |

Dua nomor perkara yang tercatat dua kali pada workbook adalah `152/Pid.Sus/2023/PN Gto` dan `190/Pid.Sus/2025/PN Gto`.

## Penamaan File PDF

Nama setiap PDF mengikuti pola:

```text
putusan_<nomor>_<jenis>_<tahun>_<pn>_<yyyymmddHHMMSS>.pdf
```

Contoh: `putusan_46_pid.sus_2025_pn_gto_20261114115956.pdf`

| Bagian | Arti |
| --- | --- |
| `nomor` | Nomor perkara |
| `jenis` | Jenis perkara (`pid.sus`) |
| `tahun` | Tahun perkara (2023, 2024, atau 2025) |
| `pn` | Kode pengadilan (`pn_gto` untuk PN Gorontalo) |
| `yyyymmddHHMMSS` | Timestamp pada nama file; rentang yang ada di ZIP `20261114114455`-`20261114120548` |

## Cara Memakai

Klon repositori, lalu ekstrak arsip PDF:

```bash
git clone https://github.com/dafanusa/Dataset-Narkotika_119_277.git
cd Dataset-Narkotika_119_277
unzip Dataset/Narkotika.zip -d Dataset/pdf
```

Baca ringkasan dengan Python:

```python
import pandas as pd

df = pd.read_excel("Overview/Overview.xlsx", sheet_name="Sheet1")
print(df.shape)  # (63, 5)
print(df.head())
```

Baca teks PDF setelah diekstrak:

```python
from pypdf import PdfReader

reader = PdfReader("Dataset/pdf/putusan_46_pid.sus_2025_pn_gto_20261114115956.pdf")
teks = "\n".join(page.extract_text() or "" for page in reader.pages)
print(teks[:1000])
```

PDF juga dapat dibaca langsung dari ZIP tanpa mengekstraknya ke disk:

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

- **Mesin pencari putusan.** Bangun indeks TF-IDF atau BM25 untuk pencarian berdasarkan kata kunci seperti `sabu`, `shabu`, `ganja`, `Pasal 112`, `Pasal 114`, atau `Pasal 127`.
- **Ekstraksi informasi.** Ambil barang bukti, lama pidana, dan besar denda dengan regex atau model NER.
- **Klasifikasi.** Kelompokkan putusan menurut jenis narkotika atau rentang pidana.
- **Evaluasi retrieval.** Susun query dan label relevansi untuk menghitung precision, recall, dan MAP.
- **Analisis teks hukum.** Teliti pola kalimat, istilah, dan struktur dokumen putusan.

## Anatomi Putusan Narkotika

Putusan pidana narkotika umumnya memiliki bagian-bagian berikut; susunan dan kelengkapannya dapat berbeda pada tiap dokumen:

1. **Kepala putusan:** nomor perkara, nama pengadilan, dan identitas terdakwa.
2. **Dakwaan dan tuntutan:** pasal yang didakwakan dan tuntutan penuntut umum.
3. **Pertimbangan hukum:** fakta persidangan, alat bukti, dan unsur pasal.
4. **Amar putusan:** bagian yang diawali kata `MENGADILI`; dapat memuat vonis, pidana penjara atau rehabilitasi, denda, dan status barang bukti.
5. **Penutup:** tanggal putusan, majelis hakim, panitera pengganti, dan keterangan lain.

## Etika dan Legalitas

Putusan pengadilan merupakan informasi publik yang dipublikasikan oleh Mahkamah Agung RI. Dataset ini dikumpulkan dari portal tersebut untuk tujuan pendidikan dan penelitian.

Dokumen memuat nama pihak yang berperkara. Gunakan dataset dengan bijak dan jangan memakainya untuk menyebarkan data pribadi atau menstigma pihak tertentu. Repositori ini tidak mengklaim kepemilikan atas dokumen asli.

## Tim

| Nama | NIM | Peran |
| --- | --- | --- |
| Rizqullah Atsir Dafa Childyasa Nusa | 202310370311119 | Pengumpulan, penyusunan dataset, dan dokumentasi |
| Ayesha Fahrelia Ningrum | 202310370311277 | Pengumpulan, pembuatan ringkasan, dan dokumentasi |

Mata kuliah Temu Kembali Informasi D, Semester Ganjil 2026/2027, Fakultas Teknik, Universitas Muhammadiyah Malang.
