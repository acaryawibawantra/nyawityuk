# NyawitYuk 🌴

Game mobile-first isometrik (gaya iklan game): tebang hutan → uang → alat, bibit, sapi →
tanam sawit → **bertahan dari serangan warga dan bencana alam**.

## Kontrol
- **Satu analog**: geser di mana saja di layar. Tidak ada tombol aksi.
- Dekat pohon = otomatis menebang · dekat warga = otomatis memukul/menembak
- **Auto-tanam**: punya bibit + berdiri di tanah apa pun (rumput/tanah/ladang) → langsung tertanam
- Sawit matang di dekatmu = otomatis dipanen · Desktop: WASD/panah

## Dunia (peta 34×34)
Hutan besar, padang rumput, ladang gandum, dua kolam, kandang sapi, hutan gelap di luar peta.

## Cuaca & hutan tumbuh
- Siklus **cerah ⇄ hujan** otomatis (hujan 16–26 dtk, cerah 30–50 dtk)
- Saat **hujan**, hutan **tumbuh kembali** (±2 pohon/dtk di sekitar pemain) dan sawit tumbuh 1,6–1,8× lebih cepat
- Setiap hujan datang, peluang **bencana alam**: **badai** (sawit tumbang), **hama** (sapi berhenti produksi 14 dtk), atau angin kencang
- Chip cuaca di HUD berubah jadi biru "Hujan"

## Senjata
| Alat | Fungsi |
|---|---|
| Kapak | tebang 1 ayunan/pohon |
| Pemotong | ayunan super cepat |
| Api | bakar 3×3 + **melukai warga** di radius 2 petak |
| Traktor | bersihkan 3×3 instan |
| **Senapan** (Rp900) | tembak warga otomatis 45 dmg, jangkauan 4 petak, jeda 0,75 dtk, butuh **peluru** (Rp45 / 12 butir) · tetap bisa menebang |

## Progresi
XP & level (bonus Rp50 × level) · misi berantai (tebang/tanam/panen/hadang warga) · combo uang sampai ×2 ·
pabrik CPO Rp1.500 (hasil panen 2×) · sapi Rp320 (Rp14/5 dtk, maks 8)

## Pertahanan
Gelombang warga tiap 30 pohon (1+wave orang, maks 5) · warga 95 HP, 11 dmg/1,1 dtk · pemain HP 100,
pukulan 26 dmg · tumbang = kehilangan 15% uang lalu bangkit di kebun.

## Teknis
Satu file `index.html`, canvas isometrik 2:1, tanpa dependency/server, simpan otomatis (`nyawityuk.v5`).
