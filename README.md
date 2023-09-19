# Nama : Chika Marsya Diandra Lumban Gaol

# Kelas : PBP F


## README UNTUK TUGAS 2
### Link Adaptable untuk Tugas 2
[smarket app -->] (https://smarkettt.adaptable.app/)

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


### (2) Buatlah bagan yang berisi request client ke web aplikasi berbasis Django beserta responnya dan jelaskan pada bagan tersebut kaitan antara urls.py, views.py, models.py, dan berkas html.
<img src="/Foto//bagan.jpg">


### (3) Jelaskan mengapa kita menggunakan virtual environment? Apakah kita tetap dapat membuat aplikasi web berbasis Django tanpa menggunakan virtual environment?

--> Kita menggunakan virtual environment untuk mengisolasi dependensi suatu project, menghindari konflik, dan menjaga kebersihan instalasi. Meskipun bisa, sangat disarankan untuk tetap menggunakan virtual environment saat membuat aplikasi web Django agar menghindari terjadinya project tidak terisolasi.

### (4) Jelaskan apakah itu MVC, MVT, MVVM dan perbedaan dari ketiganya.


- MVC (Model-View-Controller): Paradigma pengembangan perangkat lunak yang memisahkan aplikasi menjadi tiga komponen: Model (data dan logika bisnis), View (tampilan), dan Controller (pengatur aliran aplikasi).

- MVT (Model-View-Template, digunakan dalam Django): Paradigma serupa dengan MVC, di mana Model mengelola data, View menampilkan data, dan Template merender tampilan.

- MVVM (Model-View-ViewModel): Paradigma pengembangan perangkat lunak yang memisahkan Model (data), View (tampilan), dan ViewModel (perantara antara data dan tampilan), umumnya fokus terhadap pemisahan antara tampilan, logika, dan data.

## README TUGAS 3

### (1) Apa perbedaan antara form POST dan form GET dalam Django?
--> Perbedaan utama antara metode POST dan GET dalam Django adalah bagaimana data dari formulir HTML dikirimkan ke server. Dalam metode POST, data formulir dikirim sebagai bagian dari tubuh permintaan HTTP, atau dapat dibilang data yang dikirimkan tidak ditampilkan secara terbuka pada URL browser. Sementara itu, dalam metode GET, data yang dikirimkan akan terlihat pada URL dan itu akan berguna untuk permintaan yang hanya mengambil informasi dari server tanpa melakukan perubahan pada data yang ada.

### (2) Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?
--> XML (Extensible Merkup Language) 
XML adalah bahasa markup yang dirancang untuk menyimpan dan mengirim data struktural. XML sering digunakan dalam pertukaran data antara sistem yang berbeda karena fleksibilitasnya. Namun, XML cenderung memiliki format yang lebih panjang dan kompleks, sehingga membutuhkan lebih banyak bandwidth dan parsing yang lebih rumit.
--> JSON (JavaScript Object Notation)
JSON adalah format pertukaran data yang ringan dan mudah dibaca oleh manusia.JSON lebih efisien dalam penggunaan bandwidth karena formatnya lebih ringkas dibandingkan dengan XML. JSON juga lebih mudah diproses oleh JavaScript.
--> HTML (Hypertext Markup Language)
HTML adalah bahasa markup yang digunakan untuk membuat struktur dan tampilan halaman web. Meskipun tidak dirancang untuk pengiriman data, HTML dapat digunakan untuk menampilkan data dalam bentuk halaman web yang dapat diakses oleh pengguna melalui browser.

### (3) Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?
- Dapat melakukan pertukaran data dengan cepat
JSON mempercepat proses pertukaran data dengan menyediakan struktur data yang lebih sederhana dan kompak. Hal ini bertujuan untuk meminimalkan waktu pemrosesan data sehingga server dapat segera menampilkan data kepada pengguna.
- Penerjemahan data yang mudah dimengerti manusia
JSON mempermudah penerjemahan data ke bahasa manusia. Meskipun komputer hanya dapat memproses data dalam kode biner, JSON membantu menerjemahkan data ini ke dalam teks yang dapat dimengerti oleh manusia, memudahkan perbaikan atau penambahan kode.

### (4) Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

### (5) Screenshor hasil akses URL pada Postman.
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

