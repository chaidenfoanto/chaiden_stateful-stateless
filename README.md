# Session 4 : Lab Activity 1 - Stateful and Stateless widget
---
### Nama: Chaiden Richardo Foanto  
### NIM: 0806022310023  
### Mata Kuliah: Visual Programming - Flutter  

---

## Observasi Perilaku Counter pada StatelessWidget dan StatefulWidget

### StatelessWidget:
Pada versi StatelessWidget, ketika kamu menekan tombol "Increment", nilai counter tidak akan berubah. Hal ini terjadi karena StatelessWidget bersifat statis, yang berarti widget ini tidak menyimpan atau mengubah state setelah pertama kali dibuat. Meskipun tombol ditekan, widget ini tidak dapat memperbarui tampilan berdasarkan input pengguna, karena tidak ada mekanisme untuk memperbarui state.

**Kapan menggunakan StatelessWidget?**
- Cocok digunakan ketika tampilan atau UI tidak memerlukan perubahan setelah pertama kali ditampilkan.
- Misalnya untuk widget yang menampilkan data statis atau elemen UI yang tidak berubah.


### StatefulWidget:
Pada versi StatefulWidget, saat tombol "Increment" ditekan, nilai counter akan bertambah sesuai dengan fungsi incrementCounter yang dijalankan. Di dalam StatefulWidget, widget menyimpan state yang dapat diperbarui secara dinamis menggunakan metode setState. Metode setState memicu pembaruan tampilan UI, sehingga ketika state berubah (misalnya, nilai counter bertambah), UI akan merender ulang dengan nilai terbaru.

**Kapan menggunakan StatefulWidget?**
- Cocok digunakan ketika tampilan atau UI perlu berubah seiring waktu berdasarkan interaksi pengguna.
- Misalnya untuk aplikasi yang memiliki input pengguna, animasi, atau data dinamis yang perlu diperbarui setelah beberapa waktu.

---

### Perbandingan
- **StatelessWidget** lebih efisien ketika data atau tampilan tidak berubah, karena tidak perlu menyimpan atau mengelola *state*.
- **StatefulWidget** memberikan fleksibilitas lebih karena memungkinkan pembaruan *state* dan perubahan tampilan secara dinamis, tetapi sedikit lebih kompleks dalam pengelolaannya.

## Cara Mencoba 
1. Clone repo ini.
2. Buka terminal dan masuk ke direktori proyek.
3. Jalankan aplikasi menggunakan perintah `flutter run`.
4. Untuk mencoba versi `StatelessWidget`, pastikan `runApp(MyStatelessApp());` tidak di comment.
5. Untuk mencoba versi `StatefulWidget`, comment `runApp(MyStatelessApp());` dan uncomment `runApp(MyStatefulWidgetApp());`.

## Struktur Proyek
- **lib/main.dart**: Berisi kode untuk aplikasi counter menggunakan `StatelessWidget` dan `StatefulWidget`.

## Kesimpulan
Dengan memahami perbedaan antara `StatelessWidget` dan `StatefulWidget`, kita dapat memilih widget yang tepat untuk aplikasi kita berdasarkan kebutuhan pengelolaan *state*. `StatelessWidget` sangat baik untuk UI yang statis, sementara `StatefulWidget` lebih cocok untuk aplikasi yang membutuhkan perubahan dinamis berdasarkan input pengguna atau perubahan data lainnya.
