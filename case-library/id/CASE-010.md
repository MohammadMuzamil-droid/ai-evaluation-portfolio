# CASE-010 — Persyaratan keluaran kode berpagar tidak diikuti

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

Revisi Korektif Kedua Selesai — Menunggu Validasi Ulang Independen

## Tanggal

2026-07-21

## Keterlacakan Sumber

- **PRA ID:** PRA-012
- **ID TRIAGE:** dapat dilacak dari `EVENT-0224`
- **Judul Percakapan:** Alur analisis portofolio template manager
- **ID Percakapan:** `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0224`
- **ID Pesan yang Relevan:** asisten `463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9`; koreksi `bbb21769-6bce-43b7-a862-f638e55f457b`; tindak lanjut `e13f8c82-229b-43a0-9f42-23d02bde668a`

## Daftar Evidence

- **CASE-010-E01:** `bbb21174-a22d-4c35-a102-ebf3d049df4e`; pembicara `user`; stempel waktu `2026-07-21T11:22:12.871670Z`; fungsi: mengatur instruksi/konteks; percakapan `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E02:** `463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9`; pembicara `assistant`; stempel waktu `2026-07-21T11:22:13.320447Z`; fungsi: respon bermasalah; percakapan `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E03:** `bbb21769-6bce-43b7-a862-f638e55f457b`; pembicara `user`; stempel waktu `2026-07-21T11:23:40.199457Z`; fungsi: koreksi pengguna; percakapan `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.
- **CASE-010-E04:** `e13f8c82-229b-43a0-9f42-23d02bde668a`; pembicara `assistant`; stempel waktu `2026-07-21T11:23:40.819257Z`; fungsi: asisten tindak lanjut; percakapan `6a5d9813-ad40-83ee-bbd0-a7880f11b4dd`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-012: mengatur instruksi/konteks (`bbb21174-a22d-4c35-a102-ebf3d049df4e` pada 2026-07-21T11:22:12.871670Z).
[[TETAP9]]. PRE-012: respon bermasalah (`463ecd7d-cae5-4d5b-b5bb-2d7f4c21cfe9` pada 2026-07-21T11:22:13.320447Z).
[[TETAP18]]. PRE-012: koreksi pengguna (`bbb21769-6bce-43b7-a862-f638e55f457b` pada 2026-07-21T11:23:40.199457Z).
[[TETAP27]]. PRE-012: asisten tindak lanjut (`e13f8c82-229b-43a0-9f42-23d02bde668a` di 2026-07-21T11:23:40.819257Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan

## Severity

**Minor** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Bukti tersebut mempertahankan persyaratan eksplisit untuk mengembalikan konten dalam struktur kode berpagar, keluaran yang tidak menggunakan pembungkus yang diperlukan, dan koreksi pengguna. Ini adalah insiden kepatuhan format dengan pemeriksaan biner yang terlihat. Hal ini tidak tergantung pada menilai kualitas prosa yang mendasarinya.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Instruksi yang diminta disampaikan tanpa pagar kode yang ditentukan. **Persyaratan dan penyimpangan.** Pagar adalah bagian dari skema keluaran, jadi teks biasa atau format alternatif tidak dapat dipertukarkan meskipun kata-katanya dapat digunakan. **Inferensi dan batas.** Urutan ini mendukung batasan pemformatan yang terlewat; itu tidak menunjukkan apakah asisten menguraikan permintaan pagar dan kemudian membuangnya. Konsekuensinya adalah berkurangnya kemampuan penyalinan atau kegagalan dalam alur kerja hilir yang memerlukan blok berpagar.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Kembalikan teks yang diminta di dalam pembatas pagar dan label bahasa yang tepat, tanpa materi di sekitarnya yang mengganggu penyalinan langsung.

### B. Perintah/Mitigasi Pengguna

Beri nama sintaks pagar yang diinginkan ketika parser eksternal bergantung padanya, sambil mencatat bahwa instruksi yang diarsipkan telah membuat kewajiban pemformatan menjadi eksplisit.

### C. Peningkatan Model

Tambahkan validator struktural pasca-generasi yang memeriksa pagar pembukaan dan penutupan yang diperlukan sebelum mengirimkan respons.

## Pelajaran untuk Pengguna

Ketika respons dimaksudkan untuk disalin ke suatu alat, validasi wadahnya serta teksnya. Pembungkus minor secara visual dapat menjadi persyaratan fungsional.

## Pelajaran untuk Pengembang

Gunakan pengujian yang meminta blok berpagar dan periksa token keluaran mentah untuk kedua pembatas. Kesetaraan konten saja tidak boleh lolos evaluasi.

## Kesimpulan Akhir

Kasus ini dapat diverifikasi secara sempit: pembungkus berpagar yang diminta tidak ada. Karena cacatnya bersifat struktural dan bukan semantik, maka cacat ini menawarkan target regresi yang bersih tanpa perlu berspekulasi tentang alasan model.

