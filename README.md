# Portal Berkah Mulia Gabungan

Aplikasi HTML siap deploy untuk GitHub + Vercel.

## Isi aplikasi

- Penawaran & Invoice
- Kas Besar / Laporan Investor
- Single password portal
- Single Google Login
- Penyimpanan masing-masing modul tetap terpisah
- Session tetap aktif saat refresh
- Session hilang saat close tab atau logout

## File utama

Upload semua file ini ke repository GitHub:

```text
index.html
README.md
vercel.json
.gitignore
```

## Cara upload ke GitHub

1. Buat repository baru di GitHub.
2. Upload semua file dari folder ini.
3. Pastikan file utama bernama `index.html`.
4. Commit / Save.

## Cara deploy ke Vercel

1. Buka Vercel.
2. Add New Project.
3. Import repository GitHub ini.
4. Framework Preset: `Other`.
5. Build Command: kosongkan.
6. Output Directory: kosongkan.
7. Install Command: kosongkan.
8. Klik Deploy.

## Login aplikasi

Password default:

```text
mulia123
```

## Google OAuth

Aplikasi memakai Google Client ID yang sudah tertanam di file HTML.

Akun Google yang diizinkan:

```text
lezaikra553@gmail.com
```

Agar Login Google berjalan di domain Vercel baru, tambahkan domain Vercel ke Google Cloud Console:

### Authorized JavaScript origins

Tambahkan URL Vercel baru, contoh:

```text
https://nama-project.vercel.app
```

Jangan pakai garis miring `/` di belakang URL.

## Catatan penting

- Data browser memakai `localStorage`, jadi setiap browser/komputer punya data lokal masing-masing.
- Backup dan restore Google Drive tetap memakai akun Google yang sama.
- Refresh halaman tidak logout.
- Close tab/browser atau klik Keluar akan logout dari session portal.
- Jangan ubah nama file `index.html`.

## Checklist setelah deploy

1. Buka link Vercel.
2. Login password `mulia123`.
3. Tes menu Penawaran & Invoice.
4. Tes menu Kas Besar.
5. Klik Login Google.
6. Pastikan login memakai `lezaikra553@gmail.com`.
7. Coba simpan data kecil.
8. Refresh halaman, pastikan tetap login.
9. Close tab lalu buka lagi, pastikan minta password ulang.
