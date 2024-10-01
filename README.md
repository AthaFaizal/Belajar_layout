Praktikum 1
Langkah 1: Buat Project Baru
Buatlah sebuah project flutter baru dengan nama layout_flutter. Atau sesuaikan style laporan praktikum yang Anda buat.
Langkah 2: Buka file lib/main.dart Buka file main.dart lalu ganti dengan kode berikut. Isi nama dan NIM Anda di text title.
Langkah 3: Identifikasi layout diagram Langkah pertama adalah memecah tata letak menjadi elemen dasarnya:
Identifikasi baris dan kolom.Apakah tata letaknya menyertakan kisi-kisi (grid)?
Apakah ada elemen yang tumpang tindih?
Apakah UI memerlukan tab?
Perhatikan area yang memerlukan alignment, padding, atau borders.
Pertama, identifikasi elemen yang lebih besar. Dalam contoh ini, empat elemen disusun menjadi sebuah kolom: sebuah gambar, dua baris, dan satu blok teks.
berikut dibawah ini hasil dari praktikum 1
![1](https://github.com/user-attachments/assets/50263334-dcda-406e-b2e5-11c3e3c8eeba)
Praktikum 2
Langkah 1: Buat method Column _buildButtonColumn
Bagian tombol berisi 3 kolom yang menggunakan tata letak yang sama—sebuah ikon di atas baris teks. Kolom pada baris ini diberi jarak yang sama, dan teks serta ikon diberi warna primer.
Karena kode untuk membangun setiap kolom hampir sama, buatlah metode pembantu pribadi bernama buildButtonColumn(), yang mempunyai parameter warna, Icon dan Text, sehingga dapat mengembalikan kolom dengan widgetnya sesuai dengan warna tertentu.
lib/main.dart (_buildButtonColumn)
Langkah 2: Buat widget buttonSection Buat Fungsi untuk menambahkan ikon langsung ke kolom. Teks berada di dalam Container dengan margin hanya di bagian atas, yang memisahkan teks dari ikon.
Bangun baris yang berisi kolom-kolom ini dengan memanggil fungsi dan set warna, Icon, dan teks khusus melalui parameter ke kolom tersebut. Sejajarkan kolom di sepanjang sumbu utama menggunakan MainAxisAlignment.spaceEvenly untuk mengatur ruang kosong secara merata sebelum, di antara, dan setelah setiap kolom. Tambahkan kode berikut tepat di bawah deklarasi titleSection di dalam metode build():
lib/main.dart (buttonSection)
Langkah 3: Tambah button section ke body
Tambahkan variabel buttonSection ke dalam body
berikut dibawah ini hasil praktikum 2
![2](https://github.com/user-attachments/assets/4866a573-fcd6-4207-ab89-77b64ece76e2)
Praktikum 3
Langkah 1: Buat widget textSection
Tentukan bagian teks sebagai variabel. Masukkan teks ke dalam Container dan tambahkan padding di sepanjang setiap tepinya. Tambahkan kode berikut tepat di bawah deklarasi buttonSection:
Langkah 2: Tambahkan variabel text section ke body
Tambahkan widget variabel textSection ke dalam body seperti berikut:
berikut dibawah ini hasil dari praktikum 3
![3](https://github.com/user-attachments/assets/b172011c-e972-4575-8e40-88de4884fc3e)
Praktikum 4
Anda dapat mencari gambar di internet yang ingin ditampilkan. Buatlah folder images di root project layout_flutter. Masukkan file gambar tersebut ke folder images, lalu set nama file tersebut ke file pubspec.yaml seperti berikut:
Langkah 2: Tambahkan gambar ke body
Tambahkan aset gambar ke dalam body seperti berikut:
Langkah 3: Terakhir, ubah menjadi ListView
Pada langkah terakhir ini, atur semua elemen dalam ListView, bukan Column, karena ListView mendukung scroll yang dinamis saat aplikasi dijalankan pada perangkat yang resolusinya lebih kecil.
berikut adalah hasil praktikum 4
![4](https://github.com/user-attachments/assets/1edb1034-54c7-4b60-b724-e6378a726c12)
