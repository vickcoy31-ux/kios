# Kios — Pembukuan & Input HP

## File
- `index.html` — form input harian (grid tombol)
- `dashboard.html` — monitoring bahan + Neraca
- `appsscript.gs` — backend Google Sheets (arsip)
- `data/Pembukuan_Kios.xlsx` — backup Excel (opsional)

## Setup (sekali)
1. Google Sheets: Extensions → Apps Script → tempel `appsscript.gs` → Deploy → Web app → Anyone → salin URL.
2. Ganti `GANTI_DENGAN_URL_APPS_SCRIPT` di `index.html` dan `dashboard.html` dengan URL tersebut.
3. Upload repo ke GitHub → Settings → Pages → Branch main → Save. URL publik muncul.
4. Buka URL GitHub Pages dari HP. Tap-tap. Data masuk Google Sheets.

## Alur harian
- Input: buka `index.html` → tap produk, kategori, nominal, keterangan → SIMPAN.
- Cek: buka `dashboard.html` → Neraca + Bahan.
- Backup: Google Sheets → File → Download → xlsx.

## Bulan baru
- Di Google Sheets, ganti `"2026-10"` di sheet Bahan D5:D10 jadi bulan baru. Atau Ctrl+H.