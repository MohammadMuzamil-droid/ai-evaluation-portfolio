# CASE-001 — Penerapan instruksi kata 25 yang tidak konsisten

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-001.md)

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

2026-07-07

## Keterlacakan Sumber

- **PRA ID:** PRA-001
- **ID TRIAGE:** dapat dilacak dari `EVENT-0007`
- **Judul Percakapan:** Peluang Karir di AI
- **ID Percakapan:** `6a4bf6ab-5f08-83e8-afac-905a76388b09`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0007`
- **ID Pesan yang Relevan:** asisten `1a618ee5-1be4-45b4-8e01-cde97f2ffed6`; koreksi `bbb21bb5-6d99-4ef4-9bb3-b06c95741f41`; tindak lanjut `7cef39b9-7da4-4c48-b7ca-da121b016537`

## Daftar Evidence

- **CASE-001-E01:** `bbb2162e-4d3b-4c3d-a0d8-d04421d13ab3`; pembicara `user`; stempel waktu `2026-07-07T12:41:01.238962Z`; fungsi: mengatur instruksi/konteks; percakapan `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E02:** `1a618ee5-1be4-45b4-8e01-cde97f2ffed6`; pembicara `assistant`; stempel waktu `2026-07-07T12:41:01.527613Z`; fungsi: respon bermasalah; percakapan `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E03:** `bbb21bb5-6d99-4ef4-9bb3-b06c95741f41`; pembicara `user`; stempel waktu `2026-07-07T12:42:47.168915Z`; fungsi: koreksi pengguna; percakapan `6a4bf6ab-5f08-83e8-afac-905a76388b09`.
- **CASE-001-E04:** `7cef39b9-7da4-4c48-b7ca-da121b016537`; pembicara `assistant`; stempel waktu `2026-07-07T12:42:47.479027Z`; fungsi: asisten tindak lanjut; percakapan `6a4bf6ab-5f08-83e8-afac-905a76388b09`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: kata-kata persis-25 harus diterapkan secara konsisten.

## Kronologi

[[TETAP0]]. PRE-001: mengatur instruksi/konteks (`bbb2162e-4d3b-4c3d-a0d8-d04421d13ab3` pada 2026-07-07T12:41:01.238962Z).
[[TETAP9]]. PRE-001: respon bermasalah (`1a618ee5-1be4-45b4-8e01-cde97f2ffed6` pada 2026-07-07T12:41:01.527613Z).
[[TETAP18]]. PRE-001: koreksi pengguna (`bbb21bb5-6d99-4ef4-9bb3-b06c95741f41` pada 2026-07-07T12:42:47.168915Z).
[[TETAP27]]. PRE-001: asisten tindak lanjut (`7cef39b9-7da4-4c48-b7ca-da121b016537` di 2026-07-07T12:42:47.479027Z).

## Kategori Isu

Mengikuti Instruksi; Inkonsistensi

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Empat pesan yang disimpan merekam perselisihan instruksi numerik: pengguna memberikan frasa “dalam 25 kata”, asisten memperlakukan latihan sebagai tugas dengan batas maksimum 25 kata, pengguna menantang pembacaan tersebut, dan tindak lanjut menerima interpretasi tepat 25 kata. Oleh karena itu, bukti mendukung ketidakkonsistenan dalam penerapan aturan penilaian yang disebutkan, bukan klaim tentang status model internal.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: kata-kata persis-25 harus diterapkan secara konsisten.

## Analisis Teknis

**Observasi.** Jawaban yang diberikan kontras antara “dalam 25 kata” dengan “maksimal 25 kata” namun kemudian mengakui bahwa penilaian sebelumnya telah menerapkan aturan terakhir pada kata-kata sebelumnya. **Persyaratan dan penyimpangan.** Untuk latihan seperti yang tertulis, kedua jawaban kandidat terlebih dahulu memerlukan pemeriksaan kata-25yang sama persis; gerbang itu dilewati ketika satu jawaban secara efektif ditangani secara maksimal. **Inferensi dan batasan.** Ini adalah bukti penerapan aturan yang tidak stabil dalam penjelasan penilaian. Hal ini tidak menjelaskan mengapa interpretasi tersebut berubah secara internal. Konsekuensinya penting karena keputusan awal yang mengikuti instruksi berubah sebelum perbandingan kualitas dapat dimulai.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Skor ulang kedua jawaban dengan menghitung kata-katanya berdasarkan 25, nyatakan gerbang gagal untuk masing-masing jawaban, dan baru kemudian diskusikan perbedaan kualitas sekunder.

### B. Perintah/Mitigasi Pengguna

Saat meminta latihan, mintalah jumlah kata yang ditampilkan di samping setiap jawaban kandidat sehingga catatan penilaian dapat diaudit; ini membuat cek terlihat tetapi tidak memperbaiki ketidakkonsistenan aslinya.

### C. Peningkatan Model

Tambahkan pengujian status rubrik di mana 'tepat', 'maksimum', dan 'minimum' adalah operator yang berbeda dan mengharuskan operator yang dipilih untuk digaungkan dalam alasan pemberian skor.

## Pelajaran untuk Pengguna

Untuk tugas penghitungan tetap, verifikasi penghitungan sebelum menerima peringkat kualitatif. Di sini pemeriksaan kuncinya bukanlah apakah suatu jawaban terdengar lebih baik, namun apakah masing-masing kandidat memenuhi kondisi numerik yang sama persis.

## Pelajaran untuk Pengembang

Contoh regresi harus memasukkan frasa “dalam 25 kata” ditambah dua kandidat bukan kata -25, lalu menegaskan bahwa tidak ada yang lolos dari instruksi berikut dan bahwa alasannya tidak pernah menggantikan aturan maksimum.

## Kesimpulan Akhir

Kasus ini berkaitan dengan pembalikan skor tertentu: instruksi penghitungan tepat pada awalnya dianalisis sebagai batas atas. Koreksi dan tindak lanjut membuat ketidakcocokan dapat dilacak, sementara arsip tidak mengetahui penyebab utamanya. Nilai profesionalnya adalah urutan gerbang evaluasi yang jelas: kepatuhan terhadap batasan mendahului kualitas komparatif.

