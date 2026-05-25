# Game Ocong

Game Ocong adalah game platform sederhana yang dibuat dengan Phaser 3. Game ini menggunakan dua scene:

1. `sceneMenu` - menu awal
2. `scenePlay` - permainan utama

## Alur Game

1. Pemain membuka game dan masuk ke layar menu.
2. Pada layar menu, suara ambience akan diputar dan pemain melihat tombol `Play`.
3. Pemain menekan tombol `Play` untuk memulai permainan.
4. Game beralih ke scene `scenePlay`.
5. Karakter muncul dan mulai bergerak ke bawah secara otomatis.
6. Pemain mengetuk / mengklik layar untuk membuat karakter melompat ke atas.
7. Latar depan bergerak terus menerus dari kanan ke kiri untuk memberi efek berjalan.
8. Rintangan (`obstc`) muncul secara acak dari sisi kanan dan bergerak ke kiri.
9. Pemain harus menghindari tabrakan dengan rintangan.
10. Setiap kali karakter melewati rintangan, skor bertambah.
11. Jika karakter menyentuh rintangan atau naik terlalu tinggi, permainan berakhir.
12. Game kembali ke layar menu dan skor tertinggi disimpan di `localStorage`.

## Kontrol

- Klik atau ketuk layar untuk membuat karakter melompat.

## File Penting

- `index.html` - memuat konfigurasi game dan daftar scene.
- `sceneMenu.js` - menampilkan menu, membaca skor tertinggi, dan memulai permainan.
- `scenePlay.js` - menjalankan logika permainan, skor, rintangan, dan deteksi tabrakan.

## Catatan

- Pastikan folder `assets` berisi semua gambar dan audio yang dibutuhkan.
- Jika ingin mengubah ukuran game, ubah nilai `width` dan `height` di `index.html`.
