# CASE-018 — Asumsi panjang prompt membalikkan arah yang diminta

[Beranda portofolio](../../README-ID.md) · [Kasus unggulan](../../README-ID.md#kasus-unggulan) · [Kasus lengkap](../../case-library/id/CASE-018.md) · [English](../en/CASE-018.md)

## Apa yang Terjadi

Sebelum menghasilkan rewrite yang diminta, asisten memperkirakan bahwa restrukturisasi akan membuat Project Instructions lebih panjang. Pasangan before dan after yang lengkap kemudian menunjukkan bahwa hasil rewrite lebih pendek.

## Mengapa Ini Penting

Asumsi kelayakan tanpa dukungan dapat mengalihkan tugas meskipun hasil yang diminta dapat diukur dan dicapai.

## Alasan Kasus Ini Dipilih

Kasus ini menggabungkan kronologi, rekonstruksi sumber mentah, dan pengukuran yang dapat direproduksi. Hasilnya adalah 6,566 menjadi 5,482 karakter termasuk whitespace (−1,084) dan 5,558 menjadi 4,601 tanpa whitespace (−957).

## Keterampilan Evaluator yang Ditunjukkan

Validasi kuantitatif, pengujian asumsi, rekonstruksi evidence, dan koreksi ketidakpastian.

## Nilai yang Membedakan

Pengurangan terukur adalah 16.51% dan 17.22%. Angka tersebut mendukung temuan bahwa hasil lebih pendek dan secara eksplisit tidak mendukung klaim lama sekitar 40%.

[Baca kasus lengkap berbasis evidence](../../case-library/id/CASE-018.md) · [Buka Analisis Mendalam](../../deep-dives/id/CASE-018.md)
