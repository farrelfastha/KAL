---
title: TRANSFORMASI MATRIKS

---

# **TRANSFORMASI MATRIKS**
## pengertian transformasi matrix
Transformasi matriks adalah proses matematis untuk mengubah posisi, ukuran, bentuk, atau orientasi suatu objek di bidang (2D) atau ruang (3D) melalui operasi matriks.
Dalam geometri dan grafika komputer, transformasi ini digunakan untuk:
- Menggeser (translasi)
- Memutar (rotasi)
- Memperbesar/memperkecil (skalasi)
- Mencerminkan (refleksi)
- Menggeser bentuk (shear)

## Notasi titik dan matriks transformasi
📍 Titik dalam 2D:
$P = [ x  y ]^T$
📍 Sistem Homogen (untuk translasi & gabungan transformasi)
$P = [ x  y  1 ]^T$
Transformasi matriks dalam bentuk 3×3: $T = [ a b c ; d e f ; 0 0 1 ]$

## jrnis jenis transformais matriks
1️⃣ Translasi: Menggeser posisi objek.
Matriks: [1 0 tx; 0 1 ty; 0 0 1]
2️⃣ Rotasi: Memutar objek terhadap titik asal.
Matriks: [cosθ -sinθ; sinθ cosθ]
3️⃣ Skalasi: Mengubah ukuran objek.
Matriks: [sx 0; 0 sy]
4️⃣ Refleksi: Mencerminkan objek terhadap sumbu.
Contoh: Refleksi terhadap sumbu X → [1 0; 0 -1]
5️⃣ Shear: Menggeser bentuk objek.
Shear ke arah X: [1 k; 0 1]

## transformasi gabungan
Transformasi dapat digabungkan dengan mengalikan matriks-matriks transformasi sesuai urutan operasi.
Contoh: Translasi + Rotasi:
Tgabungan = R × T
Urutan perkalian matriks tidak komutatif: A × B ≠ B × A

## penerapan trnasformasi matriks
🎮 Game Development: Menggerakkan karakter, kamera, atau environment.
🎨 Desain Grafis: Memutar, membesarkan, dan mencerminkan objek.
🛰️ Teknik Geodesi: Memetakan posisi titik di permukaan bumi.
🤖 Robotika: Mengontrol lengan robot dan navigasi.
📱 Augmented Reality: Menyesuaikan posisi objek virtual dalam dunia nyata.


## tugas soal
![WhatsApp Image 2025-04-28 at 09.11.13_a967a0a9](https://hackmd.io/_uploads/SJflsTXlel.jpg)

Misalkan v = (x, y) adalah titik di bidang.
Jika dinyatakan dalam koordinat polar:
v = (r cosα, r sinα)
dengan:
r = panjang vektor v
α = sudut antara sumbu-x positif dengan vektor v

Setelah diputar sebesar θ berlawanan arah jarum jam:
v' = (r cos(α+θ), r sin(α+θ))

Gunakan identitas trigonometri:
cos(α+θ) = cosα cosθ - sinα sinθ
sin(α+θ) = sinα cosθ + cosα sinθ

Sehingga:
x' = r cos(α+θ) = r (cosα cosθ - sinα sinθ) = x cosθ - y sinθ
y' = r sin(α+θ) = r (sinα cosθ + cosα sinθ) = x sinθ + y cosθ

Jika ditulis dalam bentuk matriks:
[x']   [ cosθ  -sinθ ] [x]
[y'] = [ sinθ   cosθ ] [y]


