# CASE-005 — Konten kurikulum ditambahkan di luar cakupan alur kerja

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-005.md)

## Lingkungan Evaluasi

- **Produk:** ChatGPT
- **Paket:** ChatGPT Go
- **Sumber paket:** Konteks terkonfirmasi dari percakapan terdokumentasi
- **Fitur / konteks:** Tidak tersedia pada tingkat portofolio
- **Model, konfigurasi, dan platform:** Tidak tersedia pada tingkat portofolio

Portofolio ini mencatat penggunaan ChatGPT Go di dunia nyata dalam lingkungan yang terdokumentasi. Paket adalah konteks dari percakapan. Paket tidak diperlakukan sebagai evidence screenshot kecuali sebuah sumber menunjukkannya.

## Batas Ruang Lingkup dan Generalisasi

Ini adalah temuan khusus kasus dari penggunaan ChatGPT Go yang terdokumentasi. Temuan ini tidak membuktikan hasil yang sama untuk paket, konfigurasi, model, versi ChatGPT lain, produk OpenAI, atau sistem AI lain.

## Penanganan Evidence

Portofolio publik menyimpan Daftar Evidence dan catatan keterlacakan yang telah diverifikasi. Kutipan percakapan asli dan screenshot tetap berada di arsip proyek privat dan tidak dipublikasikan otomatis.

## Status

Diarsipkan

## Tanggal

2026-07-17

## Keterlacakan Sumber

- **PRA ID:** PRA-005
- **ID TRIAGE:** dapat dilacak dari `EVENT-0125`
- **Judul Percakapan:** Kursus Inggris
- **ID Percakapan:** `6a570be4-831c-83ee-ab90-8bcff996410e`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0125`
- **ID Pesan yang Relevan:** asisten `0894563f-1b7e-45ed-82c7-46824baf8730`; koreksi `bbb21973-61d5-4a07-9f59-3e00f21aeef7`; tindak lanjut `368e0570-ceb6-4f05-8738-c31e67b9190b`

## Daftar Evidence

- **CASE-005-E01:** `bbb21176-5de0-44fe-b727-388388599887`; pembicara `user`; stempel waktu `2026-07-17T11:21:36.486327Z`; fungsi: mengatur instruksi/konteks; percakapan `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E02:** `0894563f-1b7e-45ed-82c7-46824baf8730`; pembicara `assistant`; stempel waktu `2026-07-17T11:21:36.823546Z`; fungsi: respon bermasalah; percakapan `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E03:** `bbb21973-61d5-4a07-9f59-3e00f21aeef7`; pembicara `user`; stempel waktu `2026-07-17T11:23:34.030653Z`; fungsi: koreksi pengguna; percakapan `6a570be4-831c-83ee-ab90-8bcff996410e`.
- **CASE-005-E04:** `368e0570-ceb6-4f05-8738-c31e67b9190b`; pembicara `assistant`; stempel waktu `2026-07-17T11:23:34.427258Z`; fungsi: asisten tindak lanjut; percakapan `6a570be4-831c-83ee-ab90-8bcff996410e`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-005: mengatur instruksi/konteks (`bbb21176-5de0-44fe-b727-388388599887` pada 2026-07-17T11:21:36.486327Z).
[[TETAP9]]. PRE-005: respon bermasalah (`0894563f-1b7e-45ed-82c7-46824baf8730` pada 2026-07-17T11:21:36.823546Z).
[[TETAP18]]. PRE-005: koreksi pengguna (`bbb21973-61d5-4a07-9f59-3e00f21aeef7` pada 2026-07-17T11:23:34.030653Z).
[[TETAP27]]. PRE-005: asisten tindak lanjut (`368e0570-ceb6-4f05-8738-c31e67b9190b` di 2026-07-17T11:23:34.427258Z).

## Kategori Isu

Mengikuti Instruksi; Penanganan Konteks

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Bukti tersebut menempatkan Instruksi Proyek yang persisten di samping kurikulum sesi dan mencatat penambahan materi kurikulum di luar batas alur kerja yang diminta. Koreksi ini menyangkut pemisahan aturan proyek yang tahan lama dari konten khusus sesi. Hal ini mendukung temuan yang menyebar luas tanpa menyiratkan bahwa seluruh isi kurikulum secara intrinsik tidak sesuai.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Materi yang termasuk dalam kurikulum sesi dimasukkan ke dalam, atau diizinkan untuk diperluas, alur kerja instruksi persisten tanpa integrasi yang diminta. **Persyaratan dan penyimpangan.** Petunjuk Proyek menetapkan aturan pengoperasian yang berjangka panjang; Isi kurikulum mempunyai tujuan dan umur yang berbeda-beda. Menggabungkannya tanpa keputusan eksplisit akan mengubah cakupan konfigurasi tahan lama. **Inferensi dan batas.** Catatan mendukung kegagalan pelapisan, bukan klaim bahwa asisten tidak dapat membedakan kategori ini dalam setiap konteks. Konsekuensinya adalah kumpulan instruksi proyek yang membengkak atau terkontaminasi yang memengaruhi sesi mendatang.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Jaga agar Instruksi Proyek tetap terbatas pada aturan pengoperasian dan tempatkan konten pelajaran atau kurikulum di bagian sesi yang diberi label terpisah kecuali pengguna secara eksplisit meminta konsolidasi.

### B. Perintah/Mitigasi Pengguna

Gunakan judul seperti ‘aturan proyek yang persisten’ dan ‘kurikulum sesi ini’ ketika keduanya muncul dalam satu permintaan; label membantu meninjau tetapi tidak diperlukan bagi asisten untuk menghormati ruang lingkup.

### C. Peningkatan Model

Evaluasi komposisi konteks panjang dengan dua lapisan konten dan tolak keluaran yang memigrasikan materi pelajaran sementara menjadi instruksi yang tahan lama tanpa permintaan integrasi eksplisit.

## Pelajaran untuk Pengguna

Sebelum menerima penulisan ulang instruksi proyek, periksa apakah ada kalimat baru yang akan mengatur pekerjaan selanjutnya atau hanya mengajarkan sesi saat ini. Kedua destinasi tersebut memerlukan standar peninjauan yang berbeda.

## Pelajaran untuk Pengembang

Perlengkapan yang berguna memadukan aturan alur kerja yang stabil dengan rencana pembelajaran satu kali. Melewati keluaran akan mempertahankan batas dan menjelaskan referensi silang yang disengaja daripada menggabungkan lapisan secara diam-diam.

## Kesimpulan Akhir

Ini adalah kesalahan cakupan yang terus-menerus: materi kurikulum sementara memperluas konfigurasi yang dimaksudkan agar tetap stabil. Bukti-bukti mendukung kekhawatiran mengenai batas wilayah; hal ini tidak membuktikan bahwa kurikulum tambahan tersebut kurang bernilai dalam konteks sesi aslinya.

