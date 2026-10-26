# Generator Timesheet Gajian

Aplikasi web (satu file, tanpa server) untuk membuat **Form Timesheet Gajian** tiap periode dalam format **Excel** dan **PDF**.

## Cara pakai
1. Buka halaman aplikasi (GitHub Pages). Template "Timesheet Bulanan" terpasang otomatis (template lain bisa diupload).
2. Pilih tanggal mulai periode (tanggal akhir terisi otomatis: mulai + 1 bulan − 1 hari).
3. Isi cuti dan remarks kegiatan bila perlu (opsional).
4. Klik **Unduh Excel** atau **Unduh PDF**.

## Opsi tambahan
- **Identitas & tanda tangan (opsional):** ganti *Name Of Project*, *Location*, *Nama*, dan upload gambar tanda tangan (Employee). Kosong = pakai isi template. Ukuran tanda tangan otomatis disesuaikan dengan kotak di template.
- **Cuti dan remarks kegiatan:** tanggalnya hanya bisa dipilih di dalam periode.
- **Template** "Timesheet Bulanan" terpasang otomatis; template lain bisa di-upload. Tanda tangan milik template yang diupload dipertahankan di Excel dan PDF.
- **Tanda tangan:** kosong = tanpa tanda tangan; bisa upload gambar atau digambar langsung dengan jari/mouse (tanpa pemilih file).
- **Di HP:** setelah unduh muncul pesan konfirmasi dan tombol "Simpan" jika unduhan otomatis diblokir browser.

## Aturan yang diterapkan
- Sabtu/Minggu: baris merah, remarks `Weekend`, jam 00:00.
- Libur nasional (SKB 3 Menteri 2026–2027): baris merah, remarks nama libur, jam 00:00, tidak dihitung kehadiran. Cuti bersama tidak dimerahkan.
- Cuti: baris merah, remarks `Cuti`, jam 00:00.
- Hari kerja lain: remarks `Testing Backlog` (tidak bold), atau remarks kegiatan kustom (teks panjang otomatis wrap, maksimal 200 karakter).
- Jumlah baris tanggal mengikuti panjang periode (28–31 hari); bagian bawah tabel menyesuaikan.
- Logo, tanda tangan, dan kolom template dipertahankan.

Libur untuk tahun lain bisa ditambahkan lewat kolom "Libur tambahan" (`YYYY-MM-DD, nama`).

## Berkas
- `index.html` : aplikasi lengkap.
- `template/` : salinan template Excel.
- `CHANGELOG.md` : riwayat versi dan cara rollback.

Semua pemrosesan berjalan di browser; file tidak diunggah ke server mana pun.
