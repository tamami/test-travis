## Langkahnya 

1. buat file `.travis.yml`

1. jalankan perintah `php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"` untuk download installer

2. jalankan perintah 
```
php -r "if (hash_file('SHA384', 'composer-setup.php') === '544e09ee996cdf60ece3804abc52599c22b1f40f4323403c44d44fdfdd586475ca9813a858088ffbc1f233e9b180f061') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
```
untuk verifikasi installer

3. jalan perintah `php composer-setup.php` untuk jalankan instalasi

4. jalankan perintah `php -r "unlink('composer-setup.php');"` untuk hapus file sampah

5. buat file `composer.json`, 

6. jalankan perintah `php composer.phar install`, perlu koneksi internet

7. jalan perintah `composer require phpunit/phpunit`

8. buat file `phpunit.xml`

9. buat file `index.php` dan `result.php`

10. push ke github.

11. cek halaman travis-ci.org, aktifkan repositori-nya

12. lakukan commit untuk men-trigger build script di travis