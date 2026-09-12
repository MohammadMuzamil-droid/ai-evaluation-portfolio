# CASE-004 — REVISE mengembalikan log perubahan, bukan draf yang direvisi

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-004.md)

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

- **PRA ID:** PRA-004
- **ID TRIAGE:** dapat dilacak dari `EVENT-0114`
- **Judul Percakapan:** Perpustakaan Templat
- **ID Percakapan:** `6a57d4d3-bff4-83e8-9966-384ed9d41334`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0114`
- **ID Pesan yang Relevan:** asisten `0f152a19-8805-4dfa-8423-9682f5b5e537`; koreksi `bbb219b8-a1b8-4829-8bf8-4af32aac8f93`; tindak lanjut `f469d3f5-2141-411e-9d9d-24aac56b3a77`

## Daftar Evidence

- **CASE-004-E01:** `bbb21b26-d6d8-4209-9388-d5d7e354590f`; pembicara `user`; stempel waktu `2026-07-17T03:06:48.299575Z`; fungsi: mengatur instruksi/konteks; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E02:** `0f152a19-8805-4dfa-8423-9682f5b5e537`; pembicara `assistant`; stempel waktu `2026-07-17T03:06:48.680813Z`; fungsi: respon bermasalah; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E03:** `bbb219b8-a1b8-4829-8bf8-4af32aac8f93`; pembicara `user`; stempel waktu `2026-07-17T03:07:43.795771Z`; fungsi: koreksi pengguna; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-004-E04:** `f469d3f5-2141-411e-9d9d-24aac56b3a77`; pembicara `assistant`; stempel waktu `2026-07-17T03:07:44.175886Z`; fungsi: asisten tindak lanjut; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-004: mengatur instruksi/konteks (`bbb21b26-d6d8-4209-9388-d5d7e354590f` pada 2026-07-17T03:06:48.299575Z).
[[TETAP9]]. PRE-004: respon bermasalah (`0f152a19-8805-4dfa-8423-9682f5b5e537` pada 2026-07-17T03:06:48.680813Z).
[[TETAP18]]. PRE-004: koreksi pengguna (`bbb219b8-a1b8-4829-8bf8-4af32aac8f93` pada 2026-07-17T03:07:43.795771Z).
[[TETAP27]]. PRE-004: asisten tindak lanjut (`f469d3f5-2141-411e-9d9d-24aac56b3a77` di 2026-07-17T03:07:44.175886Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Pesan insiden menyimpan perintah berlabel REVISE, respons asisten yang terdiri dari log perubahan atau diskusi, dan koreksi pengguna bahwa draf yang direvisi itu sendiri diperlukan. Tindak lanjutnya menegaskan perbedaan tersebut. Bukti-bukti tersebut mengidentifikasi adanya substitusi perintah-untuk-diserahkan, bukannya ketidaksepakatan mengenai gaya.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Daripada mengeluarkan teks revisi yang diminta oleh REVISE, asisten menjelaskan atau menyebutkan perubahan. **Persyaratan dan penyimpangan.** Log perubahan dapat menyertai revisi, namun tidak dapat menggantikan artefak utama ketika perintah meminta draf ditulis ulang. **Inferensi dan batas.** Urutan ini menunjukkan ketidakcocokan jenis keluaran; hal ini tidak memberi tahu kami apakah draf yang dihilangkan tersebut dibuat secara internal. Hal ini penting karena pengguna tidak dapat meninjau, menyalin, atau menerapkan revisi yang diminta dari materi yang dikirimkan.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Menghasilkan draf revisi lengkap terlebih dahulu, dengan tetap mempertahankan format yang diminta; tambahkan log perubahan ringkas hanya setelah draf jika itu menambah nilai.

### B. Perintah/Mitigasi Pengguna

Nyatakan 'kembalikan teks pengganti lengkap' ketika draf harus dapat langsung digunakan, dengan tetap mengakui bahwa perintah REVISE asli sudah cukup spesifik.

### C. Peningkatan Model

Tambahkan pemeriksaan niat ke artefak sehingga REVISE memetakan konten yang diubah dan tidak hanya memberikan komentar tentang transformasi.

## Pelajaran untuk Pengguna

Untuk perintah pengeditan, periksa apakah respons berisi artefak pengganti yang dapat ditempelkan ke dalam karya. Penjelasan suntingan secara operasional tidak setara dengan teks yang disunting.

## Pelajaran untuk Pengembang

Uji REVISE dengan paragraf sumber dan minta keluaran berisi paragraf revisi penuh. Respons yang hanya berisi poin-poin tentang perubahan akan gagal meskipun poin-poin tersebut masuk akal.

## Kesimpulan Akhir

Pertukaran yang dipertahankan mengisolasi kegagalan yang dapat disampaikan secara langsung: deskripsi perubahan diberikan ketika draf yang direvisi diperlukan. Maknanya praktis—tanpa drafnya, tugas penyuntingan yang diminta tetap belum selesai.

