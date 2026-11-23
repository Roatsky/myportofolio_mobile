Nama : Muhammad Naufal Syarifuddin

NPM : 2506602896

Kelas : PBP F

Aplikasi ini merupakan portofolio pribadi saya yang saya kembangkan sebagai proyek untuk tugas PBP Semester Gasal 2026/2027. Aplikasi portofolio ini memiliki halaman dasar yang memiliki tombol untuk emnunjukan proyek, pengalaman, pendidikan, keterampilan, dan logout. 

Dalam tugas 8 ini saya menggunakan AI Gemini. Saya membangun applikasi ini dari template awal serta contoh-contoh coding flutter yang diberikan tim asdos pbp. Untuk penggunaan AI, saya gunakan AI untuk membantu pemahaman penggunaan dan koding dalam flutter dan bug fix tentang implementasi navigasi ke form model.

Pertanyaan Refleksi:
1. Navigator.push() bekerja dengan menambahkan rute halaman ke stack navigator, Navigator.pop() bekerja dengan menghapus rute halaman paling atas di stack navigator. dan Navigator.pushReplacement() bekerja sebagai gabungan pop dan push (pop halaman paling atas lalu push rute halaman baru). Untuk opsi Home di LeftDrawer, itu menggunakan Navigator.pushReplacement() untuk mengarahkan pengguna ke MyHomePage. Karena rute sebelumnya di pushReplacement dan bukan push, halaman utama tidak menumpuk berkali-kali di dalam stack.

2. Scaffold bekerja sebagai kerangka tata letak dasar standar material design di setiap halaman, AppBar bekerja sebagai widget paling atas halaman yang menunjukan judul halaman serta posisi tombol navigasi, dan Drawer bekerja sebagai penyimpan isi sidebar yang biasanya digunakan untuk menyimpan navigasi. Ketiga ini mengandung komponen yang di gunakan disetiap halaman, maka penggunaanya menjamin konsistensi antar halaman. Contoh penggunaan warna tema portofolio ada di halaman LeftDrawer, semua form, dan main dalam bentuk Colors.indigo sebagai BoxDecoration, backgroundColor, dan seedColor.

3. Tata letak formulir terbentuk oleh Form, SingleChildScrollView, Column, dan Padding. SingleChildScrollView dipilih agar halaman scrollable dan membuat halaman tetap menampilkan data bahkan jika ruang layar terbatas. Column dipilih karena form ditulis dengan alur pengisian data dari atas ke bawah. Padding dipilih agar memberikan whitespace di sekitar elemen input agar batas kotak input tidak saling menempel.

4. GlobalKey<FormState> bekerja sebagai pemegang referensi ke widget Form yang bisa digunakan untuk semua kolom input. Validator bekerja sebagai fungsi callback untuk memeriksa nilai input pengguna. Validate() bekerja dengan mengeksekusi seluruh fungsi validator di setiap kolom formulir secara serentak. Contoh nilai yang ditolak yaitu seperti input berupa string kosong pada kolom Nama Proyek atau Deskripsi Pengalaman karena pengecekan value == null || value.trim().isEmpty mengembalikan pesan error "tidak boleh kosong!".