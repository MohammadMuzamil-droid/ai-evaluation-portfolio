# CASE-018 — Asumsi panjang perintah membalikkan arah yang diminta

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](README.md) · [English](../en/CASE-018.md)

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

2026-07-29

## Keterlacakan Sumber

- **PRA ID:** PRA-024
- **ID TRIAGE:** dapat dilacak dari `EVENT-0432`
- **Judul Percakapan:** Perkembangan siswa editor cepat
- **ID Percakapan:** `6a684b13-532c-83ec-aeee-47e456ac72ce`
- **Sumber JSON:** `conversations-000.json`
- **ID Acara:** `EVENT-0432`
- **ID Pesan yang Relevan:** asisten `ce1a7ae1-4f00-4d55-96cd-1550a8271fa8`; koreksi `bbb2173a-3657-4d74-84d0-b5845cc4d269`; tindak lanjut `8f75e155-1fe2-4376-974d-efc66d1d1f1a`

## Daftar Evidence

- **CASE-018-E01:** `bbb21cd1-ebe0-4274-aa66-a1733f6f80c1`; pembicara `user`; stempel waktu `2026-07-29T02:04:44.118437Z`; fungsi: mengatur instruksi/konteks; percakapan `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E02:** `ce1a7ae1-4f00-4d55-96cd-1550a8271fa8`; pembicara `assistant`; stempel waktu `2026-07-29T02:04:44.517557Z`; fungsi: respon bermasalah; percakapan `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E03:** `bbb2173a-3657-4d74-84d0-b5845cc4d269`; pembicara `user`; stempel waktu `2026-07-29T02:05:39.316235Z`; fungsi: koreksi pengguna; percakapan `6a684b13-532c-83ec-aeee-47e456ac72ce`.
- **CASE-018-E04:** `8f75e155-1fe2-4376-974d-efc66d1d1f1a`; pembicara `assistant`; stempel waktu `2026-07-29T02:05:39.606745Z`; fungsi: asisten tindak lanjut; percakapan `6a684b13-532c-83ec-aeee-47e456ac72ce`.

## Konteks Percakapan

Hanya konteks pemerintahan langsung dan pesan insiden di atas yang digunakan.

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Kronologi

[[TETAP0]]. PRE-024: mengatur instruksi/konteks (`bbb21cd1-ebe0-4274-aa66-a1733f6f80c1` pada 2026-07-29T02:04:44.118437Z).
[[TETAP9]]. PRE-024: respon bermasalah (`ce1a7ae1-4f00-4d55-96cd-1550a8271fa8` pada 2026-07-29T02:04:44.517557Z).
[[TETAP18]]. PRE-024: koreksi pengguna (`bbb2173a-3657-4d74-84d0-b5845cc4d269` pada 2026-07-29T02:05:39.316235Z).
[[TETAP27]]. PRE-024: asisten tindak lanjut (`8f75e155-1fe2-4376-974d-efc66d1d1f1a` di 2026-07-29T02:05:39.606745Z).

## Kategori Isu

Mengikuti Instruksi; Kesalahan Pemformatan

## Severity

**Moderate** — tingkat keparahan akhir dipertahankan dari `portfolio-professional-revision-decisions`.

## Ringkasan Evidence

Arsip tersebut berisi Instruksi Proyek lengkap sebelum dan sesudah penulisan ulang, ditambah pernyataan kelayakan, koreksi pengguna, dan permintaan penulisan ulang yang diperbarui. Pengukuran langsung memverifikasi 6,566 ke 5,482 karakter termasuk spasi (−1,084; 16.51% pengurangan), dan 5,558 hingga 4,601 tidak termasuk spasi (−957; 17.22%). Bukti mendukung asumsi panjang yang terbalik; itu tidak mendukung klaim sebelumnya tentang sekitar 40%.

## Evaluasi Pengguna

**Sumber: Keputusan Validasi Manusia** — Keputusan Validasi Manusia: disetujui secara batch karena tidak ambigu; pertahankan evaluasi yang diwakili oleh koreksi arsip tanpa menambahkan opini pengguna baru.

## Analisis Teknis

**Pengamatan.** Sebelum melakukan penulisan ulang, asisten mengatakan bahwa restrukturisasi akan membuat instruksi menjadi lebih panjang meskipun pengguna menginginkannya lebih ringkas. Pasangan mentah selanjutnya menunjukkan arah yang berlawanan: instruksi lengkap yang ditulis ulang adalah 1,084 karakter lebih pendek termasuk spasi. **Persyaratan dan penyimpangan.** Tugas ini memerlukan penulisan ulang penuh berdasarkan preferensi karakter-anggaran, jadi panjangnya seharusnya diukur setelah penyusunan, bukan diasumsikan dari gagasan restrukturisasi. **Inferensi dan batas.** Ini adalah kesalahan asumsi kelayakan yang dapat dibuktikan, bukan bukti bahwa setiap penulisan ulang akan menyusut. Kronologi dan penghitungan yang tepat menyelesaikan konflik validasi sebelumnya tanpa menjelaskan prediksi awal.

## Rekomendasi Perbaikan

### A. Peningkatan Respon

Menyusun seluruh Instruksi Proyek yang telah direvisi, mengukur karakter termasuk spasi, dan menyajikan perbandingan terukur daripada memperkirakan perluasan; mempertahankan teks lengkap sebagai penyampaian utama.

### B. Perintah/Mitigasi Pengguna

Nyatakan arah yang diinginkan—lebih pendek dengan tetap mempertahankan aturan yang diperlukan—dan minta jumlah karakter sebelum/sesudah. Dalam kejadian ini, pengurangan yang terverifikasi menunjukkan bahwa preferensi pengguna dapat dicapai tanpa perubahan yang cepat.

### C. Peningkatan Model

Gunakan pengujian regresi karakter-anggaran dengan pasangan mentah ini: 6,566 sebelum dan 5,482 setelah menyertakan spasi, menolak pernyataan kelayakan yang belum diperiksa terhadap rancangan keluaran penuh.

## Pelajaran untuk Pengguna

Untuk penulisan ulang yang sensitif terhadap panjang, mintalah pengukuran penuh sebelum/sesudah daripada menerima perkiraan. Dalam hal ini, pengurangan 16.51% yang terverifikasi adalah hasil yang relevan, bukan intuisi yang tidak terukur mengenai restrukturisasi.

## Pelajaran untuk Pengembang

Pertahankan perlengkapan regresi yang berisi dua pesan instruksi yang tepat dan hitung jumlah yang menyertakan spasi dan tidak termasuk spasi. Tes tersebut harus membedakan perkiraan dari penulisan ulang terukur yang telah selesai.

## Kesimpulan Akhir

CASE-018 tetap terverifikasi secara kuantitatif: penulisan ulang terakhir mengurangi instruksi lengkap dari karakter 6,566 menjadi 5,482 termasuk spasi. Kasus ini menunjukkan mengapa kelayakan panjang harus diukur pada artefak jadi; ia tidak membuat klaim tentang tingkat kompresi universal.

