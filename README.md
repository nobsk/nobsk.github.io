# NOBSK

[![hackmd-github-sync-badge](https://hackmd.io/g57oFvBCQJ2kNNN1_pBp3g/badge)](https://hackmd.io/g57oFvBCQJ2kNNN1_pBp3g)


NOBSK is a minimal, attractive, milenial short film screening for Indonesian Film Festival. NOBSK adalah web-aplikasi yang untuk festival film pendek di Indonesia. Term ‘NOBSK.’ merupakan singkatan dari kata “NOnton-film-pendek Bareng SKuy”, di mana tujuan dari web-aplikasi ini selain untuk menyediakan screening karya film pendek oleh para pegiat film pendek di Indonesia yang bisa ditonton oleh siapa saja tanpa harus keluar rumah alias “short-film screening from home”, NOBSK juga memiliki fungsi sebagai “call for entries and festivals” yaitu manajemen film pendek untuk para Organizer. Ada beberapa role pada web-aplikasi ini: Short-film Organizer, Filmmaker/Participant, Reviewer dan Guest. NOBSK didesain dengan model interaksi yang minimalis, millennial-friendly, responsive, dan easy to navigate, sehingga harapan pengamalan berselancar di web-aplikasi ini tak kalah dengan berada di short-film screening fisikal. NOBSK memiliki inovasi dalam hal interaksinya, yaitu "Amy" sebagai tiny-based AI yang kami buat sebagai "penunggu" dari NOBSK yang dapat membantu user melakukan navigasi dan berselancar di NOBSK (Apa itu Amy? Akan dijelaskan pada poin selanjutnya).

Dekade ini, kreativitas anak bangsa di dunia perfilman tidak bisa dianggap remeh, terutama di kancah film pendek. Sudah banyak penghargaan Internasional yang didapatkan atas karya orisinil film pendek karya anak bangsa. Festival Film Pendek adalah suatu event di mana para filmmaker bisa berpartisipasi dan berkarya, meningkatkan kemampuan dengan bantuan para reviewer yang tergabung dalam festival, serta bisa terhubung dengan filmmaker lainnya. Untuk itulah NOBSK hadir sebagai solusi yang menyediakan wadah untuk berkumpulnya para filmmaker, organizer, reviewer, dan penggemar film pendek untuk menciptakan karya film pendek orisinil dan meningkatkan kualitas perfilman Indonesia.

*Kelompok:*
- **Alfian Firmansyah | 1706985874**
- Kristian Girsang | 1706986012
- Samuel Natanael | 1706986076

---

![](https://i.imgur.com/Z4F7a52.png) ==>> ![](https://i.imgur.com/QIT6a41.png)


![](https://i.imgur.com/NOAPU1T.png)
---
![](https://i.imgur.com/RyfcitG.jpg)
---
![](https://i.imgur.com/hbmiH7U.png)

## Demo

Tidak perlu menginstall pada mesin, maka bisa mengunjungi url environment nobsk pada link berikut: [di sini](https://nobsk.herokuapp.com)

## Installation

Catatan: Tidak direkomendasikan untuk membuka `index.html` secara langsung, karena ada beberapa dependensi yang dijalankan melalui webserver. Maka dari itu, berikut langkah yang dapat diikuti.

1. Download .zip / Clone repository nobsk. Atau rekomendasi download release versi stable kami: https://github.com/nobsk/nobsk.github.io/releases/tag/v1.0.0
2. Extract .zip yang sudah didownload, letakkan pada folder webroot/htdocs pada web server yang ada pada mesin (xampp, mamp, lamp)
3. Akses dengan url: http://localhost/<nama_folder>


## Amy: Adorable Machine Yawner - The First Website Assistant by nobsk

Mengapa kami membuat Amy? jawabannya adalah interactivity. Response komunikasi tercepat manusia adalah auditory atau response suara yaitu sekitar 150 ms. Sedangkan visual berada pada 200 ms, dan pain berada pada 700 ms. Amy membuat komunikasi antar sistem dan manusia menjadi "sedikit lebih dekat" dan natural, karena pada umumnya manusia berkomunikasi secara verbal dan mengeluarkan suara, dan mendapatkan feedback melalui suara pula. Sedangkan di waktu senggang mungkin ada beberapa yang melalui visual seperti chat dan sebagainya. Amy membuat komunikasi antar pengguna dan aplikasi menjadi lebih natural dan lebih dekat, dialog akan bersifat robust (kami tidak tahu apakah jika komunikasi lewat gelombang otak lebih natural?). Diharapkan dengan hadirnya "Amy", sistem tesebut bisa menjadi sebuah success factor yang menjadi pembeda dengan sistem lain yang tersebar diluar sana, karena kami percaya bahwa "Amy" adalah yang pertama sebagai Artificial Intelligent dan Website Assistant dengan metode interaksi suara dan speech synthesis. (Berbekal dari Skripsi berjudul: Implementasi Sistem Bantuan Penderita Buta Warna: Interaksi Suara Untuk Perangkat Tertanam Dengan Sistem Operasi Tertanam Microsoft oleh Dr. Ruki Harwahyu, ST. MT. Msc. 2011)

Amy bukanlah chatbot, karena basisnya adalah integrasi dari speech recognition dan synthesize lalu mampu melakukan event/tindakan secara langsung terhadap aplikasi (dan chatbot tidak melakukan itu). Amy digunakan untuk navigasi, berpindah halaman, login, logout, mencari film, dan memutar film. 

Amy mampu mendeteksi kalimat, di mana di dalam sebuah kalimat tersebut ada sebuah keyword. Amy akan menjalankan perintah berdasarkan keyword terakhir yang diucap. Misalnya:

"Halo amy, saya mau nonton ***film*** di sini bagaimana ya caranya?"

berdasarkan database, kata "***film***" adalah keyword yang tersedia, dan kata tersebut dalam kalimat di atas diucapkan terakhir (selebihnya tidak ada kata yg cocok pada database). Maka amy akan menjalankan perintah "film".
### Keywords

Keyword yang bisa digunakan saat bertanya pada Amy:

`Login` `Register` `Terima kasih` `Duluan` `Film` `Pendek` `Rekomendasi` `Halo` `Hai` `Logout` `Masuk` `Daftar` `Kopi` `Boleh` `Teh` `Tutup` `Pagi` `Siang` `Sore` `Malam` `Ya` `Iya` `Logout` `Keluar` `No` `Nggak` `Susu` `Milk` `Mau` `Festival` `Emi` `Watchlist` `Baru` `Rilis` `Comingsoon` `Profil` `favorite` `favorit` `akun` `Bantuan` `Help` `Tilik` `Detail`.

Amy juga mampu melakukan nested question dengan keyword:

`pagi`
`siang`
`sore`
`malam`

dan ikuti amy seterusnya untuk menjawab pertanyaannya.

Berikut demo penggunaan Amy. (Maaf jika bahasa yang diujicobakan sangat random dan tidak formal.)
[![Amy](http://img.youtube.com/vi/zOL0_gS4VxE/0.jpg)](http://www.youtube.com/watch?v=zOL0_gS4VxE "Amy.")

Untuk menyembunyikan Amy cukup dengan bilang:
`Sembunyikan` maka amy akan hilang secara otomatis.

### Sequence Diagram Amy
![](https://i.imgur.com/rTWliHV.png)

Sequence diagram amy memiliki 4 object utama:
- SpeechRecognition: adalah API dari Chrome dan Mozillafirefox (akan difungsikan keduanya menggunakan *case*)
- Engine Event: Engine event adalah sekumpulan algoritma yang dibuat sebagai "handler/controller" dari input yang diterima, memprosesnya dan memberikan event serta feedback/output. Basis engine ini adalah murni javascript dan dikombinasikan dengan JQuery.
- Speech Synthesis: Speech synthesize yang kami gunakan juga berbasis javascript, yaitu dengan menggunakan suara wanita ber-bahasa inggris (untuk saat ini belum ada bahasa indonesia yang native). Kami memberi nama amy, karena service Amazon Polly dengan accent en-Us adalah Amy.
- DISPLAY: Display adalah file berekstensi `.html` yang akan menampilkan hasil dari event yang dilakukan oleh amy, dan juga menampilkan halaman dengan functional lainnya.

### Tested
Mozilla Firefox & Google Chrome (Desktop & Mobilephone)


## Usage Workflow: Lengkap

**General:**
1. User membuka halaman utama
2. Bisa mendaftarkan akun (dengan hanya menekan tombol register dan disini sengaja dibuat gagal daftar)
3. Bisa login (ketika klik tombol login, bisa login ke dalam sistem)
4. Ketika sudah di dalam sistem maka ada 4 navigasi utama: Film Pendek, Festival, Watchlist, Baru Rilis, dan Coming Soon. Bisa dipilih dengan interaksi klik pada mouse, atau dengan bantuan "*Amy*".
5. Pada halaman yang sama, terdapat dropdown di bagian kanan atas, di sana terdapat: Profil Saya, Favorit Saya, Pengaturan Akun, Bantuan, dan Logout. Interaksi yang bisa dilakukan bisa diklik secara manual, atau juga dengan bantuan "*Amy*"

Halaman Film pendek:
1. User dapat melakukan Play Film Pendek pada slider
2. User dapat memilih 1 film dalam suatu kategori dengan klik pada tiap card, maka akan diarahkan ke halaman detail dari film tersebut (Atau bisa dengan bantuan "Amy" dengan keyword "**Detail**")
3. bisa melakukan scrolling, dan akan muncul infinite scrolling
4. User dapat melakukan upload film baru (individual), dengan klik upload film pendek
![upload-2](images/upload2.gif)

Halaman Film Detail:
1. Halaman Film Detail bisa diakses melalui card-card film yang tersedia, atau dengan bantuan "Amy" dengan keyword `detail`
2. Di halaman ini, user dapat memutar video, membaca deskripsi, melihat review sebelumnya, melihat komentar sebelumnya, dan menambahkan komentar
3. Setiap komponen dapat diklik dengan muncul suatu aksi tertentu
4. Memutar video bisa dilakukan dengan Amy dengan keyword "Putar"
5. Sembunyikan amy dengan keyword "Sembunyikan"
6. Halaman ini didesain untuk responsive di semua device.
![](https://i.imgur.com/8gYjafY.jpg)

Halaman Festival:
1. Halaman festival bisa diakses dengan menggunakan navigasi sidebar di sisi kiri, dan juga dengan bantuan "Amy" dengan keyword `festival`
2. Di halaman ini bisa melakukan pembuatan festival dengan menekan tombol Buat Festival.
3. Halaman ini didesain dengan responsivitas dan juga infinite scrolling "Semua Festival"

Pada bagian kanan atas, terdapat beberapa halaman user, yaitu Profil Saya, Favorit Saya, Pengaturan Akun, Bantuan, dan Logout. Semua halaman ini bisa diakses langsung dengan klik, dan juga dengan bantuan "Amy".

## UseCase Diagram

![use-case](https://i.imgur.com/2p0r8fw.png)


UseCase dari website terdapat 5 bagian, yaitu
1. Festival Owner: 
  Festival owner memiliki 2 hal yang bisa dilakukan setelah login ke dalam website, yaitu Request festival dan Create festival. Request festival akan langsung diteruskan ke admin dan admin bisa memberikan fee payment dan approval dari request yang diberikan festival owner. Setelah melakukan create festival, festival owner akan me-manage short film yang ada di dalam festival yang sudah dibuat.
    
2. Participant: 
  Participant dapat melakukan upload short film ke dalam festival yang sedang berlangsung, kemudian bisa melakukan manage terhadap short film nya masing-masing. Setelah upload, admin akan menyaring setiap film yang diupload oleh participant dan memberikan approval dari film yang diupload.
    
3. Reviewer: 
  Reviewer memiliki 4 hal yang bisa dilakukan di dalam website, yaitu mnginvite reviewer lain, submit review, menonton film yang sudah diupload, dan melakukan vote winner film festival. Invite reviewer lain ini dilakukan agar reviewer lain juga bisa melakukan manage short film. hasil voting dari reviewer juga akan masuk ke dalam manajemen dari setiap short film tersebut sehingga jumlah vote bisa dilihat dan ditentukan siapa pemenangnya.

4. Guest: 
  Guest hanya bisa menonton film dan submit comment di dalam website. Setelah memasukkan comment, admin akan melakukan remove inappropriate comment. 

5. Admin
  Admin akan menerima data yang dimasukkan ke dalam website. Kemudian dapat melakukan manajemen terhadap setiap short film, setiap comment, dan participant yang mengambil bagian dalam website. Admin juga mengatur payment kepada setiap participant dan festival owner di dalam website.


## Technologies

Bootstrap4
JQuery
undraw.co
Polly SDK
Chrome & Mozilla SpeechRecognition
skrn

## Infinite Scrolling
![infinite-scrolling](images/infinite.gif)

## Skeleton Loader + Infinite Scrolling
![skeleton-loader](images/skeleton.gif)

## Smooth Loadmore Section
![smooth-loadmore](images/loadmore.gif)

## Multiple Item touch horizontal scrollable and beautiful Toast Notification
![multiple-slider-custom-toast](images/slider.gif)

## Video Player
![video-player](images/player.gif)

## Uploader Progressbar
![progress-bar](images/upload.gif)
