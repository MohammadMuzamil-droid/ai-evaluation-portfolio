# Mengevaluasi ChatGPT Go dalam Penggunaan Nyata

*27 Studi Kasus Berbasis Bukti tentang Kegagalan, Keterbatasan, dan Masalah Kualitas*

**[English](README.md)**

## Tentang Portofolio Ini

Portofolio untuk recruiter ini menunjukkan cara saya mengevaluasi respons AI dengan evidence. Portofolio ini meninjau 27 kasus tervalidasi dari penggunaan ChatGPT Go di dunia nyata yang terdokumentasi. Setiap kasus menghubungkan requirement aktif, respons yang diamati, evaluasi pengguna, analisis teknis, severity, dan referensi evidence yang dapat dilacak.

## Mengapa Ini Penting

Evaluasi AI lebih dari sekadar menemukan jawaban yang buruk. Evaluasi memerlukan pertanyaan pengujian yang jelas, penanganan evidence yang cermat, dan kesimpulan yang tidak melampaui catatan. Portofolio ini menunjukkan proses tersebut pada kepatuhan instruksi, penanganan konteks, asumsi, penalaran, pemformatan, penggunaan alat, dan workflow bertahap.

## Hasil Sekilas

- Kasus: 27
- Referensi evidence tervalidasi: 132
- Severity: 3 Minor, 14 Moderate, 10 Major, 0 Critical
- Kasus Unggulan: 8
- Analisis Mendalam: 4
- CASE-018 termasuk whitespace: 6,566 menjadi 5,482 (−1,084; 16.51%)
- CASE-018 tidak termasuk whitespace: 5,558 menjadi 4,601 (−957; 17.22%)

## Kompetensi yang Ditunjukkan

- Ekstraksi, pemetaan, dan keterlacakan evidence
- Evaluasi kepatuhan instruksi dan penanganan konteks
- Analisis asumsi, konsistensi, dan penalaran
- Validasi kuantitatif dan penilaian severity
- Pemisahan evidence, konteks, evaluasi pengguna, analisis, dan inferensi
- Validasi manusia, corrective QC, validasi ulang independen, dan verifikasi tertarget
- Dokumentasi bilingual yang mempertahankan evidence serta menangani ketidakpastian

## Ringkasan Metode

Kasus direkonstruksi dari catatan percakapan primer. Event duplikat atau terkait hanya dikonsolidasikan ketika logika insiden yang disetujui mendukungnya. ID evidence tetap terhubung dengan setiap kronologi. Evaluasi manusia diberi label sebagai evaluasi manusia, bukan sebagai evidence objektif. Analisis teknis memisahkan observasi dari inferensi. Pemeriksaan korektif dan independen dilakukan sebelum publikasi.

[Baca metodologi lengkap](methodology/id/evaluation-methodology.md)

## Kasus Unggulan

- [CASE-001 — Konsistensi aturan jumlah kata tetap](featured-cases/id/CASE-001.md): memeriksa apakah satu instruksi numerik diterapkan secara konsisten.
- [CASE-007 — Intent workflow terstruktur](featured-cases/id/CASE-007.md): menguji apakah pertanyaan operasional JSON dijawab sebelum redesign diusulkan.
- [CASE-008 — Semantik perintah lintas percakapan](featured-cases/id/CASE-008.md): mengikuti makna ARCHIVE pada tiga rangkaian insiden yang disetujui.
- [CASE-014 — Lineage dan fidelitas dokumentasi](featured-cases/id/CASE-014.md): mengevaluasi alur dari sumber yang disetujui ke artefak yang dibuat.
- [CASE-016 — Ketidakpastian sebelum eksekusi](featured-cases/id/CASE-016.md): menemukan tahap konfirmasi yang hilang sebelum file dibuat.
- [CASE-018 — Validasi prompt kuantitatif](featured-cases/id/CASE-018.md): mengganti asumsi panjang tanpa dukungan dengan pengukuran yang dapat direproduksi.
- [CASE-021 — Preservasi dibandingkan peringkasan](featured-cases/id/CASE-021.md): menguji apakah EXTRACT mempertahankan konten sumber yang diminta.
- [CASE-024 — Atribusi peran evaluator](featured-cases/id/CASE-024.md): memisahkan kesalahan label evaluator dari aktor yang dianotasi.

## Analisis Mendalam

- [CASE-008 — Kontinuitas state dan perintah](deep-dives/id/CASE-008.md)
- [CASE-014 — Rantai evidence dari persetujuan ke ekspor](deep-dives/id/CASE-014.md)
- [CASE-018 — Analisis jumlah karakter yang dapat direproduksi](deep-dives/id/CASE-018.md)
- [CASE-024 — Atribusi kesalahan berbasis peran](deep-dives/id/CASE-024.md)

## Ruang Lingkup dan Keterbatasan

Temuan hanya menjelaskan interaksi ChatGPT Go yang terdokumentasi ini. Temuan bukan estimasi prevalensi dan tidak membandingkan paket atau model. Temuan mungkin tidak berlaku untuk paket, konfigurasi, model, versi, atau fitur ChatGPT lain, produk OpenAI, LLM, atau sistem AI. Penyebab historis hasil false-zero QC masuk akal tetapi belum terkonfirmasi karena skrip atau log asli tidak tersedia.

## Jelajahi

[Pustaka Kasus](case-library/id/README.md) · [Kasus Unggulan](#kasus-unggulan) · [Analisis Mendalam](#analisis-mendalam) · [Metodologi](methodology/id/evaluation-methodology.md) · [Temuan](reports/id/findings.md) · [Pemetaan Evidence](evidence/README-ID.md) · [Laporan QC](portfolio-qc/release-gate-report-ID.md)
