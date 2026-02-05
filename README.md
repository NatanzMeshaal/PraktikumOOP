# 📘 Praktikum OOP Python

Repository ini berisi latihan dan analisis Object Oriented Programming menggunakan Python. Materi mencakup Class, Object, Inheritance, Encapsulation, Abstraction, dan Polymorphism.

## 🦸 Latihan 1. Membuat Class Hero

Soal
• Apa yang terjadi jika hero1.hp diubah menjadi 500 setelah objek dibuat.
• Jalankan print(hero1.hp).

Jawaban
• Nilai hp berubah menjadi 500.
• Hal ini terjadi karena hp bersifat public.
• Atribut public bisa diubah dari luar class.
• Data penting menjadi tidak aman jika tidak dienkapsulasi.

## 🤝 Latihan 2. Interaksi Antar Objek

Soal
• Method serang memiliki parameter lawan berupa objek.
• Mengapa bukan string nama?

Jawaban
• Objek menyimpan data dan perilaku.
• Hero bisa langsung mengurangi hp lawan.
• Method lain pada lawan bisa dipanggil.
• String hanya teks dan tidak punya perilaku.

## 🧬 Latihan 3. Pewarisan Inheritance

Soal
• Hapus baris super().init(name, hp, attack_power) pada class Mage.
• Jalankan eudora.info().
• Amati error yang muncul.

Jawaban
• Muncul error Mage object has no attribute 'name'.
• Atribut name tidak dibuat.
• Constructor parent tidak dijalankan.
• Fungsi super() menghubungkan data parent ke child.
• Tanpa super(), pewarisan atribut gagal.

## 🔐 Latihan 4. Enkapsulasi

Soal 4.1
• Tambahkan kode print(hero1._Hero__hp).
• Amati hasilnya.

Jawaban
• Nilai HP tetap muncul.
• Python memakai Name Mangling.
• Atribut diubah namanya secara internal.
• Akses ini tidak dianjurkan.
• Melanggar prinsip keamanan data.

Soal 4.2
• Hapus validasi pada set_hp.
• Jalankan hero1.set_hp(-100).

Jawaban
• HP berubah menjadi -100.
• Data menjadi tidak logis.
• Setter menjaga integritas data.
• Validasi mencegah bug dalam game.

## 🧾 Latihan 5. Abstraction dan Interface

Soal 5.1
• Hapus method serang dari class Hero.
• Jalankan program.

Jawaban
• Muncul error Can't instantiate abstract class Hero.
• Hero melanggar kontrak abstrak.
• Method abstrak wajib diimplementasikan.
• Python mencegah objek tidak lengkap.

Soal 5.2
• Aktifkan kode unit = GameUnit().

Jawaban
• GameUnit tidak bisa diinstansiasi.
• Class abstract adalah cetakan.
• Digunakan sebagai standar.
• Memastikan semua turunan konsisten.

## 🔄 Latihan 6. Polymorphism

Soal 6.1
• Buat class Healer(Hero).
• Isi method serang untuk menyembuhkan.
• Tambahkan ke list pasukan tanpa ubah loop.

Jawaban
• Program tetap berjalan normal.
• Loop tidak peduli jenis objek.
• Asal method serang tersedia.
• Polymorphism memudahkan penambahan fitur.

Soal 6.2
• Ubah nama method serang pada Archer menjadi tembak_panah.

Jawaban
• Program error saat dijalankan.
• Loop memanggil method serang.
• Method tidak ditemukan.
• Nama method harus konsisten.

📚 Penutup

Latihan ini menunjukkan manfaat OOP.
Kode lebih rapi.
Data lebih aman.
Program mudah dikembangkan.
Cocok untuk game dan aplikasi skala besar.
