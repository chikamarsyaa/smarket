# Nama : Chika Marsya Diandra Lumban Gaol

# Kelas : PBP F

---
## README TUGAS 2
---
### Link Adaptable untuk Tugas 2
[smarket app -->] (https://smarkettt.adaptable.app/)

---
### (1) Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step.
STEP : 

- Saya membuat project django baru yang namanya tidak sama dengan project saat tutorial. 
- Lalu, setelah membuat projek baru saya mengaktifkan virtual environment Django dengan menjalankan command berikut pada terminal ( "python -m venv env" dan "env\Scripts\activate" ).
- Setelah itu, saya membuat file baru bernama requirements.txt yang berisi dependencies yang akan diperlukan.
- Lalu, untuk mendownload dependenciesnya jalankan command berikut pada terminal ("pip install -r requirements.txt").
- Buka file settings.py, lalu siapapun yang ingin memberi host ketik “*” pada allowd host.
- Tambahkan berkas .gitignore agar dapat mengabaikan file file yang tidak diperlukan.
- Lalu, saya membuat aplikasi bernama main sesuai dengan perintah soal dengan menjalankan command ( “python manage.py startapp main" ).
- Di dalam folder main, saya membuat folder bernama templates yang nantinya akan diisi dengan file main.html yang digunakan untuk menampilkan aplikasi.
- Setelah itu, agar url file dapat saling terhubung saya membuat file baru bernama urls.py di dalam folder main dan menambahkan path baru 'path('', show_main, name='show_main).
- Lalu, pada file urls.py yang berada di folder smarket kita tambahkan path baru juga yaitu ‘main’ pada url patterns.
- Setelah itu, saya membuat atribut pada models.py sesuai dengan ketentuan soal.
- Lalu, klik views.py dan buat function yang mewakilkan atribut-atribut pada models.py tadi agar dapat di return pada main.html nantinya untuk ditampilkan secara statis.
- Setelah selesai dengan semua ketentuan file dan isinya, kita bisa melakukan add, push, commit ke repository github.
- Saat github sudah menerima kiriman update file tadi secara lengkap, kita bisa melakukan deploy di adaptable dengan cara menghubungkan repository github kita.

---
### (2) Buatlah bagan yang berisi request client ke web aplikasi berbasis Django beserta responnya dan jelaskan pada bagan tersebut kaitan antara urls.py, views.py, models.py, dan berkas html.
<img src="/Foto//bagan.jpg">

---
### (3) Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?

--> Kita menggunakan virtual environment untuk mengisolasi dependensi suatu project, menghindari konflik, dan menjaga kebersihan instalasi. Meskipun bisa, sangat disarankan untuk tetap menggunakan virtual environment saat membuat aplikasi web Django agar menghindari terjadinya project tidak terisolasi.

---
### (4) Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.

- MVC (Model-View-Controller): Paradigma pengembangan perangkat lunak yang memisahkan aplikasi menjadi tiga komponen: Model (data dan logika bisnis), View (tampilan), dan Controller (pengatur aliran aplikasi).

- MVT (Model-View-Template, digunakan dalam Django): Paradigma serupa dengan MVC, di mana Model mengelola data, View menampilkan data, dan Template merender tampilan.

- MVVM (Model-View-ViewModel): Paradigma pengembangan perangkat lunak yang memisahkan Model (data), View (tampilan), dan ViewModel (perantara antara data dan tampilan), umumnya fokus terhadap pemisahan antara tampilan, logika, dan data.

---
## README TUGAS 3
---
### (1) Apa perbedaan antara form POST dan form GET dalam Django?
--> Perbedaan utama antara metode POST dan GET dalam Django adalah bagaimana data dari formulir HTML dikirimkan ke server. Dalam metode POST, data formulir dikirim sebagai bagian dari tubuh permintaan HTTP, atau dapat dibilang data yang dikirimkan tidak ditampilkan secara terbuka pada URL browser. Sementara itu, dalam metode GET, data yang dikirimkan akan terlihat pada URL dan itu akan berguna untuk permintaan yang hanya mengambil informasi dari server tanpa melakukan perubahan pada data yang ada.

---
### (2) Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?
- XML (Extensible Merkup Language) 
XML adalah bahasa markup yang dirancang untuk menyimpan dan mengirim data struktural. XML sering digunakan dalam pertukaran data antara sistem yang berbeda karena fleksibilitasnya. Namun, XML cenderung memiliki format yang lebih panjang dan kompleks, sehingga membutuhkan lebih banyak bandwidth dan parsing yang lebih rumit.
- JSON (JavaScript Object Notation)
JSON adalah format pertukaran data yang ringan dan mudah dibaca oleh manusia.JSON lebih efisien dalam penggunaan bandwidth karena formatnya lebih ringkas dibandingkan dengan XML. JSON juga lebih mudah diproses oleh JavaScript.
- HTML (Hypertext Markup Language)
HTML adalah bahasa markup yang digunakan untuk membuat struktur dan tampilan halaman web. Meskipun tidak dirancang untuk pengiriman data, HTML dapat digunakan untuk menampilkan data dalam bentuk halaman web yang dapat diakses oleh pengguna melalui browser.

---
### (3) Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?
- Dapat melakukan pertukaran data dengan cepat
JSON mempercepat proses pertukaran data dengan menyediakan struktur data yang lebih sederhana dan kompak. Hal ini bertujuan untuk meminimalkan waktu pemrosesan data sehingga server dapat segera menampilkan data kepada pengguna.
- Penerjemahan data yang mudah dimengerti manusia
JSON mempermudah penerjemahan data ke bahasa manusia. Meskipun komputer hanya dapat memproses data dalam kode biner, JSON membantu menerjemahkan data ini ke dalam teks yang dapat dimengerti oleh manusia, memudahkan perbaikan atau penambahan kode.

---
### (4) Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

1. Buat file dengan nama forms.py
Langkah pertama, kita perlu membuat file forms.py. File ini akan  berisi variabel sesuai dengan model yang telah didefinisikan di file models.py.

2. Modifikasi file views.py
Selanjutnya, kita perlu melakukan beberapa modifikasi pada file views.py. Pertama, buat fungsi baru bernama create product. Tujuannya untuk membuat produk sesuai input user. Kita juga perlu mengubah bagian fungsi show_main yang ada di dalam views.py agar setiap produk yang telah diinput dapat disimpan.

3. Buat file create_product.html
Setelah itu, kita perlu membuat file create_product.html sebagai tampilan untuk input produk. File ini memiliki tombol add new product yang dapat mengarahkan user ke page input produk. Setelah produk diinput, pengguna akan langsung kembali ke main page untuk melihat input produk.

4. Routing 
Langkah terakhir, kita akan melakukan routing pada semua fungsi yang telah kita buat. Kita dapat menambahkan beberapa import yang diperlukan pada file views.py, lalu tambahkan juga beberapa path baru untuk memanggil fungsi melalui URL. 
Berikut adalah isi dari urls.py : 
<img src="/Foto//urls.py.png">

---
### (5) Screenshot hasil akses URL pada Postman.
(a) HTML 
<img src="/Foto//html.jpg">
(b) XML 
<img src="/Foto//xml.jpg">
(c) JSON 
<img src="/Foto//json.jpg">
(d) XML ID
<img src="/Foto//xml[1].jpg">
(e) JSON ID 
<img src="/Foto//json[1].jpg">

---
## README TUGAS 4
---
### (1) Apa itu Django UserCreationForm, dan jelaskan apa kelebihan dan kekurangannya?
- Django UserCreationForm merupakan salah satu form yang disediakan oleh django, form ini dirancang khusus untuk membuat dan mendaftarkan pengguna baru dalam aplikasi web yang akan dibangun dengan Django. Form ini juga menyediakan beberapa fitur umum untuk proses pendaftaran, seperti username, password, dan kata sandi. 
- Berikut adalah beberapa kelebihan dan kekurangan yang dimiliki oleh Django UserCreationForm :
---
(+) Kelebihan
- Validasi Terintegrasi
- Mudah untuk dikustomisasi sesuai dengan kebutuhan project
- Form terhubungan dengan model bawaan django, sehingga menyederhanakan proses penyimpanan informasi ke dalam database
---
(-) Kekurangan 
- Terbatas pada fitur dasar
- Tampilan default yang cukup sederhana

---
### (2) Apa perbedaan antara autentikasi dan otorisasi dalam konteks Django, dan mengapa keduanya penting?
-> Dalam konteks django, autentikasi dan otorisasi merupakan dua konsep yang sangat penting dalam mengelola akses pengguna kedalam aplikasi web. Perbedaan utama antara keduanya adalah : 
1. Autentikasi 
- Autentikasi adalah proses memverivikasi identitas pengguna, sistem akan mengonfirmasi apakah pengguna yang ingin mengakses aplikasi adalah orang yang sudah diklaim dalam website atau tidak. 
- Pada Django, autentikasi melibatkan beberapa identitas pengguna seperti, username dan password.

2. Otorisasi
- Otorisasi adalah proses yang menentukan apa saja yang dapat dilakukan oleh user yang telah berhasil dalam proses autentikasi. Sistem mengontrol akses pengguna terhadap fitur dalam aplikasi. 
- Pada Django, otorisasi dilakukan dengan memeriksa permission yang diberikan kepada penggguna. Permission ini dapat mengatur apakah pengguna memiliki hak akses untuk melakukan operasi tertentu, seperti mengedit atau menghapus data. 

---
### (3) Apa itu cookies dalam konteks aplikasi web, dan bagaimana Django menggunakan cookies untuk mengelola data sesi pengguna?
- Cookies adalah istilah untuk kumpulan informasi yang berisi rekam jejak atau aktivitas ketika menelusuri sebuah website, atau secara sederhana Cookies merupakan kumpulan data yang diterima komputer dari sebuah situs dan mengirimkan kembali ke situs yang dikunjungi. 
- Django menggunakan cookies untuk mengelola data sesi pengguna, seperti menyimpan data login pengguna, menyimpan data sesi, dan juga berfungsi untuk mengamankan cookie. Hal ini yang dapat membuat Django menyimpan informasi sesi pengguna dengan aman dan mengaksesnya kembali ketika pengguna melakukan permintaan ulang.

---
### (4) Apakah penggunaan cookies aman secara default dalam pengembangan web, atau apakah ada risiko potensial yang harus diwaspadai?
-  Penggunaan cookies dalam pengembangan web adalah alat yang umum  digunakan untuk mengelola data sesi pengguna, tetapi ada beberapa risiko potensial yang harus diwaspadai, yaitu :
1. Kebocoran data
2. Serangan Cross-Site Scripting
3. Serangan Man-In-The-middle   
4. Saat cookies disimpan dalam log server, informasi sensitif dapat menjadi rentan jika log tersebut tidak diamankan.

Beberapa tindakan preventif yang dapat dilakukan untuk mencegah risiko diatas yaitu : 
1. Memastikan log server tidak mencatat informasi sensitif.
2. Pastikan website menggunakan Perlindungan CSRF yang disediakan oleh Django atau modul terpercaya lainnya.
3. Pastikan untuk mengaktifkan enkripsi cookie pada website. 

---
### (5) Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
- Mengaktifkan virtual environment terlebih dahulu 
- Mengimpor beberapa modul yang diperlukan, seperti UserCreationForm
- Membuat fungsi register untuk menghasilkan formulir registrasi secara otomatis
- Membuat berkas HTML yang digunakan sebagai tampilan dari hasil form pendaftaran akun user ketika data telah disubmit.
- Mengimpor fungsi "register" ke dalam berkas urls.py dan menambahkan path URL ke dalam urlpatterns.
- Mengimpor fungsi login dengan nama "login_user" dan authenticate dengan langkah yang sama. 
- Membuat fungsi logout, dengan mengimpor modul "logout"
- Pada berkas main.html yang dimiliki oleh fungsi logout diperlukan sebuah tag hyperlink.
- Untuk melakukan proses otorisasi, kita dapat menggunakan modul "login_required" untuk membatasi akses pengguna. 
- Proses diatas dilakukan dengan menambahkan kode "@login_required(login_url='/login')" di atas fungsi show_main pada views.py agar halaman main hanya dapat diakses oleh pengguna yang sudah login (terautentikasi).
- Selanjutnya, kita perlu membuat dua akun untuk menghubungkan Item dan Product, dengan cara menambahkan import User ke dalam models.py.
- Melakukan beberapa modifikasi pada fungsi create_product di views.py agar Django dapat mengenali bahwa objek dimiliki oleh pengguna. 
- Setelah itu, lakukan migrasi untuk menyimpan semua perubahan pada sistem. 

---
## README TUGAS 5
---

### (1) Jelaskan manfaat dari setiap element selector dan kapan waktu yang tepat untuk menggunakannya.
- Selektor ID 
-> Selektor ini berfungsi untuk memilih elemen HTML berdasarkan atribut ID. Atribut ID harus bersifat unik, dan selektor ini berguna saat kita ingin menerapkan style pada elemen tertentu. 

- Element Style
-> Element ini berisi informasi gaya untuk dokumen atau bagian dari dokumen. Bisa dibuat dalam file yang berbeda yaitu CSS, yang nantinya file css akan dipanggil untuk menerapkan elemen dalam HTML.

- Selector Class
-> Selector ini berfungsi untuk memilih elemen HTML berdasarkan atribut kelas. Syntax yang digunakan yaitu <div class = "profile"> maka selektor ini akan membantu menerapkan gaya pada class profile.

- Selector Universal
-> Selector ini berfungsi untuk memilih semua elemen pada HTML. Syntax yang digunakan yaitu "*". Selector ini dapat berguna ketika kita ingin menerapkan style yang sama pada seluruh elemen.

---
### (2) Jelaskan HTML5 Tag yang kamu ketahui.
- <html>	--> untuk memulai dokumen HTML
- <head>	--> untuk membuat bagian head
- <body>	--> untuk membuat bagian body
- <h1> sampai <h6>	--> untuk membuat heading pada artikel
- <p>	    --> untuk membuat paragraf
- <table>   --> untuk membuat sebuah tabel
- <!-- -->	--> untuk membuat komentar

---
### (3) Jelaskan perbedaan antara margin dan padding.
- MARGIN
-> Margin merupakan sisi luar dari sebuah elemen, digunakan saat kita ingin mengatur jarak antar elemen. Ada beberapa syntax margin yang dapat digunakan, yaitu margin-top, margin-left, margin-right,dll. Namun, jika kita menggunakan syntax margin saja maka akan secara otomatis mengatur jarak atas, bawah, kiri, dan kanan elemen. Margin tidak memiliki background color. 

- PADDING
-> Padding merupakan sisi dalam dari sebuah elemen, digunakan untuk mengatur jarak pada sisi dalam sebuah elemen yang bisa kita tentukan. Padding juga memiliki beberapa syntax yang mirip dengan margin, yaitu padding-top, padding-left, padding-right,dll. Dan sama seperti margin, apabila hanya menulis syntax padding saja, maka posisi sudah diatur jarak atas, bawah, kiri, dan kanan elemen. Berbeda dengan margin, padding memilki background color yang bisa digunakan untuk elemen pada HTML.

---
### (4) Jelaskan perbedaan antara framework CSS Tailwind dan Bootstrap. Kapan sebaiknya kita menggunakan Bootstrap daripada Tailwind, dan sebaliknya?
- Tailwind CSS dan Bootstrap adalah dua framework CSS yang populer dan digunakan untuk mempercepat pengembangan tampilan web. Kedua framewrok ini juga memiliki perbedaan, yaitu : 
1. Tailwind CSS lebih memprioritaskan utilitas dan fleksibelitas dalam membuat design custom dengan menggunakan class yang sudah ditulis sebelumnya.
2. Bootstrap lebih berfokus pada komopnen yang siap pakai dan responsive terhadap beberapa ukuran dan Bootstrap juga menyediakan tema dan template yang mudah untuk digunakan. 

- Kapan kita menggunakan Tailwind CSS ?
1. Saat kita menginginkan design dengan tingkat customization yang tinggi dan fleksible
2. Saat ingin menghasilkan kode HTML yang lebih bersih tanpa tambahan kelas yang tidak perlu.

- Kapan kita menggunakan Bootstrap ?
1. Saat kita ingin membuat tampilan yang mudah digunakan dan cepat
2. Bootstrap sangat cocok untuk situs web sederhana yang umum dan simple

---
### (5) Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

