* Nama : M. Rafif Farihan
* Nim  : 09011282328042
* kelas: SK3C
  
# Tugas 6 Praktikum Sistem Operasi

## 1. Eksekusi seluruh profile yang ada

### a. Edit file profile /etc/profile dan tampilkan pesan sebagai berikut:

```bash
echo "Profile dari /etc/profile"
```

![1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1.png)
![1-a](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-a.png)
![1-a1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-a1.png)

### b. Asumsi nama anda stD02001, maka edit semua profile yang ada yaitu:

- /home/stD02001/.bash_profile
![1-b1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-b1.png)

- /home/.stD02001/.bash_login
![1-b2](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-b2.png)

- /home/mahasiswa/.profile
![1-b3](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-b3.png)

- /home/mahasiswa/.bashrc
![1-b3](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-b3.png)

<div align="justify">
Ganti nama /home/mahasiswa dengan nama anda sendiri. Pada setiap file tersebut, cantumkan instruksi echo, misalnya pada /home/mahasiswa/.bash_profile : echo "Profile dari .bash_profile" Lakukan hal yang sama untuk file lainnya, sesuaikan tampilan dengan nama file yang bersangkutan.
</div>

- Memeriksa apakah instruksi yang sudah dibuat sebelumnya sudah ada apa belum
![1-b5](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-b5.png)

### c. Jalankan instruksi subtitute user, kemudian keluar dengan perintah exit sebagai berikut:

```bash
$ su mahasiswa
$ exit
```

Kemudian gunakan opsi – sebagai berikut:

```bash
$ su – mahasiswa
$ exit
```

Jelaskan perbedaan kedua utilitas tersebut.
![1-c](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/1-c.png)

<div align="justify">
Perbedaan antara perintah su mahasiswa dan su - mahasiswa terletak pada pengelolaan lingkungan shell. Perintah su mahasiswa hanya mengganti pengguna aktif menjadi mahasiswa tanpa mengubah lingkungan shell, sehingga variabel lingkungan tetap mengikuti konfigurasi pengguna sebelumnya. Sedangkan, su - mahasiswa tidak hanya mengganti pengguna aktif menjadi mahasiswa, tetapi juga memuat ulang seluruh lingkungan shell pengguna tersebut, termasuk variabel dan pengaturan lingkungan yang ada di profil pengguna mahasiswa. Opsi - memastikan bahwa Anda bekerja dengan konfigurasi penuh dari pengguna baru.
</div>

## 2. Prompt String (PS)

### a. Edit file .bash_profile, ganti prompt PS1 dengan '>'. Instruksi export diperlukan dengan parameter nama variable tersebut, agar perubahan variable PS1 dikenal oleh semua shell

```bash
PS1='> '
export PS1
```

![2-a](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/2-a.png)

### b. Eksperimen hasil PS1:

```bash
$ PS1="\! > "
69 > PS1="\d > "
Mon Sep 23 > PS1="\t > "
10:10:20 > PS1="Saya=\u > "
Saya=mahasiswa > PS1="\w >"
~ > PS1=\h >"
```

![2-b](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/2-b.png)

## 3. Logout

Edit file .bash_logout, tampilkan pesan dan tahan selama 5 detik, sebelum eksekusi logout

```bash
Echo "Terima kasih atas sesi yang diberikan"
Sleep 5
clear
```

![3](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/3.png)
![3-a](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/3-a.png)

## 4. Bash script

### a. Buat 3 buah script p1.sh, p2.sh, p3.sh dengan isi masing-masing:

p1.sh
```bash
#!/bin/bash
echo "Program p1"
ls -l
```
![4-a](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-a.png)

p2.sh
```bash
#!/bin/bash
echo "Program p2"
who
```
![4-a2](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-a2.png)

p3.sh
```bash
#!/bin/bash
echo "Program p3"
ps x
```
![4-a3](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-a3.png)

### b. Jalankan script tersebut sebagai berikut:

```bash
$ ./p1.sh ; ./p3.sh ; ./p2.sh
```
![4-b1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b1.png)
![4-b2](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b2.png)
![4-b3](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b3.png)
![4-b4](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b4.png)

```bash
$ ./p1.sh &
```
![4-b5](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b5.png)

```bash
$ ./p1.sh $ ./p2.sh & ./p3.sh &
```
![4-b6](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b6.png)
![4-b7](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b7.png)
![4-b8](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b8.png)

```bash
$ ( ./p1.sh ; ./p3.sh ) &
```
![4-b9](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/4-b9.png)

## 5. Jobs

### a. Buat shell-script yang melakukan loop dengan nama pwaktu.sh, setiap 10 detik, kemudian menyimpan tanggal dan jam pada file hasil.

```bash
#!/bin/bash
while [ true ]
do
    date >> hasil
    sleep 10
done
```
![5-a1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/5-a1.png)

### b. Jalankan sebagai background; kemudian jalankan satu program (utilitas find) di background sebagai berikut:

```bash
$ jobs
$ find / -print > files 2>/dev/null &
$ jobs
```
![5-b](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/5-b.png)

### c. Jadikan program ke 1 sebagai foreground, tekan ^Z dan kembalikan program tersebut ke background

```bash
$ fg %1
$ bg
```
![5-c](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/5-c.png)

### d. Stop program background dengan utilitas kill

```bash
$ ps x
$ kill [Nomor PID]
```
![5-d1](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/5-d1.png)
![5-d2](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/5-d2.png)

## 6. History

### a. Ganti nilai HISTSIZE dari 1000 menjadi 20

```bash
$ HISTSIZE=20
$ h
```
![6-a](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/6-a.png)

### b. Gunakan fasilitas history dengan mengedit instruksi baris ke 5 dari instruksi yang terakhir dilakukan

```bash
$ !-5
```
![6-b](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/6-b.png)

### c. Ulangi instruksi yang terakhir. Gunakan juga ^P dan ^N untuk bernavigasi pada history bufer

```bash
$ !!
```
![6-c](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/6-c.png)

### d. Ulangi instruksi pada history bufer nomor 150

```bash
$ !150
```
![6-d](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/6-d.png)

### e. Ulangi instruksi dengan prefix "ls"

```bash
$ !ls
```
![6-e](https://github.com/Rafiffarihan13/M.-Rafif-Farihan_09011282328042_SK3C_Tugas-6-praktikum-sistem-operasi/blob/main/Gambar/6-e.png)


