# Nama : Chika Marsya Diandra Lumban Gaol

# Kelas : PBP F

## Link Adaptable untuk Tugas 2
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