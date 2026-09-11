# CASE-002 — Saran CV yang kontradiktif tentang klaim yang dapat didukung

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

2026-07-09

## Keterlacakan Sumber

- **PRA ID:** PRA-002
- **ID TRIAGE:** dapat dilacak dari `EVENT-0033`
- **Judul Percakapan:** Buat gambar
- **ID Percakapan:** `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0033`
- **ID Pesan yang Relevan:** asisten `523a35b7-1741-48db-8e66-db15a1324899`; koreksi `bbb21b3e-8f22-406a-b3ea-8be79021b22e`; tindak lanjut `8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6`

## Daftar Evidence

- **CASE-002-E01:** `bbb21e5d-dd3b-45ec-8134-14f84b08e903`; pembicara `user`; stempel waktu `2026-07-09T21:46:10.199103Z`; fungsi: mengatur instruksi/konteks; percakapan `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E02:** `523a35b7-1741-48db-8e66-db15a1324899`; pembicara `assistant`; stempel waktu `2026-07-09T21:46:10.546755Z`; fungsi: respon bermasalah; percakapan `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E03:** `bbb21b3e-8f22-406a-b3ea-8be79021b22e`; pembicara `user`; stempel waktu `2026-07-09T21:47:56.998648Z`; fungsi: koreksi pengguna; percakapan `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.
- **CASE-002-E04:** `8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6`; pembicara `assistant`; stempel waktu `2026-07-09T21:47:57.368687Z`; fungsi: asisten tindak lanjut; percakapan `6a4fe3f1-d02c-83ee-ba44-9d7f455f2dcf`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: saran tersebut menghadirkan potensi risiko klaim platform yang tidak didukung/tidak sesuai; tidak ada pelanggaran kebijakan aktual yang dinyatakan.

## Kronologi

[[TETAP0]]. PRE-002: mengatur instruksi/konteks (`bbb21e5d-dd3b-45ec-8134-14f84b08e903` pada 2026-07-09T21:46:10.199103Z).
[[TETAP9]]. PRE-002: respon bermasalah (`523a35b7-1741-48db-8e66-db15a1324899` pada 2026-07-09T21:46:10.546755Z).
[[TETAP18]]. PRE-002: koreksi pengguna (`bbb21b3e-8f22-406a-b3ea-8be79021b22e` pada 2026-07-09T21:47:56.998648Z).
[[TETAP27]]. PRE-002: asisten tindak lanjut (`8aa2c1c7-ce61-4ec5-8386-447eca1e5ed6` di 2026-07-09T21:47:57.368687Z).

## Kategori Isu

Kontradiksi; Inkonsistensi; Asumsi yang Salah

## Severity

**Major** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Urutan saran CV yang disimpan menyandingkan rekomendasi tentang klaim yang harus didukung dengan kata-kata yang dapat mendorong platform atau klaim pengalaman yang tidak didukung. Penilaian validasi pengguna menggambarkan hal ini sebagai potensi risiko, bukan pelanggaran kebijakan yang terbukti. Bukti mendukung pengujian konsistensi saran, bukan dugaan adanya pelanggaran eksternal yang sebenarnya.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: saran tersebut menghadirkan potensi risiko klaim platform yang tidak didukung/tidak sesuai; tidak ada pelanggaran kebijakan aktual yang dinyatakan.

## Analisis Teknis

**Pengamatan.** Saran tersebut membedakan kualifikasi yang didukung bukti dari klaim yang memerlukan dukungan, namun bagian lain mengusulkan bahasa yang dukungannya tidak ditetapkan dalam konteks yang diberikan. **Persyaratan dan penyimpangan.** Rekomendasi CV harus menggunakan pengalaman yang ditunjukkan atau memberi label keterampilan yang diusulkan sebagai tujuan pembelajaran; ia tidak dapat menerapkan standar bukti yang lebih ketat secara selektif. **Inferensi dan batasan.** Pertukaran tersebut menunjukkan logika rekomendasi yang bertentangan, bukan bukti bahwa pengguna akan mengirimkan CV palsu atau melanggar kebijakan platform. Kerugian praktisnya adalah bahwa seorang pembelajar mungkin menyalin sebuah frasa halus yang menurut nasihat di sekitarnya harus dibuktikan.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Tulis ulang panduan CV ke dalam dua wadah berlabel—pengalaman terverifikasi dan tujuan pengembangan masa depan—dan hilangkan atau kualifikasikan kalimat apa pun yang tidak memiliki bukti pendukung.

### B. Perintah/Mitigasi Pengguna

Berikan daftar singkat proyek yang telah selesai, alat yang digunakan, dan hasil yang dapat dibuktikan sebelum meminta kata-kata CV; apabila materi itu sudah diberikan, hendaknya Pembantu tidak diam-diam menurunkan standar pembuktiannya.

### C. Peningkatan Model

Evaluasi respons penulisan karier untuk mengetahui konsistensi antara aturan peringatan dan klaim yang disarankan, termasuk pemeriksaan kontradiksi untuk referensi produk, kredensial, atau platform yang tidak dapat diverifikasi.

## Pelajaran untuk Pengguna

Perlakukan saran CV sebagai inventaris klaim: tanyakan pekerjaan, artefak, atau hasil nyata apa yang memungkinkan kandidat mempertahankan setiap barisnya. Kemampuan aspirasional merupakan bagian dari rencana pengembangan, bukan secara otomatis berdasarkan pengalaman.

## Pelajaran untuk Pengembang

Gunakan tes berpasangan di mana asisten memperingatkan terhadap klaim yang tidak didukung dan kemudian menerima undangan untuk membuat drafnya. Perilaku yang diharapkan adalah mempertahankan peringatan tersebut dan menawarkan alternatif yang jelas berorientasi masa depan.

## Kesimpulan Akhir

Bukti menunjukkan nasihat yang pada prinsipnya hati-hati namun berpotensi permisif dalam penerapannya. Karena penilaian pengguna tidak menyatakan adanya pelanggaran kebijakan yang telah selesai, maka kasus yang paling kuat adalah masalah konsistensi dan dukungan klaim, bukan tuduhan kepatuhan.

