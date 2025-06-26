# Aplikasi-Demo
By Dara Nabilah

Ini adalah tugas kuliah pemrograman 1

Selamat datang di proyek **Nama_Proyek_Anda_Di_Sini**! Repositori ini berisi kode sumber untuk aplikasi Java desktop yang dikembangkan menggunakan NetBeans dan terhubung dengan database MySQL.

## 🚀 Langkah-langkah Pengembangan Lokal

Ikuti langkah-langkah di bawah ini untuk mengatur dan menjalankan proyek ini di lingkungan pengembangan Anda (NetBeans).

### 1. Pembuatan Proyek di NetBeans

1.  Buka NetBeans IDE Anda.
2.  Pilih `File > New Project...`. 
3.  Pilih kategori `Java with Ant` (atau `Java with Maven`/`Gradle` jika preferensi Anda demikian) dan pilih `Java Application`. Klik `Next`.
4.  Pada kolom "Project Name", masukkan nama proyek Anda, contoh: `DaraNabilah`.
5.  Pastikan opsi "Create Main Class" tidak dicentang (jika Anda akan membuat struktur package terpisah).
6.  Klik `Finish`.

### 2. Struktur Package

Buat empat (4) package utama di dalam `Source Packages` proyek Anda:
* `p13`
* `p14`
* `p15`
* `p16`

**Cara membuat package:**
Klik kanan pada `Source Packages` > `New` > `Java Package...` > Masukkan nama package > `Finish`.

### 3. Pembuatan Class dan Kode

Lanjutkan untuk membuat Class (baik `JFrame Form` untuk GUI atau `Java Class` biasa) di dalam setiap package (`p13` hingga `p16`) sesuai dengan desain aplikasi Anda.

* Untuk menambahkan file, klik kanan pada package yang sesuai (`p13`, `p14`, dst.) > `New` > Pilih jenis file yang diperlukan (misal: `JFrame Form...` atau `Java Class...`).
* Isi setiap file Class dengan kode Java yang telah disediakan atau yang Anda kembangkan.

### 4. Pengelolaan Import Package

Pastikan setiap Class yang menggunakan Class lain dari package yang berbeda di-import dengan benar. NetBeans biasanya akan membantu dengan auto-import, namun pastikan sintaks `import` berada di bagian atas setiap file Java yang membutuhkan:

```java
import p13.NamaClassDariP13; // Contoh import class spesifik
import p14.*; // Contoh import semua class dari p14 (tidak selalu disarankan untuk project besar)

### 5. Setup Database MySQL (dengan XAMPP)

Aplikasi ini membutuhkan database MySQL. Ikuti langkah-langkah berikut untuk setup:

1.  Pastikan **XAMPP Control Panel** Anda berjalan dan layanan **Apache** serta **MySQL** telah diaktifkan.
    ![XAMPP Control Panel](images/xampp_control_panel.png) 
2.  Buka browser web Anda dan navigasi ke `http://localhost/phpmyadmin`.
    ![Tampilan phpMyAdmin](images/phpmyadmin_main_page.png) 
3.  Di phpMyAdmin, klik `New` di sidebar kiri atau tab `Databases`.
    ![Membuat Database Baru di phpMyAdmin](images/phpmyadmin_new_database.png) 
4.  Buat database baru dengan nama `db_aplikasifitness` (sesuai kebutuhan proyek Anda).
5.  Impor file `.sql` yang berisi skema dan data database Anda ke dalam `db_aplikasifitness` jika ada.
    ![Import SQL di phpMyAdmin](images/phpmyadmin_import_sql.png) 

### 6. Menambahkan MySQL Connector/J

Aplikasi Java Anda memerlukan driver JDBC untuk terhubung ke MySQL.

1.  Unduh `mysql-connector-j-9.3.0.jar` (atau versi terbaru yang kompatibel) dari [situs resmi MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/).
2.  Di NetBeans, di jendela `Projects`, klik kanan pada folder `Libraries` di bawah proyek Anda (`DaraNabilah`).
    ![Klik Kanan Libraries NetBeans](images/netbeans_right_click_libraries.png) 
3.  Pilih `Add JAR/Folder...`.
    ![Add JAR Folder NetBeans](images/netbeans_add_jar_folder.png) 
4.  Navigasi ke lokasi file `mysql-connector-j-9.3.0.jar` yang telah Anda unduh, pilih, dan klik `Open`.
    ![JAR MySQL Connector di Libraries](images/netbeans_mysql_connector_added.png) 

### 7. Menambahkan JDK untuk Kalender (dan Konfigurasi Platform)

Jika aplikasi Anda menggunakan komponen kalender yang memerlukan JDK 21, pastikan JDK 21 telah terinstal dan terkonfigurasi:

#### Untuk Library Kalender (jika ada JAR terpisah):

1.  Unduh file `.jar` untuk library kalender yang Anda gunakan (misalnya `JCalendar.jar`).
2.  Tambahkan `.jar` tersebut ke `Libraries` proyek Anda sama seperti langkah menambahkan MySQL Connector/J.
    ![Menambahkan Library Kalender NetBeans](images/netbeans_add_calendar_jar.png) #### Memastikan NetBeans Menggunakan JDK 21:

### 8. Menjalankan Aplikasi

Sebelum menjalankan aplikasi Anda, pastikan **XAMPP Apache dan MySQL** sedang berjalan.

1.  Di NetBeans, klik ikon `Run Project` (panah hijau) atau tekan `Shift + F6`.
    ![]() 
2.  Aplikasi Anda akan berjalan dan terhubung ke database MySQL yang telah Anda siapkan.
    ![]()
