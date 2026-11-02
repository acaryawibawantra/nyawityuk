# NyawitYuk 🌴

Game mobile-first: hutan → tebang → uang → alat → bibit sawit → panen → demo warga.

## Kontrol
- **Satu analog** (geser di mana saja di layar). Tidak ada tombol aksi.
- **Dekat pohon = otomatis menebang** (3 ayunan dengan kapak).
- Berdiri diam di tanah kosong dengan bibit di tas = **otomatis menanam**.
- Sawit matang di dekatmu = **otomatis dipanen** (Rp70).
- Desktop: WASD / panah.

## Alur ekonomi
| Aksi | Hasil |
|---|---|
| Tebang 1 pohon | Rp9 |
| Panen 1 sawit | Rp70 |
| Bibit sawit | Rp30 (tumbuh 34 detik) |
| Pemotong | Rp120 (1 ayunan per pohon) |
| Api | Rp280 (bakar 3×3, Rp8/pakai) |
| Traktor | Rp700 (bersihkan 3×3, Rp20/pakai) |
| Demo warga | muncul tiap 10 pohon, minta ganti rugi; dibiarkan → tuntutan naik 15% tiap 26 dtk |

## Teknis
- Satu file `index.html`, canvas isometrik 2:1, tanpa dependency, tanpa server.
- Progres disimpan di `localStorage` (`nyawityuk.v2`).
- Diuji di viewport iPhone 390×844 (DPR 3): analog, auto-tebang, auto-tanam, auto-panen, demo, simpan-muat.
