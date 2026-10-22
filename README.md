# Generator Timesheet Gajian

Aplikasi web (satu file, tanpa server) untuk membuat **Form Timesheet Gajian** tiap periode dalam format **Excel** dan **PDF**.

## Cara pakai
1. Buka halaman aplikasi (GitHub Pages). Template bawaan terpasang otomatis.
2. Pilih tanggal mulai periode (tanggal akhir terisi otomatis: mulai + 1 bulan − 1 hari).
3. Isi cuti dan remarks kegiatan bila perlu (opsional).
4. Klik **Unduh Excel** atau **Unduh PDF**.

## Aturan yang diterapkan
- Sabtu/Minggu: baris merah, remarks `Weekend`, jam 00:00.
- Libur nasional (SKB 3 Menteri 2026–2027): baris merah, remarks nama libur, jam 00:00, tidak dihitung kehadiran. Cuti bersama tidak dimerahkan.
- Cuti: baris merah, remarks `Cuti`, jam 00:00.
- Hari kerja lain: remarks `Test log` (atau remarks kegiatan kustom).
- Logo, tanda tangan, kolom, dan baris template dipertahankan.

Libur untuk tahun lain bisa ditambahkan lewat kolom "Libur tambahan" (`YYYY-MM-DD, nama`).

## Berkas
- `index.html` : aplikasi lengkap.
- `template/` : salinan template Excel.

Semua pemrosesan berjalan di browser; file tidak diunggah ke server mana pun.
