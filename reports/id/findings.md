# Temuan Portofolio

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](../../case-library/id/README.md) · [Metodologi](../../methodology/id/evaluation-methodology.md) · [Pemetaan evidence](../../evidence/README-ID.md) · [English](../en/findings.md)

## Hal yang Ditunjukkan Portofolio Ini

Ke-27 kasus mendokumentasikan masalah kualitas dalam penggunaan ChatGPT Go di dunia nyata. Pola terkuat adalah kepatuhan instruksi, tetapi kasus-kasus tersebut juga menunjukkan masalah konteks, penalaran, format, penggunaan alat, dan workflow. Severity menjelaskan konteks setiap kasus yang disetujui, bukan rating produk secara umum.

## Kategori Isu yang Tidak Saling Eksklusif

| Kategori isu | Kasus |
|---|---:|
| Mengikuti Instruksi | 19 |
| Kesalahan Pemformatan | 11 |
| Penanganan Konteks | 8 |
| Requirement yang Hilang | 6 |
| Penggunaan Alat | 6 |
| Inkonsistensi | 5 |
| Kesalahan Penalaran | 5 |
| Asumsi yang Salah | 2 |
| Kontradiksi | 1 |
| Halusinasi | 1 |

Kategori saling tumpang tindih, sehingga jumlah kategori lebih besar dari 27. Penghitungan ini hanya menjelaskan portofolio ini. Angka tersebut bukan estimasi prevalensi untuk ChatGPT Go dan bukan perbandingan dengan paket, model, konfigurasi, atau versi lain.

## Pola Evaluasi

### Interpretasi requirement

Beberapa kasus menunjukkan alasan evaluator harus mengidentifikasi requirement aktif sebelum menilai kualitas output. Contohnya mencakup perbedaan aturan jumlah kata tepat pada [CASE-001](../../case-library/id/CASE-001.md), pertanyaan operasional JSON pada [CASE-007](../../case-library/id/CASE-007.md), dan tahap ringkasan pada [CASE-023](../../case-library/id/CASE-023.md).

### Kontinuitas konteks dan workflow

Pekerjaan bertahap dapat gagal meskipun setiap respons tampak wajar jika dilihat terpisah. [CASE-008](../../case-library/id/CASE-008.md) menguji kontrak perintah yang berulang. [CASE-014](../../case-library/id/CASE-014.md) mengikuti konten yang disetujui melalui pengambilan dan ekspor. [CASE-016](../../case-library/id/CASE-016.md) memeriksa apakah ketidakpastian diselesaikan sebelum eksekusi.

### Fidelitas dan klaim terukur

Kualitas penyajian tidak menggantikan fidelitas sumber. [CASE-021](../../case-library/id/CASE-021.md) memisahkan preservasi dari peringkasan. [CASE-018](../../case-library/id/CASE-018.md) menunjukkan alasan klaim kelayakan harus diuji dengan pengukuran yang dapat direproduksi.

### Peran dan tanggung jawab

[CASE-024](../../case-library/id/CASE-024.md) menunjukkan bahwa evaluator harus mengidentifikasi siapa yang membuat keputusan klasifikasi sebelum menetapkan kesalahan atau tindakan korektif.

## Batasan

Portofolio ini tidak menguji setiap fitur atau interaksi ChatGPT Go. Portofolio ini tidak menetapkan penyebab internal, tingkat kegagalan umum, atau perbedaan kinerja antarproduk. Temuan tetap dibatasi pada evidence, validasi manusia, severity yang disetujui, dan ketidakpastian yang dicatat pada setiap kasus.
