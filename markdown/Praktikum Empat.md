# Praktikum Empat: File dan Direktori

![file-directory](img/file-directory.jpg)

## Outline

- [Operasi Direktori.](##Operasi Direktori)
- [Operasi File dan Direktori.](##Operasi File dan Direktori)
- [Challenge.](##Challenge)

## Operasi Direktori

#### Teori

**1. File**

Koleksi data yang disimpan di hardisk dan dapat dimanipulasi sebagai unit tunggal dengan namanya.

**2. Direktori**

File yang berperan sebagai wadah untuk file lainnya.

Directori dapat berisi directori lain yang disebut sebagai Subdirektori.

Direcotri yang menampung directory lain disebut Directori Induk atau Parent Directori.

**3. Struktur Direktori**

**Windows**

![windows-structure](img/windows-structure.jpg)

**Linux**

![linux-structure](img/linux-structure.png)

#### Praktikum

**1. ls: listing information**

![ls](img/ls.jpg)

`ls` adalah perintah untuk menampilkan isi direktori

- menampilkan isi direktori: `ls`.
- menampilkan isi direktori (format list): `ls -l`.
- menampilkan isi direktori (format list & all): `ls -la`.
- menampilkan isi direktori /etc: `ls -l /etc`.

**2. pwd: print working directory**

![pwd](img/pwd.jpg)

`pwd` adalah perintah untuk menampilkan atau mengecek posisi direktori sekarang.

- Cek posisi direktori sekarang: `pwd`.
- Melihat isi direktori: `ls -l`.
- Pindah ke direktori Desktop: `cd Desktop`.
- Cek posisi direktori sekarang: `pwd`.

**3. cd: change directory**

![cd](img/cd.jpg)

`cd` adalah perintah untuk berpindah direktori.

**Path Absolute**: Path yang dimulai dari root (/)

**Path Relative**:  Path yang dimulai dari posisi terakhir (current direktori).

**Path Absolute**

- Cek posisi sekarang: `pwd`.
- Pindah ke Direktori Desktop: `cd /home/aufa18/Desktop`.
- Cek posisi sekarang: `pwd`.
- Pindah ke Direktori Documents: `cd /home/aufa18/Documents`.
- Cek posisi sekarang: `pwd`.

**Path Relative**

- Cek posisi sekarang: `pwd`.
- Lihat isi direktori: `ls -l`.
- Pindah ke Direktori Desktop: `cd Desktop`.
- cek posisi sekarang: `pwd`.
- Pindah ke Direktori Documents: `cd ../Documents`.
- Pindah ke Direktori sebelumnya (1 kali): `cd ../`.
- Pindah ke Direktori sebelumnya (2 kali): `cd ../../`.

**Note**

Perintah `cd` akan langsung diarahkan ke direktori home user (/home/namauser).

Ketika membuka terminal, maka posisi user langsung diarahkan ke direktori home user (/home/namauser).

**4. mkdir: make directory**

![mkdir](img/mkdir.jpg)

`mkdir` adalah perintah untuk membuat direktori.

- Cek posisi sekarang: `pwd`.
- Lihat isi direktori: `ls -l`.
- Pindah ke direktori Desktop (path relative): `cd Desktop`.
- Buat folder HTML: `mkdir HTML`.

Selesai.

## Operasi File dan Direktori

**1. cp: copy**

![cp](img/cp.jpg)

`cp` adalah perintah untuk mengcopy file atau direktori.

- Membuat file index.html: `touch index.html`.
- Membuat folder HTML: `mkdir HTML`.
- Melihat isi direktori: `ls -l`.
- Mencogpy file index.html: `cp index.html contact.html`.
- Mengcopy folder HTML: `cp HTML HTML-BACKUP`.

**2. mv: move / rename**

![mv](img/mv.jpg)

`mv` adalah perintah untuk memindahkan atau mengganti nama file atau direktori.

- Melihat isi direktori: `ls -l`.
- mengganti nama file index.html: `mv index.html app.html`.
- Melihat isi direktori: `ls -l`.
- memindahkan file app.html ke folder HTML: `mv app.html HTML`.
- Melihat isi direktori HTML: `ls -l HTML`.
- Mengganti nama folder HTML: `mv HTML PUBLIC`.

**3. rm: remove**

![rm](img/rm.jpg)

`rm` adalah perintah untuk menghapus file atau direktori.

- Membuat file footer.html: `touch footer.html`.
- Menghapus file footer.html: `rm footer.html`.
- Melihat isi direktori PUBLIC: `ls -l PUBLIC`.
- Menghapus direktori PUBLIC (rmdir): `rmdir PUBLIC`.
- Menghapus direktori PUBLIC: `rm -r PUBLIC`.
- Melihat isi direktori: `ls -l`.

## Challenge

![tree](img/tree.png)

1. Buat struktur direktori dan file seperti gambar di atas
   - Buat file index.html.
   - Buat direktori style dan di dalamnya ada file style.css.
   - Buat direktori script dan di dalamnya ada file script.js
   - tampilkan struktur di atas dengan perintah `tree`.
2. Pindah direktori
   - Cek posisi sekarang.
   - Pindah ke direktori style (relatif).
   - Cek posisi sekarang.
   - Pindah ke direktori script (relatif).
3. Memindahkan file
   - Buat file icon.css
   - Pindahkan file icon.css ke folder style.
4. Menghapus file dan folder
   - Hapus file icon.css yang di dalam folder style.
   - Hapus folder script.
5. Apa evaluasi praktikum empat? apa masukan dan saran?

