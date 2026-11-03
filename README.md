# NyawitYuk 🌴

Game mobile-first isometrik (gaya iklan game/Township): tebang hutan → uang → alat, bibit, sapi →
tanam sawit → **bertahan dari serangan warga**.

## Kontrol
- **Satu analog**: geser di mana saja di layar. **Tidak ada tombol aksi.**
- Dekat pohon = otomatis menebang; dekat warga = otomatis memukul.
- Berdiri diam di tanah kosong dengan bibit = otomatis menanam.
- Sawit matang di dekatmu = otomatis dipanen.
- Desktop: WASD / panah.

## Ekonomi
| Item | Angka |
|---|---|
| 1 pohon | Rp10 |
| Panen sawit | Rp60 (tumbuh 14 dtk) |
| Bibit | Rp25 |
| Pemotong / Api / Traktor | Rp120 / Rp280 / Rp700 |
| Sapi perah | Rp320 · Rp14 tiap 5 dtk otomatis · maks 8 |
| Warga tumbang | +Rp25 |
| Gelombang bersih | +Rp60 |

## Pertahanan (menggantikan "bayar demo")
- Tiap **30 pohon** ditebang → **gelombang warga** menyerbu kebun (1 gelombang = 1+wave orang, maks 5).
- Warga mengejar (kecepatan 1,95 vs pemain 4,0), menyangkut di pohon, dan menyerang 11 damage tiap 1,1 dtk.
- Pemain HP **100**, memukul 26 damage tiap 0,34 dtk saat warga dalam jangkauan; HP pulih 7/dtk setelah 5 dtk aman.
- Kalau tumbang: **kehilangan 15% uang**, layar mati, lalu bangkit di kebun (HP penuh, gelombang reset).

## Peta & tampilan
Hutan variatif (3 palet + ukuran acak), padang rumput, ladang gandum, kolam beriak, tanah bekas tebang,
kandang sapi, hutan pinggiran gelap di luar peta, bayangan, partikel, kilatan merah saat kena serang, vignette.

## Teknis
Satu file `index.html`, canvas isometrik 2:1, tanpa dependency/server. Simpan otomatis di `localStorage` (`nyawityuk.v4`).
