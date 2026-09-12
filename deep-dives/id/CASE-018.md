# Analisis Mendalam — CASE-018: Analisis jumlah karakter yang dapat direproduksi

[Beranda portofolio](../../README-ID.md) · [Analisis mendalam](../../README-ID.md#analisis-mendalam) · [Kasus lengkap](../../case-library/id/CASE-018.md) · [English](../en/CASE-018.md)

## Pertanyaan Evaluasi

Apakah prediksi bahwa restrukturisasi akan membuat Project Instructions lebih panjang didukung oleh rewrite yang selesai?

## Rantai Evidence dan Kronologi

`EVENT-0432` mempertahankan permintaan yang mengatur, pernyataan kelayakan, koreksi pengguna, dan tindak lanjut asisten sebagai `CASE-018-E01` sampai `CASE-018-E04`. Validasi korektif kemudian menemukan Project Instructions lengkap sebelum dan sesudah proses revisi yang sama dalam `conversations-000.json`.

## Metode Penghitungan yang Dapat Direproduksi

Kedua isi prompt diekstrak secara verbatim. Tidak ada teks yang dinormalisasi, diperbaiki, atau diringkas sebelum penghitungan. Nilai termasuk whitespace menggunakan `len(text)`. Nilai tanpa whitespace menghitung setiap karakter yang memenuhi `not character.isspace()`.

| Pengukuran | Sebelum | Sesudah | Selisih | Pengurangan |
|---|---:|---:|---:|---:|
| Karakter termasuk whitespace | 6,566 | 5,482 | −1,084 | 16.51% |
| Karakter tanpa whitespace | 5,558 | 4,601 | −957 | 17.22% |

## Penalaran Evaluator

Tugas dapat diukur setelah draf lengkap tersedia. Pasangan aktual bergerak ke arah yang diminta, sehingga prediksi sebelumnya seharusnya tidak menggantikan rewrite atau mengalihkan tugas.

## Observasi dan Inferensi

**Observasi:** rewrite yang selesai lebih pendek menurut kedua metode. **Inferensi terbatas:** asumsi kelayakan terbalik dalam insiden ini. Hasil tersebut tidak membuktikan bahwa setiap tugas restrukturisasi akan menjadi lebih pendek atau menjelaskan alasan prediksi dibuat.

## Interpretasi Alternatif

Restrukturisasi kadang dapat menambah teks. Kemungkinan umum tersebut tidak mengalahkan hasil terukur untuk pasangan ini.

## Ketidakpastian dan Dampak

Klaim lama sekitar 40% tidak tervalidasi dan tidak boleh dipulihkan. Hasil yang didukung adalah pengurangan 16.51% termasuk whitespace dan 17.22% tanpa whitespace. Dampaknya adalah pengalihan yang dapat dihindari dari permintaan yang sebenarnya dapat dipenuhi.

## Pelajaran untuk Praktik Evaluasi

Untuk tugas yang peka terhadap panjang, bandingkan artefak before dan after yang lengkap dengan aturan penghitungan yang dinyatakan. Pisahkan estimasi dari hasil terukur.

[Buka catatan lengkap berbasis evidence](../../case-library/id/CASE-018.md)
