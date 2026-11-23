# Naruto Senki 3D – Ultimate Ninja Battle (Browser Edition)

Game pertarungan ninja 3D berbasis browser (Three.js). Dapat dimainkan langsung di browser modern.

## Cara Menjalankan

### Opsi 1: Langsung buka file
Buka `index.html` di browser (Chrome/Edge/Firefox). Beberapa browser membatasi module lokal; jika blank, gunakan Opsi 2.

### Opsi 2: Server lokal
```bash
cd NarutoSenki3D
python -m http.server 8080
```
Lalu buka http://localhost:8080

Atau dengan Node:
```bash
npx serve .
```

## Kontrol PC
- WASD: Gerakan
- Mouse: Kamera (klik canvas untuk pointer lock)
- Klik kiri: Attack
- Klik kanan: Block
- Space: Jump
- Shift: Dash
- Q/E/R: Skill 1/2/3
- F: Ultimate
- G/H/J: Special Skills (@headroom / @caveman / @ponytail)
- Esc: Pause

## Kontrol Android
- Joystick virtual kiri
- Tombol kanan: ATK, JMP, DSH, BLK, S1, S2, S3, ULT, SPC

## Fitur
- 14 karakter (Naruto, Sasuke, Kakashi, Sakura, Itachi, Madara, Minato, Obito, Pain, Gaara, Rock Lee, Might Guy, Hashirama, Tobirama)
- 7 arena 3D
- Sistem pertarungan: basic/combo/heavy/dash/dodge/block/counter/air combo/skill combo/ultimate/target lock/HP & Chakra bar
- AI musuh
- Mode: Quick Battle, Story, Survival, Boss Battle, Tournament, Training (Custom/Online placeholder)
- Special Skills config: @headroom, @caveman, @ponytail (editable di Settings)
- Settings: quality, resolution scale, FPS cap, sound

## Catatan
Aset 3D dibuat prosedural (original) agar bebas lisensi. Untuk kualitas AAA (UE5/Unity) gunakan source ini sebagai prototipe gameplay/logic.

## Struktur
- index.html : game utuh (HTML+CSS+JS)
- README.md : petunjuk
- skills.config.json : (opsional) konfigurasi skill khusus
