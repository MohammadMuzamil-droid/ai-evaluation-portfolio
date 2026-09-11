# CASE-027 — Struktur pedoman-pelatihan diratakan

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

2026-08-11

## Keterlacakan Sumber

- **PRA ID:** PRA-033
- **ID TRIAGE:** dapat dilacak dari `EVENT-0947`
- **Judul Percakapan:** Peringkat Cabang Bab 4.
- **ID Percakapan:** `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`
- **Sumber JSON:** `conversations-001.json`
- **ID Acara:** `EVENT-0947`
- **ID Pesan yang Relevan:** asisten `0ff7c441-7bff-48a5-95bb-5fff990cf823`; koreksi `bbb21011-1743-4a38-b382-3476ccbdeefc`; tindak lanjut `f8c944eb-af19-444b-badf-8cd93a9fa0d6`

## Daftar Evidence

- **CASE-027-E01:** `bbb2147a-877b-4852-9e35-ad973e0a4539`; pembicara `user`; stempel waktu `2026-08-11T03:54:14.849810Z`; fungsi: mengatur instruksi/konteks; percakapan `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E02:** `0ff7c441-7bff-48a5-95bb-5fff990cf823`; pembicara `assistant`; stempel waktu `2026-08-11T03:54:15.248598Z`; fungsi: respon bermasalah; percakapan `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E03:** `bbb21011-1743-4a38-b382-3476ccbdeefc`; pembicara `user`; stempel waktu `2026-08-11T03:57:57.477553Z`; fungsi: koreksi pengguna; percakapan `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.
- **CASE-027-E04:** `f8c944eb-af19-444b-badf-8cd93a9fa0d6`; pembicara `assistant`; stempel waktu `2026-08-11T03:57:57.980883Z`; fungsi: asisten tindak lanjut; percakapan `6a7a835c-26b8-83ec-bd9a-99ed40fd3195`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: Kemajuan 1 dan 2 masing-masing berisi Pedoman 1/2; Kemajuan 3+ membuat pedoman sebelum setiap pertanyaan diajukan.

## Kronologi

[[TETAP0]]. PRE-033: mengatur instruksi/konteks (`bbb2147a-877b-4852-9e35-ad973e0a4539` pada 2026-08-11T03:54:14.849810Z).
[[TETAP9]]. PRE-033: respon bermasalah (`0ff7c441-7bff-48a5-95bb-5fff990cf823` pada 2026-08-11T03:54:15.248598Z).
[[TETAP18]]. PRE-033: koreksi pengguna (`bbb21011-1743-4a38-b382-3476ccbdeefc` pada 2026-08-11T03:57:57.477553Z).
[[TETAP27]]. PRE-033: asisten tindak lanjut (`f8c944eb-af19-444b-badf-8cd93a9fa0d6` di 2026-08-11T03:57:57.980883Z).

## Kategori Isu

Mengikuti Instruksi; Penanganan Konteks

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Bukti-bukti tersebut menggambarkan alur kerja pelatihan pedoman yang hierarkis: pola dua pedoman hanya berlaku untuk Kemajuan 1 dan 2, sedangkan siklus pertanyaan selanjutnya memerlukan pedoman sebelum setiap siklus. Tanggapannya meratakan aturan khusus tahapan tersebut. Bukti mendukung kegagalan penanganan hierarki/pengecualian, bukan klaim bahwa satu alur kerja sederhana tidak akan pernah berguna di tempat lain.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: Kemajuan 1 dan 2 masing-masing berisi Pedoman 1/2; Kemajuan 3+ membuat pedoman sebelum setiap pertanyaan diajukan.

## Analisis Teknis

**Pengamatan.** Respons yang diberikan adalah dengan menggeneralisasi pola dua pedoman awal pada tahap kemajuan selanjutnya, dan bukan menerapkan persyaratan pedoman per siklus yang dinyatakan. **Persyaratan dan penyimpangan.** Alur kerja memiliki pola dasar ditambah pengecualian yang bergantung pada tahapan; pelaksanaan yang benar bergantung pada pelestarian struktur umum dan batas perubahannya. Meratakan hierarki akan menghapus aturan selanjutnya. **Inferensi dan batas.** Arsip menunjukkan kegagalan penanganan pengecualian dalam urutan ini, bukan alasan hilangnya perbedaan tahapan. Konsekuensinya adalah penentuan waktu pedoman yang tidak tepat untuk siklus pembelajaran berikutnya.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Terapkan pengaturan dua pedoman hanya pada Kemajuan 1 dan 2, lalu buat atau aktifkan pedoman sebelum setiap siklus pertanyaan selanjutnya seperti yang ditentukan.

### B. Perintah/Mitigasi Pengguna

Sajikan alur kerja sebagai tabel tahapan kecil—Kemajuan 1–2 versus siklus selanjutnya—saat menyerahkannya kepada asisten, sambil menyadari bahwa struktur yang dibedakan sudah menjadi bagian dari persyaratan yang divalidasi.

### C. Peningkatan Model

Uji instruksi hierarki berikut dengan aturan umum, pengecualian tahap eksplisit, dan beberapa siklus berikutnya; pemberian skor harus menghukum interpretasi satu aturan yang diratakan.

## Pelajaran untuk Pengguna

Untuk prosedur bertahap, periksa batas pengecualian, bukan hanya pola pertama yang diulang. Pertanyaan tinjauan yang paling penting sering kali adalah kapan aturan yang sudah lazim tidak lagi berlaku.

## Pelajaran untuk Pengembang

Kasus regresi harus dijalankan melalui Kemajuan 1, Kemajuan 2, dan dua siklus berikutnya. Melewati perilaku mengubah waktu pedoman setelah tahap awal dan mempertahankan perubahan itu pada setiap siklus selanjutnya.

## Kesimpulan Akhir

Kegagalan tersebut bukanlah pedoman yang hilang secara abstrak; hilangnya aturan khusus tahapan yang mengubah alur kerja setelah Kemajuan 2. Bukti mendukung ketidakcocokan hierarki tersebut, namun tetap membiarkan bagaimana model mewakili prosedur secara internal.

