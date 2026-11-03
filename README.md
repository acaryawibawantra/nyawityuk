# NyawitYuk 🌴

Game mobile-first isometrik (gaya iklan game): tebang hutan → uang → alat, bibit, sapi →
tanam sawit → **bertahan dari serangan warga**.

## Kontrol
- **Satu analog**: geser di mana saja di layar. Tidak ada tombol aksi.
- Dekat pohon = otomatis menebang · dekat warga = otomatis memukul
- **Auto-tanam**: punya bibit + berdiri di tanah apa pun (rumput/tanah/ladang) → langsung tertanam
- Sawit matang di dekatmu = otomatis dipanen · Desktop: WASD/panah

## Progresi
| Sistem | Detail |
|---|---|
| XP & Level | tebang +2, panen +6, warga +5, misi +8. Naik level = bonus Rp50 × level |
| Misi berantai | tebang / tanam / panen / hadang warga; selesai otomatis dapat hadiah |
| Combo | tebang/panen beruntun (≤2,6 dtk) → uang ×1,1 per combo, maks ×2 |
| Pabrik CPO | Rp1.500 → hasil panen sawit jadi Rp120 (2×) |

## Ekonomi
1 pohon Rp10 · panen Rp60 (CPO Rp120) · bibit Rp25 (tumbuh 14 dtk) · sapi Rp320 (Rp14/5 dtk, maks 8)
· pemotong Rp120 · api Rp280 · traktor Rp700 · warga tumbang +Rp25 · gelombang bersih +Rp60

## Pertahanan
- Tiap **30 pohon** → gelombang warga (1+wave orang, maks 5)
- Warga: 95 HP, 11 damage/1,1 dtk, kecepatan 1,95 (pemain 4,0 — bisa kabur sambil menanam)
- Pemain: HP 100, pukulan 26 dmg/0,34 dtk, regen 7/dtk setelah 5 dtk aman
- Tumbang: kehilangan 15% uang → tombol bangkit (HP penuh, gelombang reset)

## Teknis
Satu file `index.html`, canvas isometrik 2:1, tanpa dependency/server, simpan otomatis (`nyawityuk.v4`).
