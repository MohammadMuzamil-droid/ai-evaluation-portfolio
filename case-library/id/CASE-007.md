# CASE-007 — Perpustakaan Templat JSON dan penyimpangan alur kerja

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

2026-07-17

## Keterlacakan Sumber

- **PRA ID:** PRA-007
- **ID TRIAGE:** dapat dilacak dari `EVENT-0138`
- **Judul Percakapan:** Perpustakaan Templat
- **ID Percakapan:** `6a57d4d3-bff4-83e8-9966-384ed9d41334`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0138`
- **ID Pesan yang Relevan:** asisten `8fc51020-a797-49ec-8138-b68c62641100`; koreksi `ff7a5ca0-7cef-40d7-a3d1-2226c222b29d`; tindak lanjut `f4759725-34b7-45c0-a38e-2d0fc0eda88d`

## Daftar Evidence

- **CASE-007-E01:** `ab0fa726-8246-4477-8494-e45633df9209`; pembicara `user`; stempel waktu `2026-07-17T15:14:47.421000Z`; fungsi: mengatur instruksi/konteks; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E02:** `8fc51020-a797-49ec-8138-b68c62641100`; pembicara `assistant`; stempel waktu `2026-07-17T15:14:49.079363Z`; fungsi: respon bermasalah; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E03:** `ff7a5ca0-7cef-40d7-a3d1-2226c222b29d`; pembicara `user`; stempel waktu `2026-07-17T15:15:53.854000Z`; fungsi: koreksi pengguna; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.
- **CASE-007-E04:** `f4759725-34b7-45c0-a38e-2d0fc0eda88d`; pembicara `assistant`; stempel waktu `2026-07-17T15:15:55.468077Z`; fungsi: asisten tindak lanjut; percakapan `6a57d4d3-bff4-83e8-9966-384ed9d41334`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-007: mengatur instruksi/konteks (`ab0fa726-8246-4477-8494-e45633df9209` pada 2026-07-17T15:14:47.421000Z).
[[TETAP9]]. PRE-007: respon bermasalah (`8fc51020-a797-49ec-8138-b68c62641100` pada 2026-07-17T15:14:49.079363Z).
[[TETAP18]]. PRE-007: koreksi pengguna (`ff7a5ca0-7cef-40d7-a3d1-2226c222b29d` pada 2026-07-17T15:15:53.854000Z).
[[TETAP27]]. PRE-007: asisten tindak lanjut (`f4759725-34b7-45c0-a38e-2d0fc0eda88d` di 2026-07-17T15:15:55.468077Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan; Penggunaan Alat

## Severity

**Major** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Insiden ini berpusat pada pertanyaan JSON multi-bagian tentang alur kerja Perpustakaan Templat. Asisten memperlakukannya sebagai undangan untuk merancang arsitektur baru daripada menjawab pertanyaan operasional yang disajikan. Oleh karena itu, bukti mendukung masalah klasifikasi maksud dan penyimpangan alur kerja, bukan penilaian bahwa diskusi desain selalu tidak tepat.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Respons dipindahkan dari struktur tugas/JSON multi-bagian yang disediakan ke tugas desain baru. **Persyaratan dan penyimpangan.** Permintaan aktif menanyakan cara menangani konfigurasi operasional; jawaban yang diperlukan untuk menafsirkan bidang dan langkah yang diberikan sebelum mengusulkan desain ulang. **Inferensi dan batasan.** Hal ini konsisten dengan penyimpangan niat dari implementasi/menjawab pertanyaan menuju pembuatan arsitektur. Arsip tidak dapat menetapkan pengklasifikasi internal yang bertanggung jawab. Konsekuensinya adalah alur kerja JSON langsung pengguna tetap tidak terjawab meskipun menerima materi desain yang berpotensi relevan.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Jawab pertanyaan JSON multibagian bidang demi bidang, nyatakan tindakan operasional untuk setiap bagian, dan tawarkan desain ulang arsitektur hanya sebagai langkah opsional berikutnya.

### B. Perintah/Mitigasi Pengguna

Awali dengan pertanyaan langsung seperti 'Bagaimana alur kerja JSON ini diproses?' dan tanyakan alternatif desain secara terpisah; konteks multipart yang ada harus tetap menjadi sinyal utama.

### C. Peningkatan Model

Latih dan uji perutean yang membedakan interpretasi konfigurasi, panduan implementasi, dan permintaan desain greenfield ketika istilah domain yang sama muncul di ketiganya.

## Pelajaran untuk Pengguna

Untuk tugas data terstruktur, periksa apakah jawabannya membahas kunci, nilai, dan transisi alur kerja yang disediakan. Proposal desain yang lebih luas dapat bermanfaat namun tidak boleh menggantikan jawaban operasional yang diminta.

## Pelajaran untuk Pengembang

Buat pengujian dengan payload JSON multibagian dan pertanyaan operasional yang sempit. Perilaku passing mengacu pada bagian sebenarnya dari muatan; kegagalan adalah proposal arsitektur umum tanpa resolusi tingkat lapangan.

## Kesimpulan Akhir

Respons yang diberikan mengubah jenis pekerjaan yang dilakukan—dari interpretasi operasional hingga desain. Bukti yang ada membuat pengalihan tersebut terlihat dan mendukung evaluasi perutean tugas, namun tidak mengesampingkan desain sebagai percakapan keikutsertaan di kemudian hari.

