# CASE-011 — Pembatasan pilihan ganda yang diciptakan

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-011.md)

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

2026-07-22

## Keterlacakan Sumber

- **PRA ID:** PRA-013
- **ID TRIAGE:** dapat dilacak dari `EVENT-0246`
- **Judul Percakapan:** Anontasi data
- **ID Percakapan:** `6a5fab6f-6cf8-83ee-8a04-960e18d40895`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0246`
- **ID Pesan yang Relevan:** asisten `340ff6dc-dbf7-4b4b-ad00-bb841550e649`; koreksi `bbb21e2b-73f4-4c86-899a-88da2e697bee`; tindak lanjut `0509f710-fb8e-4fbc-998c-3ea059fdf4f2`

## Daftar Evidence

- **CASE-011-E01:** `bbb21ba9-1a30-42ce-9c4f-12793bdabda2`; pembicara `user`; stempel waktu `2026-07-22T00:27:47.135599Z`; fungsi: mengatur instruksi/konteks; percakapan `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E02:** `340ff6dc-dbf7-4b4b-ad00-bb841550e649`; pembicara `assistant`; stempel waktu `2026-07-22T00:27:47.481355Z`; fungsi: respon bermasalah; percakapan `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E03:** `bbb21e2b-73f4-4c86-899a-88da2e697bee`; pembicara `user`; stempel waktu `2026-07-22T00:28:35.166404Z`; fungsi: koreksi pengguna; percakapan `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.
- **CASE-011-E04:** `0509f710-fb8e-4fbc-998c-3ea059fdf4f2`; pembicara `assistant`; stempel waktu `2026-07-22T00:28:35.801158Z`; fungsi: asisten tindak lanjut; percakapan `6a5fab6f-6cf8-83ee-8a04-960e18d40895`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-013: mengatur instruksi/konteks (`bbb21ba9-1a30-42ce-9c4f-12793bdabda2` pada 2026-07-22T00:27:47.135599Z).
[[TETAP9]]. PRE-013: respon bermasalah (`340ff6dc-dbf7-4b4b-ad00-bb841550e649` pada 2026-07-22T00:27:47.481355Z).
[[TETAP18]]. PRE-013: koreksi pengguna (`bbb21e2b-73f4-4c86-899a-88da2e697bee` pada 2026-07-22T00:28:35.166404Z).
[[TETAP27]]. PRE-013: asisten tindak lanjut (`0509f710-fb8e-4fbc-998c-3ea059fdf4f2` di 2026-07-22T00:28:35.801158Z).

## Kategori Isu

Halusinasi; Instruksi Mengikuti

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Alur kerja evaluasi yang dipertahankan mencakup konteks pedoman A/B/C/D dan respons yang memperkenalkan batasan pilihan ganda yang tidak disediakan oleh aturan aktif. Tantangan koreksi yang disisipkan restriksi. Bukti yang ada lebih mendukung temuan kendala yang tidak didukung dibandingkan dengan klaim bahwa pedoman yang mendasarinya tidak memiliki batasan yang sah.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Asisten memperlakukan batasan seolah-olah itu milik rubrik A/B/C/D yang aktif meskipun pedoman yang diberikan tidak menetapkannya. **Persyaratan dan penyimpangan.** Seorang evaluator harus membedakan kriteria tertulis dari asumsi yang terdengar masuk akal. Menambahkan aturan akan mengubah jawaban mana yang dapat dipertimbangkan dan karenanya mengubah evaluasi. **Inferensi dan batas.** Arsip menunjukkan error penyisipan batasan, bukan sumber asumsi tersebut. Pentingnya hal ini bersifat prosedural: pembatasan yang dibuat-buat dapat membatalkan penilaian namun terkesan lebih ketat.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Mengutip atau memparafrasekan rubrik peraturan sebelum menerapkan pembatasan, dan jika aturan yang diperlukan tidak ada, mintalah klarifikasi daripada membuat aturan.

### B. Perintah/Mitigasi Pengguna

Berikan kutipan rubrik yang relevan dengan petunjuk evaluasi jika memungkinkan; pengguna tidak perlu bertahan terhadap kendala yang tidak ada dalam pedoman yang disebutkan.

### C. Peningkatan Model

Kembangkan deteksi aturan yang tidak didukung yang membandingkan setiap batasan yang ditetapkan dengan alasan terhadap set instruksi aktif dan menandai klaim yang tidak cocok.

## Pelajaran untuk Pengguna

Saat menerima alasan evaluasi, tanyakan kalimat rubrik mana yang memberi wewenang pada setiap aturan diskualifikasi. Hal ini sangat berguna ketika aturan mempersempit pilihan jawaban yang tersedia.

## Pelajaran untuk Pengembang

Perlengkapan contoh tandingan harus menampilkan rubrik dengan label A/B/C/D tetapi menghilangkan dugaan pembatasan. Melewati keluaran mengidentifikasi kelalaian; kegagalan memperlakukan kondisi yang diciptakan sebagai sesuatu yang mengikat.

## Kesimpulan Akhir

Masalah yang terdokumentasi bukanlah ketidaksepakatan mengenai pilihan jawaban namun aturan tambahan yang dimasukkan ke dalam proses penjurian. Koreksi ini menjadikan ketiadaan aturan tersebut sebagai hal yang penting, sementara arsip tidak dapat menentukan dari mana asumsi tersebut berasal.

