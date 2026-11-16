Nama : Muhammad Naufal Syarifuddin

NPM : 2506602896

Kelas : PBP F

Aplikasi ini merupakan portofolio pribadi saya yang saya kembangkan sebagai proyek untuk tugas PBP Semester Gasal 2026/2027. Aplikasi portofolio ini memiliki halaman dasar yang memiliki tombol untuk emnunjukan proyek, pengalaman, pendidikan, keterampilan, dan logout. 

Dalam tugas 7 ini saya menggunakan AI Gemin. Saya membangun applikasi ini dari template awal yang tim asdos PBP berikan dan saya gunakan AI untuk membantu pemahaman penggunaan dan koding dalam flutter serta bug fix.

Pertanyaan Refleksi:
1. Widget tree adalah strukur hierarchy berbentuk pohon yang bekerja sebagai seluruh UI aplikasi flutter. Setiap elemen visual, seperti teks, tombol, gambar, hingga pengaturan jarak, disusun sebagai simpul (node) di dalam pohon ini. Dalam pohon ini, ada relasi antar parent dan child dimana child dibungkus oleh parent dan mendapatkan informasi seperti ukuran dan posisi.

2. Semua widget dan fungsi:
    a. MyApp: Widget root utama yang mengatur tema dan halaman awal
    b. MaterialApp: Membungkus seluruh aplikasi dengan konfigurasi Google Material Design
    c. MyHomePage: Widget halaman utama
    d. Scaffold: Kerangka tata letak dasar untuk snackbar, appbar, dan body
    e. Appbar: Menampilkan bar navigasi bagian atas halaman aplikasi
    f. SingleChildScrollView Membuat konten di dalamnya dapat discroll
    g. Padding: Memberi padding sekeliling widget 
    h. Column: Menyusun daftar widget anak secara vertikal 
    i. Row: Menyusun daftar widget anak secara horizontal
    j. InfoCard: Menampilkan kartu informasi identitas
    k. Card: Kontainer bergaya kartu
    l. Container: Mengatur dimensi ukuran width, padding, dan tata letak anak (card) di dalamnya
    m. GridView.count: Menampilkan kumpulan widget dengan jumlah kolom tetap
    n. ItemCard: Menampilkan setiap tombol aksi pada menu portofolio
    o. Material: Menyediakan permukaan kanvas Material Design
    p. InkWell: Mendeteksi interaksi sentuhan pengguna
    q. SnackBar: Menampilkan pesan notifikasi paska tekan tombol
    r. Icon: Menampilkan ikon
    s. SizedBox: Kotak kosong dengan tinggi tertentu untuk memberikan jarak vertikal antar-widget.   
    t. Center: Memposisikan widget anaknya tepat di tengah ruang yang tersedia secara horizontal maupun vertikal.   
    u. Text: Menampilkan teks serta menentukan fontWeight, fontSize, color, dan textAlign.   

3. MaterialApp adalah widget pembungkus tingkat atas yang membungkus aplikasi agar mengikuti sistem desain Google Material Design. MaterialApp bekerja sebagai root widget karena sebagai root widget, MaterialApp bekerja sebagai pondasi dimana merupakan parent semua widget seterusnya dan akan berikan informasi berkenai navigasi, tema, dan pengaturan yang sesuai dengan sistem desain Google Material Design.

4. Stateless widget merupakan widget yang bersifat immutable (nilai atau properti di dalamnya bersifat tetap sejak pertama kali dibuat) sedangkan stateful widget merupakan widget yang memiliki state (data yang dapat berubah-ubah selama siklus hidup widget). Stateless widget digunakan untuk UI yang menampilkan informasi statis (seperti infocard di proyek ini), sedangkan stateful widget digunakan untuk UI yang penampilannya dinamis seperti ada animasi, pembaruan data, user interaction, dll.

5. BuildContext adalah objek peganggan (handle) yang merepresentasikan lokasi spesifik sebuah widget di dalam widget tree. BuildContext sangat penting sebagai cara efisien dalam mencari informasi dari ancestor. BuildContex digunakan dalam build untuk mengambil parameter mengenaik navigasi, tema, ukuran, warna, dll yang dibutuhkan untuk membangun UI aplikasi

6. Hot reload mengulang penampilan agar kode baru tertunjuk namun menyimpan status aplikasi, sedangkan hot restart memuat kode baru dengan menghilangkan kondisi app dan inisialisasi ulang  main. Karena hot reload hanya bekerja jika mengubah tampilan flutter tanpa mengubah inti kodenya, maka hot reload hanya bisa untuk perubahan UI sedangkan hot restart untuk inisialisasi ulang widget atau mengubah variabel global dan full restart untuk perubahan kode native atau menambahkan dependensi baru