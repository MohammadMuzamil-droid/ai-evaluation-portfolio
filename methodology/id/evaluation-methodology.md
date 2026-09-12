# Metodologi Evaluasi

[Beranda portofolio](../../README-ID.md) · [Pustaka kasus](../../case-library/id/README.md) · [Temuan](../../reports/id/findings.md) · [Pemetaan evidence](../../evidence/README-ID.md) · [English](../en/evaluation-methodology.md)

## Tujuan dan Ruang Lingkup

Metode ini mendukung peninjauan berbasis evidence terhadap 27 kasus ChatGPT Go yang terdokumentasi. Metode ini tidak mengukur prevalensi kegagalan, membandingkan paket atau model, menguji setiap fitur produk, atau memeriksa proses internal model.

## Rekonstruksi Kasus

Setiap kasus direkonstruksi berdasarkan requirement aktif, respons yang diamati, koreksi atau evaluasi, dan tindak lanjut yang relevan. Catatan percakapan primer memberikan kronologi dan keterlacakan tingkat pesan. Portofolio publik tidak mereproduksi screenshot privat atau evidence mentah yang sensitif.

## Keterlacakan Evidence

Setiap kasus publik mempertahankan percakapan sumber, identifier event, identifier pesan yang relevan, dan Daftar Evidence. ID evidence menghubungkan narasi kasus dengan arsip privat tanpa membuka arsip tersebut. Pemetaan yang dipublikasikan memuat 132 referensi evidence tervalidasi.

## Memisahkan Evidence dan Interpretasi

- **Evidence:** catatan sumber yang dipertahankan untuk mendukung apa yang terjadi.
- **Konteks Percakapan:** materi sekitar yang digunakan untuk merekonstruksi requirement aktif.
- **Evaluasi Pengguna:** penilaian manusia yang disetujui dan diberi label sesuai perannya.
- **Analisis Teknis:** interpretasi terbatas tentang requirement, penyimpangan, dan dampak.

Observasi bukan klaim tentang penyebab internal. Inferensi tetap diberi label dan dibatasi ketika sumber tidak dapat membuktikan mekanismenya.

## Validasi Manusia dan Severity

Keputusan manusia menyelesaikan inklusi kasus, konsolidasi, wording Evaluasi Pengguna, dan severity yang disetujui. Severity dipertahankan melalui tahap revisi berikutnya kecuali kontradiksi faktual memerlukan peninjauan. Distribusi yang dipublikasikan adalah 3 Minor, 14 Moderate, 10 Major, dan 0 Critical.

## Konsolidasi dan Deduplicasi

Duplikat teknis dari branch atau export dibedakan dari beberapa koreksi yang termasuk dalam satu insiden. Event terkait hanya dikonsolidasikan ketika logika insiden yang disetujui mendukung satu kasus. Secara khusus, logika konsolidasi CASE-008, CASE-009, dan CASE-014 tetap dipertahankan.

## Corrective dan Independent QC

Working layer melewati corrective QC, second corrective revision, independent re-validation, dan targeted correction verification. Verifikasi tertarget memulihkan teks Evaluasi Pengguna yang disetujui untuk CASE-008, CASE-009, dan CASE-014 tanpa mengubah field kasus lain. Pemeriksaan publikasi juga mencakup inventaris kasus, ID evidence, severity, struktur bilingual, ruang lingkup, privasi, dan link.

## Validasi Kuantitatif CASE-018

Validasi korektif menemukan Project Instructions lengkap before dan after dalam arsip percakapan mentah. Penghitungan memakai string verbatim: `len(text)` untuk hasil termasuk whitespace, dan jumlah karakter yang memenuhi `not character.isspace()` untuk hasil tanpa whitespace. Hasilnya adalah 6,566 menjadi 5,482 (−1,084; 16.51%) dan 5,558 menjadi 4,601 (−957; 17.22%). Klaim lama sekitar 40% tidak tervalidasi.

## Batas Privasi

Repository memublikasikan identifier evidence, pemetaan, dan ringkasan terbatas. Screenshot asli, kutipan percakapan mentah, kredensial, materi autentikasi, dan informasi pribadi sensitif tetap berada di luar lapisan publik.

## Ketidakpastian yang Tersisa

Beberapa kasus mendukung penyimpangan yang terdokumentasi tanpa membuktikan penyebab internalnya. Penyebab historis false-zero QC masuk akal tetapi belum terkonfirmasi karena skrip atau log asli tidak tersedia. Batasan tersebut dipertahankan dan tidak diperkuat menjadi kepastian.

## Independensi dan Hubungan

Portofolio ini bukan peninjauan, sertifikasi, endorsement, afiliasi, atau sponsorship dari OpenAI. Ini adalah portofolio evaluasi independen berdasarkan lingkungan terdokumentasi dan evidence yang tersedia untuk kasus-kasus ini.
