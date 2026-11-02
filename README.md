# NyawitYuk 🌴

Game mobile-first bergaya iklan game (Township-ish): hutan → tebang → uang → alat & bibit → panen sawit → ternak sapi → demo warga.

## Kontrol
- **Satu analog**: geser di mana saja di layar, thumbstick muncul di situ. **Tidak ada tombol aksi.**
- **Dekat pohon = otomatis menebang** (1 ayunan dengan kapak).
- Berdiri diam di tanah kosong dengan bibit = **otomatis menanam**.
- Sawit matang di dekatmu = **otomatis dipanen**.
- Desktop: WASD / panah.

## Tempo (versi cepat)
- Tebang ~**3 pohon/detik** (kapak 0,18 dtk/ayunan, pohon 2 hp)
- Tanam **0,16 dtk** setelah berhenti di tanah
- Sawit siap panen **14 dtk**
- Jalan 4,0 petak/detik

## Ekonomi
| Item | Angka |
|---|---|
| 1 pohon | Rp10 |
| Panen sawit | Rp60 |
| Bibit sawit | Rp25 |
| Pemotong | Rp120 (ayunan 0,11 dtk) |
| Api | Rp280 (bakar 3×3, Rp8/pakai) |
| Traktor | Rp700 (3×3 instan, Rp20/pakai) |
| Sapi perah | Rp320 · Rp14 tiap 5 dtk otomatis · maks 8 ekor |
| Demo warga | tiap **30 pohon**; minta ganti rugi, naik 15% tiap 45 dtk kalau dibiarkan |

## Peta
Hutan, padang rumput, ladang gandum (dekor), tanah bekas tebang (bisa ditanam), kolam, kandang sapi.

## Teknis
- Satu file `index.html`, canvas isometrik 2:1, tanpa dependency dan tanpa server.
- Progres tersimpan di `localStorage` (`nyawityuk.v2`).
- Diuji di viewport iPhone 390×844 DPR 3: analog, auto-tebang (3 pohon/dtk), auto-tanam, auto-panen, ternak sapi, demo, tanpa error JS.
