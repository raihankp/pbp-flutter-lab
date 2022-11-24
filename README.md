# counter_7

## Tugas 7

### Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget dan jelaskan perbedaan dari keduanya.
- Stateless widget adlaah widget yang dimuat secara statis. Seluruh konfigurasi yang dimuat didalamnya telah diinisiasikan sejak awal widget tersebut dibuat. Stateless widget adalah sebuah widget yang tidak dapat diubah dan tidak akan pernah berubah.
- Stateful widget merupakan suatu widget yang sifatnya dinamis atau dapat berubah-ubah, kebalikan dari stateless widget. Stateful widget dapat mengubah tampilan, menambah widget, mengubah nilai variabel, icon, warna, dan lain-lain.

### Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Text: Menampilkan Teks
2. Column: Menampung widget dan disusun secara vertikal
3. Row: Menampung widget dan disusun secara horizontal
4. FloatingActionButton: Widget button yang berada di depan widget lainnya
5. Icon: Menampilkan suatu ikon
6. Center: Layout widget yang berfungsi untuk menengahkan childnya

### Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
setState() berfungsi untuk mengubah suatu state yang ada di stateful widget. Variabel yang terdampak di fungsi tersebut adalah _counter.

### Jelaskan perbedaan antara const dengan final.
Final harus diinisiasikan terlebih dahulu, tidak bisa diubah valuenya, dan harus sudah diketahui valuenya pada saat run time. Sedangkan, const bisa diubah valuenya dan valuenya diketahui pada saat compile time.

### Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Membuat projek dengan `flutter create counter_7`
2. Membuat fungsi untuk mendecrement counter
3. Menambahkan widget FloatingActionButton kedua untuk mendecrement dan akan hilang apabila counternya = 0
4. Membuat Text berwarna merah ketika counter % 2 = 0, dan biru ketika tidak terpenuhi. 

## Tugas 8

### Jelaskan perbedaan Navigator.push dan Navigator.pushReplacement.
- Navigator.push adalah method yang berfungsi untuk push sebuah route ke stack Navigator
- Navigator.pushReplacement adalah method yang berfungsi untuk mengganti route yg sedang ditamplikan mnjadi route baru, lalu mempush route baru ke Stack Navigator

### Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Navigator: Mengelola widget child dengan menggunakan struktur stack.
2. TextFormField: Menerima input user
3. DropdownButtonFormField: Dropdown untuk memilih input yang diinginkan
4. Card: Menampilkan data yang telah diinput dalam bentuk cards
5. Expanded: Memperluas child dari Row, Column, atau Flex untuk mengisi ruang yang tersedia.
6. Container: Penampung berbagai widget untuk menerapkan posisi, ukuran, dan property lainnya secara seragam
7. EdgeInsets: Memberikan Offset ke 4 arah kardinal yang bersifat immutable
8. Visibility: Menampilkan/menyembunyikan suatu child

### Sebutkan jenis-jenis event yang ada pada Flutter (contoh: onPressed).
onPressed()
onChanged()
onTap()
onSaved()

### Jelaskan bagaimana cara kerja Navigator dalam "mengganti" halaman dari aplikasi Flutter.
Navigator bekerja dengan menggunakan struktur stack, dimana route yang berada di paling atas stack adalah route yang ditampilkan saat ini. Cara mengganti halamannya adalah dengan menggunakan pop dan push ke stack tersebut.

### Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Membuat widget drawer untuk menavigasi ke route lain
2. Membuat halaman form yang berisi title budget dan nominal budget dengan tipe data TextField serta type budget dengan DrowdownButtonFormField berisi pengeluaran dan pemasukan
3. Membuat FloatingActionButton untuk menyimpan input yang sudah diisi dan melakukan validasi kepada input
4. Menambahkan data yang telah diinput ke dalam list kosong global
5. Membuat halaman list budget dalam bentuk cards
6. Import semua file .dart ke masing-masing file
7. Membuat tampilan setiap elemen pada list dengan menggunakan ListView.builder()
8. Membuat card yang menampilkan title, nominal, dan type budget


## Tugas 9

### Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data JSON?
Bisa, tetapi kita tidak bisa memastikan apakah data JSON yang diambil sudah memiliki bentuk seperti yang kita inginkan. Sehingga akan lebih baik apabila kita membuat model terlebih dahulu.

### Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
1. Stack: Memposisikan children relatif terhadap tepi-tepi kotak.
2. Text: Menampilkan Teks
3. Column: Menampung widget dan disusun secara vertikal
4. TextSpan: Menampilkan teks immutable secara merentang
5. SizedBox: Menampilkan sebuah box dengan ukuran tertentu
6. Container: Penampung berbagai widget untuk menerapkan posisi, ukuran, dan property lainnya secara seragam
7. FutureBuilder: Widget yang membangun tampilan dirinya sendiri. Berguna untuk menampilkan berbagai widget yang sama dengan data yang berbeda.
8. MainAxisAlignment: Menempatkan children sepanjang sumbu utama dalam sebuah layout flex
9. EdgeInsets: Memberikan Offset ke 4 arah kardinal yang bersifat immutable

### Jelaskan mekanisme pengambilan data dari json hingga dapat ditampilkan pada Flutter.
Menambahkan depedensi http, kemudian melakukan GET pada data json yang selanjutnya dikonversikan ke dalam suatu model yang dibuat. Data json kemudian ditampilkan dengan menggunakan FutureBuilder.

### Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas.
1. Menambahkan dependensi HTTP pada proyek flutter sehingga dapat mengambil data dari internet
2. Membuat model serialisasi data JSON dari MyWatchlist
3. Fetch data MyWatchlist secara asynchronous dari website Heroku Tugas 3, lalu serialisasi data tersebut
4. Membuat halaman yang menampilkan list dari objek-objek MyWatchlist menggunakan data yang telah diserialisasi
5. Mem-wrap setiap objek sebagai tombol dengan routing ke halaman detail watchlist
6. Membuat halaman detail watchlist yang menampilkan atribut-atribut dari suatu objek MyWatchlist
