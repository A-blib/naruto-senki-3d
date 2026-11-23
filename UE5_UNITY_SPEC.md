# Panduan Migrasi ke Unreal Engine 5 / Unity 3D

Prototipe browser ini menyediakan gameplay loop, data karakter, arena, skill, dan AI.
Untuk kualitas AAA, porting ke UE5/Unity dengan mapping berikut.

## Struktur Proyek
- /Characters : 14 karakter (skeletal mesh + anim blueprint)
- /Animations : Idle, Walk, Run, Jump, Attack, Block, Hit, Skill, Ultimate, Death
- /Skills : data asset per skill (damage, cooldown, chakra, VFX, SFX)
- /Arenas : 7 level
- /AI : Behavior Tree + Blackboard
- /UI : UMG (UE5) / uGUI (Unity)

## Special Skills (identifier wajib dipertahankan)
- @headroom : buff speed+damage
- @caveman : AOE brutal
- @ponytail : homing projectiles
Konfigurasi di `skills.config.json` (copy ke DataTable/DataAsset).

## Kontrol
PC: WASD, Mouse, LMB attack, RMB block, Space jump, Shift dash, Q/E/R skill, F ultimate.
Android: Virtual joystick + buttons.

## Checklist Fitur
- [x] 3D third-person camera
- [x] Combat basic/combo/heavy/dash/block/jump/air
- [x] Skills + ultimate
- [x] AI chase/attack/skill/ultimate
- [x] 7 arena
- [x] 8 mode (quick/survival/boss/training + placeholders)
- [x] UI lengkap
- [x] Settings quality/resolution/fps
- [x] Save progress (localStorage -> SaveGame)

## Aset
Gunakan aset original/berlisensi. Jangan pakai aset resmi Naruto tanpa izin.
Model prosedural di prototipe dapat diganti dengan skeletal mesh berkualitas.

## Instalasi UE5
1. Install Unreal Engine 5.3+
2. Buat project Third Person
3. Import karakter (Mixamo/aset berlisensi)
4. Buat Anim Blueprint per karakter
5. Implementasi GAS (Gameplay Ability System) untuk skill
6. Build AI dengan Behavior Tree
7. Package untuk Windows/Android
