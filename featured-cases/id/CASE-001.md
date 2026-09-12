# CASE-001 — Penerapan instruksi 25 kata yang tidak konsisten

[Beranda portofolio](../../README-ID.md) · [Kasus unggulan](../../README-ID.md#kasus-unggulan) · [Kasus lengkap](../../case-library/id/CASE-001.md) · [English](../en/CASE-001.md)

## Apa yang Terjadi

Pengguna memberikan frasa “dalam 25 kata”. Asisten memperlakukan tugas sebagai batas maksimum 25 kata. Setelah pengguna menantang pembacaan tersebut, tindak lanjut menerima interpretasi tepat 25 kata.

## Mengapa Ini Penting

Hasil penilaian tidak dapat diandalkan jika aturan numerik yang sama diterapkan dengan dua cara berbeda. Jumlah kata harus diperiksa sebelum perbandingan kualitas dilakukan.

## Alasan Kasus Ini Dipilih

Rangkaian empat pesan membuat requirement, penyimpangan, koreksi, dan pengakuan mudah dilacak.

## Keterampilan Evaluator yang Ditunjukkan

Evaluasi kepatuhan instruksi dan analisis konsistensi untuk batasan numerik tetap.

## Nilai yang Membedakan

Kasus ini menunjukkan bagaimana satu perbedaan kecil—“tepat” dibandingkan “maksimum”—dapat mengubah seluruh hasil evaluasi tanpa memerlukan klaim tentang status model internal.

[Baca kasus lengkap berbasis evidence](../../case-library/id/CASE-001.md)
