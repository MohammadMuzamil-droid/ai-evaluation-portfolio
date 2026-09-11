# CASE-015 — Evaluasi menghilangkan teks jawaban lengkap

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

2026-07-27

## Keterlacakan Sumber

- **PRA ID:** PRA-021
- **ID TRIAGE:** dapat dilacak dari `EVENT-0373`
- **Judul Percakapan:** Sertifikasi OneForma LLM
- **ID Percakapan:** `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0373`
- **ID Pesan yang Relevan:** asisten `37192b10-28ec-4b5d-b04c-6c6dab4ac3c8`; koreksi `bbb217c9-23b4-40d0-8ad2-2d7480fd9edb`; tindak lanjut `ca81f180-6671-4c78-b729-959495f0b444`

## Daftar Evidence

- **CASE-015-E01:** `bbb21a3e-6b5c-4218-82cb-6786cdf814a1`; pembicara `user`; stempel waktu `2026-07-27T12:37:02.935905Z`; fungsi: mengatur instruksi/konteks; percakapan `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E02:** `37192b10-28ec-4b5d-b04c-6c6dab4ac3c8`; pembicara `assistant`; stempel waktu `2026-07-27T12:37:03.202118Z`; fungsi: respon bermasalah; percakapan `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E03:** `bbb217c9-23b4-40d0-8ad2-2d7480fd9edb`; pembicara `user`; stempel waktu `2026-07-27T12:37:41.375942Z`; fungsi: koreksi pengguna; percakapan `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.
- **CASE-015-E04:** `ca81f180-6671-4c78-b729-959495f0b444`; pembicara `assistant`; stempel waktu `2026-07-27T12:37:41.588036Z`; fungsi: asisten tindak lanjut; percakapan `6a6743f9-3840-83ec-9fbe-816eb2a7abf0`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-021: mengatur instruksi/konteks (`bbb21a3e-6b5c-4218-82cb-6786cdf814a1` pada 2026-07-27T12:37:02.935905Z).
[[TETAP9]]. PRE-021: respon bermasalah (`37192b10-28ec-4b5d-b04c-6c6dab4ac3c8` pada 2026-07-27T12:37:03.202118Z).
[[TETAP18]]. PRE-021: koreksi pengguna (`bbb217c9-23b4-40d0-8ad2-2d7480fd9edb` pada 2026-07-27T12:37:41.375942Z).
[[TETAP27]]. PRE-021: asisten tindak lanjut (`ca81f180-6671-4c78-b729-959495f0b444` di 2026-07-27T12:37:41.588036Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan

## Severity

**Major** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Bukti mencatat alur kerja evaluasi atau penelitian yang analisis selanjutnya memerlukan teks jawaban lengkap, sedangkan catatan yang dihasilkan mempertahankan label atau ringkasan tanpa isi jawaban lengkap. Koreksi mengidentifikasi bidang yang hilang sebagai material. Hal ini mendukung masalah kelengkapan skema, bukan klaim bahwa label yang dipertahankan tidak akurat.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Catatan tersebut menghilangkan teks jawaban lengkap yang diperlukan evaluasi hilir. **Persyaratan dan penyimpangan.** Dalam skema analisis, label jawaban, skor, atau ringkasan tidak dapat menggantikan teks yang diperlukan untuk memeriksa alasan, kata-kata, dan bukti. Kelalaian ini membuat peninjauan kembali secara struktural menjadi tidak mungkin atau lebih lemah. **Inferensi dan batas.** Arsip menunjukkan hilangnya payload yang diperlukan, bukan kesimpulan tentang alasan kolom tersebut dihapus. Konsekuensinya adalah hilangnya kemampuan untuk diaudit: pengulas tidak dapat secara independen merekonstruksi tanggapan yang dievaluasi hanya dari label saja.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Simpan jawaban lengkap kata demi kata di samping label, skor, dan catatan, lalu validasi bahwa setiap kolom catatan yang diperlukan ada sebelum menutup langkah evaluasi.

### B. Perintah/Mitigasi Pengguna

Saat menugaskan tabel evaluasi, sebutkan bidang hilir yang diperlukan untuk ditinjau nanti; jika kebutuhan tersebut telah dinyatakan, maka ketidakhadiran tersebut tetap merupakan suatu cacat pengiriman dan bukan suatu kelalaian yang terjadi seketika.

### C. Peningkatan Model

Tambahkan validasi skema yang menolak catatan evaluasi yang tidak lengkap dan mempertahankan hash konten atau bidang teks yang tepat untuk setiap respons yang ditinjau.

## Pelajaran untuk Pengguna

Untuk kumpulan data evaluasi, konfirmasikan bahwa pembaca di masa mendatang dapat melihat jawaban pasti yang sedang dinilai. Putusan tanpa teks yang mendasarinya tidak dapat mendukung peninjauan kualitas secara rinci.

## Pelajaran untuk Pengembang

Cakupan regresi harus mengirimkan jawaban, memerlukan label ditambah konten kata demi kata, dan gagal ketika sistem hanya menyimpan skor atau deskripsi singkat. Ini menguji pelestarian, bukan hanya akurasi klasifikasi.

## Kesimpulan Akhir

Kasusnya adalah mengenai catatan yang tidak lengkap, bukan sekedar ringkasan yang kurang rinci. Karena jawaban lengkap diperlukan untuk analisis selanjutnya, ketidakhadiran jawaban tersebut akan mengganggu kemampuan penelusuran meskipun label lainnya berguna.

