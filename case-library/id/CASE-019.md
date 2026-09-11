# CASE-019 — Pemetaan nama resmi tidak digunakan

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

2026-07-29

## Keterlacakan Sumber

- **PRA ID:** PRA-025
- **ID TRIAGE:** dapat dilacak dari `EVENT-0469`
- **Judul Percakapan:** Proyek Progres Muhafadhoh
- **ID Percakapan:** `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0469`
- **ID Pesan yang Relevan:** asisten `3b2df342-a8c2-4e42-ac21-da81e3f063c6`; koreksi `bbb219f0-84a1-445f-bb06-001d4091fa70`; tindak lanjut `26860c01-fb8f-4965-8650-607c831860c8`

## Daftar Evidence

- **CASE-019-E01:** `bbb21998-b53a-4170-98b4-03ec70bd1c3c`; pembicara `user`; stempel waktu `2026-07-29T12:19:41.181159Z`; fungsi: mengatur instruksi/konteks; percakapan `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E02:** `3b2df342-a8c2-4e42-ac21-da81e3f063c6`; pembicara `assistant`; stempel waktu `2026-07-29T12:19:43.472699Z`; fungsi: respon bermasalah; percakapan `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E03:** `bbb219f0-84a1-445f-bb06-001d4091fa70`; pembicara `user`; stempel waktu `2026-07-29T12:20:39.071314Z`; fungsi: koreksi pengguna; percakapan `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.
- **CASE-019-E04:** `26860c01-fb8f-4965-8650-607c831860c8`; pembicara `assistant`; stempel waktu `2026-07-29T12:20:47.185016Z`; fungsi: asisten tindak lanjut; percakapan `6a69efb1-d37c-83ec-b195-1c36ce3f5c62`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: Absen Resmi adalah sumber kebenaran untuk nama yang ditampilkan; nama buku setoran hanya untuk pencocokan saja.

## Kronologi

[[TETAP0]]. PRE-025: mengatur instruksi/konteks (`bbb21998-b53a-4170-98b4-03ec70bd1c3c` pada 2026-07-29T12:19:41.181159Z).
[[TETAP9]]. PRE-025: respon bermasalah (`3b2df342-a8c2-4e42-ac21-da81e3f063c6` pada 2026-07-29T12:19:43.472699Z).
[[TETAP18]]. PRE-025: koreksi pengguna (`bbb219f0-84a1-445f-bb06-001d4091fa70` pada 2026-07-29T12:20:39.071314Z).
[[TETAP27]]. PRE-025: asisten tindak lanjut (`26860c01-fb8f-4965-8650-607c831860c8` di 2026-07-29T12:20:47.185016Z).

## Kategori Isu

Penanganan Konteks; Asumsi yang Salah; Persyaratan Tidak Ada

## Severity

**Major** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Hirarki sumber yang dipertahankan mengidentifikasi alias operasional, Absen Setoran, lapisan Pemetaan, dan nama tampilan resmi Absen Resmi. Responsnya tidak menerapkan pemetaan tersebut sebelum memilih identitas yang ditampilkan. Bukti tersebut mendukung kesalahan penyelesaian entitas, bukan klaim bahwa alias itu sendiri tidak valid dalam konteks operasionalnya.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: Absen Resmi adalah sumber kebenaran untuk nama yang ditampilkan; nama buku setoran hanya untuk pencocokan saja.

## Analisis Teknis

**Pengamatan.** Asisten memilih atau mempertahankan label operasional tanpa melintasi Pemetaan yang disediakan ke nama resmi. **Persyaratan dan penyimpangan.** Jika hierarki secara eksplisit membedakan alias, pemetaan, dan identitas tampilan resmi, penamaan keluaran harus diselesaikan melalui rantai tersebut sebelum presentasi. **Inferensi dan batas.** Urutan ini menunjukkan kegagalan penggunaan pemetaan yang tersedia; itu tidak menentukan penyebab kegagalan resolusi atau membatalkan alias sumber. Konsekuensinya adalah pemberian label resmi yang tidak tepat dalam konteks yang mementingkan otoritas nama.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Selesaikan Absen Setoran melalui catatan Pemetaan dan tampilkan Absen Resmi sebagai nama resmi, secara opsional tetap mempertahankan alias dalam tanda kurung agar dapat ditelusuri.

### B. Perintah/Mitigasi Pengguna

Berikan pemetaan alias-ke-resmi di dekat permintaan ketika beberapa nama hidup berdampingan; setelah pemetaan tersebut diberikan, pengguna tidak perlu mengulangi nama mana yang otoritatif.

### C. Peningkatan Model

Tambahkan pengujian resolusi entitas yang mengharuskan sistem mempertahankan alias operasional dan nama tampilan kanonik sambil memilih bentuk kanonik untuk hasil akhir.

## Pelajaran untuk Pengguna

Ketika alur kerja berisi beberapa nama untuk satu item, identifikasikan kontrol lapisan mana yang ditampilkan. Sebuah alias mungkin berguna untuk pencarian namun tetap salah untuk label resminya.

## Pelajaran untuk Pengembang

Catatan regresi harus menyertakan alias, pemetaan, dan nama resmi dengan bentuk permukaan yang bertentangan. Melewati keluaran mengikuti pemetaan dan menjelaskan alias yang dipertahankan hanya sebagai konteks.

## Kesimpulan Akhir

Kesalahannya adalah kegagalan spesifik untuk mengikuti rantai penamaan yang berwenang. Arsip tersebut menunjukkan rute yang diperlukan dari Absen Setoran ke Absen Resmi, namun tidak berarti bahwa setiap penggunaan alias operasional salah.

