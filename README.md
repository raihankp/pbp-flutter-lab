# counter_7

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
