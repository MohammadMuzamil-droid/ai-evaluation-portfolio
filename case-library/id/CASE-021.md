# CASE-021 — EKSTRAK menghasilkan ringkasan PDF

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-021.md)

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

2026-07-31

## Keterlacakan Sumber

- **PRA ID:** PRA-027
- **ID TRIAGE:** dapat dilacak dari `EVENT-0510`
- **Judul Percakapan:** Pembelajaran DOLA Web Search
- **ID Percakapan:** `6a6b508e-8c68-83ec-bc9e-207be38c8039`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0510`
- **ID Pesan yang Relevan:** asisten `b0448e02-aa19-4645-b819-b477b1ce06f5`; koreksi `bbb21e81-8b18-41e7-8952-c0f072400691`; tindak lanjut `4fa6fa74-46a4-4724-a79f-5d2398cd0c42`

## Daftar Evidence

- **CASE-021-E01:** `bbb21f84-c99e-44d2-b798-18fdff8263c9`; pembicara `user`; stempel waktu `2026-07-31T04:19:57.654775Z`; fungsi: mengatur instruksi/konteks; percakapan `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E02:** `b0448e02-aa19-4645-b819-b477b1ce06f5`; pembicara `assistant`; stempel waktu `2026-07-31T04:20:07.865488Z`; fungsi: respon bermasalah; percakapan `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E03:** `bbb21e81-8b18-41e7-8952-c0f072400691`; pembicara `user`; stempel waktu `2026-07-31T04:21:09.065567Z`; fungsi: koreksi pengguna; percakapan `6a6b508e-8c68-83ec-bc9e-207be38c8039`.
- **CASE-021-E04:** `4fa6fa74-46a4-4724-a79f-5d2398cd0c42`; pembicara `assistant`; stempel waktu `2026-07-31T04:21:23.473186Z`; fungsi: asisten tindak lanjut; percakapan `6a6b508e-8c68-83ec-bc9e-207be38c8039`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-027: mengatur instruksi/konteks (`bbb21f84-c99e-44d2-b798-18fdff8263c9` pada 2026-07-31T04:19:57.654775Z).
[[TETAP9]]. PRE-027: respon bermasalah (`b0448e02-aa19-4645-b819-b477b1ce06f5` pada 2026-07-31T04:20:07.865488Z).
[[TETAP18]]. PRE-027: koreksi pengguna (`bbb21e81-8b18-41e7-8952-c0f072400691` pada 2026-07-31T04:21:09.065567Z).
[[TETAP27]]. PRE-027: asisten tindak lanjut (`4fa6fa74-46a4-4724-a79f-5d2398cd0c42` di 2026-07-31T04:21:23.473186Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan; Penggunaan Alat

## Severity

**Major** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Perintah EXTRACT yang disimpan memerlukan penyimpanan keluaran terbaru, sementara asisten menghasilkan ringkasan PDF yang menghilangkan atau mengubah materi alih-alih menyimpannya. Koreksi berfokus pada semantik EKSTRAK. Bukti mendukung temuan kerugian tanpa menyatakan bahwa ringkasan tidak pernah berguna jika diminta secara eksplisit.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Meminta EKSTRAK akan menghasilkan PDF yang diringkas, bukannya menyimpan hasil terbaru dengan setia. **Persyaratan dan penyimpangan.** Dalam alur kerja ini, EXTRACT berarti meneruskan materi sumber; ringkasan mengubah pilihan, kata-kata, dan kemungkinan penghilangan. PDF yang dipoles tidak setara dengan ekstrak ketika pelestarian adalah kontrak perintah. **Inferensi dan batas.** Catatan menunjukkan substitusi semantik dari preservasi ke kondensasi. Itu tidak menghitung setiap bagian yang hilang kecuali dibandingkan baris demi baris. Konsekuensinya adalah artefak yang diekspor tidak dapat berfungsi sebagai catatan asli sumber yang diminta.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Buat ekstrak yang mereproduksi keluaran terbaru tanpa meringkasnya, dan beri label sinopsis terpisah sebagai artefak opsional yang berbeda.

### B. Perintah/Mitigasi Pengguna

Tentukan 'ekstrak kata demi kata/keluaran terbaru' ketika pengguna hilir memerlukan pelestarian yang tepat, sedangkan perintah EXTRACT yang sudah ada seharusnya sudah diterapkan setelah ditentukan.

### C. Peningkatan Model

Tambahkan perbandingan sumber-ke-ekspor untuk perintah pelestarian, pengiriman gagal ketika konten diringkas, disusun ulang, atau dihilangkan tanpa permintaan transformasi eksplisit.

## Pelajaran untuk Pengguna

Untuk perintah pelestarian, bandingkan sumber dan hasilnya daripada menilai hanya apakah hasilnya terlihat bagus. Ringkasan dapat berguna namun tetap menjadi artefak yang salah.

## Pelajaran untuk Pengembang

Uji regresi harus memanggil EXTRACT pada respons multi-bagian dan membandingkan file yang dihasilkan dengan respons tersebut untuk mengetahui adanya kelalaian. Ringkasan PDF harus diklasifikasikan sebagai operasi yang berbeda.

## Kesimpulan Akhir

Kasus ini mengaktifkan semantik perintah: EXTRACT memerlukan fidelitas, tetapi responsnya menghasilkan kondensasi. Bukti mendukung ketidakcocokan pelestarian, sementara inventarisasi terperinci dari setiap baris yang dihilangkan memerlukan perbedaan file sumber yang terpisah.

