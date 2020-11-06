# NOBSK

[![hackmd-github-sync-badge](https://hackmd.io/g57oFvBCQJ2kNNN1_pBp3g/badge)](https://hackmd.io/g57oFvBCQJ2kNNN1_pBp3g)


NOBSK is a minimal, attractive, milenial short film screening for Indonesian Film Festival.

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

1. Download .zip / Clone repository nobsk. Atau rekomendasi download release versi beta kami: https://github.com/nobsk/nobsk.github.io/releases/tag/v1.0.0-beta.1
2. Extract .zip yang sudah didownload, letakkan pada folder webroot/htdocs pada web server yang ada pada mesin (xampp, mamp, lamp)
3. Akses dengan url: http://localhost/<nama_folder>




## Amy: Adorable Machine Yawner - The Next Website Assistant (Amy > Chatbot)

Amy != chatbot, karena basisnya adalah integrasi dari speech recognition dan synthesize lalu mampu melakukan event/tindakan terhadap aplikasi. Amy digunakan untuk navigasi, berpindah halaman, login, logout, mencari film, dan memutar film.

Amy mampu mendeteksi kalimat, di mana di dalam sebuah kalimat tersebut ada sebuah keyword. Amy akan menjalankan perintah berdasarkan keyword terakhir yang diucap. Misalnya:

"Halo amy, saya mau nonton ***film*** di sini bagaimana ya caranya?"

berdasarkan database, kata "***film***" adalah keyword yang tersedia, dan kata tersebut dalam kalimat di atas diucapkan terakhir (selebihnya tidak ada kata yg cocok pada database). Maka amy akan menjalankan perintah "film".
### Keywords

Keyword yang bisa digunakan saat bertanya pada Amy:

"Login", "Register", "Terima kasih", "Duluan", "Film", "Pendek", "Rekomendasi", "Halo", "Hai", "Logout", "Masuk", "Daftar", "Kopi", "Boleh", "Teh", "Tutup", "Pagi", "Siang", "Sore", "Malam", "Ya", "Iya", "Logout", "Keluar", "No", "Nggak", "Susu", "Milk", "Mau", "Festival", "Emi", "Watchlist", "Baru", "Rilis", "Comingsoon", "Profil", "favorite", "favorit", "akun", "Bantuan", "Help", "Tilik", "Detail".

Amy juga mampu melakukan nested question dengan keyword:

"pagi",
"siang",
"sore",
"malam"

dan ikuti amy seterusnya untuk menjawab pertanyaannya.

Berikut contoh penggunaan Amy. (Maaf jika bahasa yang diujicobakan sangat random.)
[![Amy](http://img.youtube.com/vi/zOL0_gS4VxE/0.jpg)](http://www.youtube.com/watch?v=zOL0_gS4VxE "Amy.")

Untuk menyembunyikan Amy cukup dengan bilang:
"Sembunyikan", maka amy akan hilang secara otomatis.

### Sequence Diagram Amy
![](https://i.imgur.com/rTWliHV.png)

### Tested
Mozilla Firefox & Google Chrome (Desktop & Mobilephone)

## UseCase Diagram

![](https://i.imgur.com/8EjdwIJ.png)


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