# <h1 align="center">Laporan Praktikum Modul 13  <br> Perintah Dasar Linux </h1>
<p align="center">Novita Syahwa Tri Hapsari - 2311104007</p>

## A. Dasar Teori

### a. Perintah Dasar
Secara umum, perintah pada Linux dijalankan melalui Bash Shell (/bin/bash). Bash berfungsi sebagai antarmuka yang menerima perintah dari pengguna dan meneruskannya ke sistem untuk dieksekusi.

### b. Aturan Dasar Penulisan Perintah
Linux bersifat case sensitive, sehingga perbedaan huruf besar dan kecil akan memengaruhi hasil eksekusi perintah. Format umum penulisan perintah Linux adalah:
    $ perintah [opsi] [parameter]
Keterangan:
- Perintah: Instruksi atau program yang dijalankan.
- Opsi: Digunakan untuk memodifikasi perilaku perintah (biasanya diawali dengan - atau --)
- Parameter: Objek yang dikenai perintah, seperti file atau direktori.

## B. Unguided

### I. Perintah-Perintah Dasar Linux

#### 1. Pada terminal Linux terdapat command prompt seperti ini: ubuntu@localhost:~$

a. Jalankan dan screenshot terminal Anda!
  ![alt text](61.png) 

b. Jelaskan arti dari command prompt milik Anda!

   Xinu adalah nama pengguna aktif, dan xinu-develop-end adalah nama host atau komputer yang digunakan. Direktori home user dapat dilihat dengan tanda "~" dan pengguna yang aktif ditunjukkan sebagai user biasa (bukan root).
   
#### 2. Setiap perintah pada Linux mempunyai bentuk umum: nama_perintah option command_line_argument

a. Jalankan dan screenshot perintah berikut ini: ls
   ![alt text](62.png) 

b. Apakah option dan parameter dari perintah di atas?
   - Nama perintah = ls
   - Option = tidak ada
   - Parameter = tidak ada

c. Apa fungsi dari perintah tersebut?

   Perintah ls digunakan untuk menampilkan daftar file dan folder pada direktori saat ini.

 d. Jalankan perintah berikut ini: ls -al /

   ![alt text](63.png) 

e. Apakah option dan parameter dari perintah di atas?

   - Nama perintah = ls
   - Option = -al
   - Parameter = /

f. Apa fungsi dari perintah tersebut?

   - Option -a digunakan untuk menampilkan file tersembunyi.
   - Option -l digunakan untuk menampilkan detail file dan folder.
   - Parameter / menunjukkan direktori root Linux.

g. Jelaskan mengapa perintah pada a dan e mempunyai hasil yang berbeda!

   Hasil berbeda karena ls hanya menampilkan isi direktori yang sedang aktif saat ini, sedangkan ls -al / menampilkan isi direktori root (/) secara detail termasuk file tersembunyi. 


#### 3. Melihat struktur direktori dan file pada Linux sama seperti melihat file dan direktori(folder) yang berada pada GUI. Pada Linux terdapat direktori utama yaitu “/” (root). Dibawah direktori root terdapat berbagai direktori yang lain seperti: home, etc, usr, dll. Contoh: program firefox terdapat pada path /usr/lib/firefox, berarti untuk mengakses firefox kita berjalan dari root kemudian direktori “usr” dilanjutkan direktori “lib” baru dapat mengeksekusi firefox

a. Jalankan dan tunjukan perintah: pwd

   ![alt text](64.png) 
   
 Apakah option dan parameter dari perintah tersebut?

   - Nama perintah = pwd
   - Option = tidak ada
   - Parameter = tidak ada

c. Apa fungsi perintah tersebut?

   Perintah pwd (Print Working Directory) digunakan untuk menampilkan lokasi atau direktori kerja saat ini.

   ### 4. Perpindahan

a. Jalankan dan screenshot perintah: cd /

   ![alt text](65.png) 

b. Apakah option dan parameter dari perintah tersebut?

   - Nama perintah = cd
   - Option = tidak ada
   - Parameter = /

c. Apa yang dilakukan perintah tersebut?

   Perintah cd / digunakan untuk berpindah ke direktori root (/) pada sistem Linux.

   #### 5. Direktori khusus

a. Lakukan dan screenshot perintah cd / kemudian lakukan perintah cd ~. Jelaskan hasil dari keduanya!

   ![alt text](66.png) 
   
   Perintah cd / memindahkan pengguna ke direktori root (/). Sedangkan cd ~ memindahkan pengguna ke direktori home user (/home/xinu). Perbedaannya adalah cd / menuju direktori utama sistem, sedangkan cd ~ menuju direktori milik pengguna yang sedang aktif.

   #### 6. Copy, rename dan delete file (screenshot setiap tahapan!)

a. Copylah file dari /proc/cpuinfo ke folder home Anda (/home/user/) menggunakan command pada terminal. Ganti user dengan username anda.

   ![alt text](6a.jpeg) 

b. Tunjukkan menggunakan perintah bahwa file tersebut benar-benar telah dicopy ke folder home Anda.

   ![alt text](6b.jpeg) 

c. Copy file dari /proc/uptime ke folder home Anda.

   ![alt text](6c.jpeg) 

d. Tunjukkan menggunakan perintah bahwa file tersebut benar-benar telah dicopy ke folder home Anda.

   ![alt text](6d.jpeg) 

e. Hapuslah file uptime di folder home Anda.

   ![alt text](6e.jpeg) 

f. Tunjukkan menggunakan perintah bahwa file tersebut benar-benar telah dihapus ke folder home Anda.

   ![alt text](6f.jpeg) 

g. Rename file cpuinfo di folder home Anda menjadi infocpu

   ![alt text](6g.jpeg) 


b. Lakukan perintah cd /proc/self. Buatlah perintah menggunakan cd .. agar dapat berpindah ke direktori / (root). Berapa kali perintah cd .. harus dieksekusi? Screenshot hasilnya!

   ![alt text](6h.jpeg) 

   Perintah cd .. harus dieksekusi 2 kali untuk berpindah dari /proc/self ke direktori root (/).

   #### 7. Membuat folder baru.

a. Buatlah folder baru dengan nama “nim_anda”.

  ![alt text](68.png)
  
b. Buatlah di dalam folder “nim_anda”, folder baru dengan nama “nama_anda”.

  ![alt text](69.png) 

  #### 8. Membaca manual

a. Bukalah fungsi manual untuk perintah “ls”

  ![alt text](70.png) 

b. Apa fungsi perintah “ls”?

   Perintah ls digunakan untuk menampilkan daftar file dan direktori.

c. Siapakah pencipta perintah “ls”?
   
writen by Torbjom Grandlund, David Mackenzie, and Jim Mereying.

d. Apakah arti dari -h dari manual ls?

   -h (human readable) digunakan untuk menampilkan ukuran file dalam format yang lebih mudah dibaca seperti KB, MB, GB.

e. Option apa yang harus digunakan agar dapat melihat direktori secara rekursif?

   -R digunakan untuk menampilkan isi direktori beserta subdirektori secara rekursif.

f. Bukalah fungsi manual untuk perintah “cp”

   ![8f](Image/8f.jpeg)

g. Apa fungsi perintah “cp”

   cp digunakan untuk menyalin (copy) file atau direktori.

h. Siapakah pencipta perintah “cp”?

   ![8h](Image/8h.jpeg)

i. Apakah arti -v dalam perintah “cp?

   -v (verbose) digunakan untuk menampilkan proses penyalinan secara detail.

j. Jika ingin interaktif, option apa yang harus digunakan?

   -i (interactive) meminta konfirmasi sebelum file ditimpa.
