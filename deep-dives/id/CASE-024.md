# Analisis Mendalam — CASE-024: Atribusi kesalahan berbasis peran

[Beranda portofolio](../../README-ID.md) · [Analisis mendalam](../../README-ID.md#analisis-mendalam) · [Kasus lengkap](../../case-library/id/CASE-024.md) · [English](../en/CASE-024.md)

## Pertanyaan Evaluasi

Apakah kesalahan klasifikasi diatribusikan kepada orang yang memilih label, atau kepada aktor yang perilakunya sedang dianotasi?

## Rantai Evidence dan Kronologi

`EVENT-0782` mempertahankan konteks yang mengatur, respons bermasalah, koreksi pengguna, dan tindak lanjut asisten sebagai `CASE-024-E01` sampai `CASE-024-E04`. Koreksi mempertahankan evaluator dan aktor yang dianotasi sebagai peran terpisah.

## Penalaran Evaluator

Evaluasi dimulai dengan satu pertanyaan tanggung jawab: siapa yang memilih kategori? Aktor menghasilkan atau menunjukkan perilaku. Evaluator menerapkan label. Kesalahan pemilihan kategori berada pada peran kedua, meskipun perilaku aktor juga dapat dievaluasi.

## Observasi dan Inferensi

**Observasi:** penjelasan mengatribusikan kesalahan kategori kepada aktor yang dianotasi. **Inferensi terbatas:** tanggung jawab salah diatribusikan dalam contoh pelatihan ini. Catatan tidak menetapkan intent atau kompetensi secara luas.

## Interpretasi Alternatif

Aktor yang dianotasi mungkin juga menunjukkan masalah terpisah. Kemungkinan itu tidak memindahkan tanggung jawab atas pilihan label evaluator.

## Ketidakpastian dan Dampak

Evidence tidak mendukung klaim lebih luas tentang salah satu peserta. Dampak yang didukung adalah feedback yang salah sasaran dan pelajaran pelatihan yang mengarahkan tindakan korektif kepada peran yang salah.

## Pelajaran untuk Praktik Evaluasi

Evaluasi berbasis peran harus memisahkan perilaku, anotasi, dan keputusan klasifikasi. Counterfactual yang berguna mempertahankan perilaku tetapi hanya mengubah label evaluator.

[Buka catatan lengkap berbasis evidence](../../case-library/id/CASE-024.md)
