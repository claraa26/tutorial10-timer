# Nama: Clara Sista Widhiastuti
# NPM: 2206825782
# Kelas: AdvPro A


### 1.2. Understanding how it works.
![](https://imgur.com/jY0mdXh.jpg)

Diketahui bahwa pemanggilan howdy dan done terjadi secara asynchronous, dan akan dieksekusi setelah diproses oleh executor
sedangkan hey hey terdapat pada program utama dan sebelum executor, sehingga memberikan output seperti di gambar.

### 1.3. Multiple Spawn and removing drop
![](https://imgur.com/0plf8Oo.jpg)

Pada kali ini saya telah memodifikasi untuk membuat spawner.spawn menjadi ada 3 dan menghapus drop(spawner). Pada output
tercetak howdy terlebih dahulu sebanyak 3 kali baru tercetak done. Hal tersebut karna program berjalan secara asychronous. 
Executor akan mengekseskusi taks pertama terlebih dahulu hingga selesai yaitu output howdy baru task selanjutnya hingga 
done tereksekusi. Sedangkan penghapusan drop(spawner) mengakibatkan program tidak berhenti, karena program menunggu 
task-task selanjutnya.