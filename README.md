# belajar-docker
## Cerita
Disuatu hari yang cerah, dua sosok engineer devops sedang pusing dengan pekerjaannya. Engineer itu bernama Rizqi dan Wana. Mereka sedang duduk berdua sambil bertatapan penuh kasih sayang dikarenakan pusing dengan pekerjaan mereka untuk setup CDN, API, Wordpress dan DB Mysql. Bantulah mereka ya :).
### Komponen:
1. Docker CDN: https://nama.fathoniadi.dev/cdn-public
2. Docker API: https://api.nama.fathoniadi.dev
3. Docker Wordpress: https://nama.fathoniadi.dev
4. Docker DB Mysql Untuk Wordpress
5. Nginx di server
6. Certifiate agar bisa akses domain nama.fathoniadi.dev dan *.nama.fathoniadi.dev
Catatan: 
nama: disesuaikan masing-masing


Arsitektur:

![](./belajar-docker.jpg)


Aturan main:
1. CDN harus dibuat image terlebih dahulu tidak boleh mount manual. Isi image cdn berisi foto bang dedi di folder image.
2. CDN dapat diakses ketika mengakses url https://nama.fathoniadi.dev/cdn-public/image/dedi.jpeg
3. Domain diatur di nginx server
4. SSL diatur di nginx server
5. Semua harus dalam bentuk docker compose
6. API boleh dimount manual dari code dan config nginxnya
7. Config nginx dapat menggunakan nginx-default.conf dan di mount ke /etc/nginx/conf/sites-enabled/default
8. Code api di folder api 








