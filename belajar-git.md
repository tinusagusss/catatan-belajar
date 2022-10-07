# Version Control System
VCS sangat populor dikalangan programmer dikarenakan sangat dapat membantu mereka untuk mengelola perubahan kode program. Namun, VCS tentu juga dapat digunakan oleh siapapun untuk mengelola file apapun, seperti mahasiswa ketika menyusun skripsi.

# Tipe Version Control
## 1. Local Version Control 
Hanya berjalan di satu komputer saja. itu artinya ketika komputer mengalaman kerusakan, rekaman yang telah dibuat tentu akan hilang.

## 2. Centralize Version Control
Perubahan akhir yang dibuat akan disimpan di sebuah server, dengan demikian pengguna juga dapat membagikan ataupun berkerja secara kolaboratif namun harus terkoneksi dengan internet/jaringan. 

## 3. Distributed Version Control
Seluruh riwayat perubahan disimpan kedalam server (menyalin seluruh riwayat). Contoh: Git

# Git
Git pertama kali diperkanalkan di tahun 2005 dan populer hingga sekarang.

Git merupakan salah satu DVCs, namun dapat juga menjadi Local Version Control apabila tidak membutuhkan server.

Git Menggunakan algoritma hashing SHA-1

Dalam Git, sebuah project baru disebut repository

## Configuration
```
git config --global user.name “git username”
git config --global user.email “git email”
```

## Repository
Untuk membuat sebuah repository kita dalam menggunakan perintah git ini, dan kemudian membuka project tersebut dengan code . apabila menggunakan Visual Studio Code

```
git init

code .
```

## Workflow
Git memiliki tiga state
1. Modified: Melakukan perubahan didalam repository
2. Staged: Menandai modifikasi yang telah yakin dan akan disimpan ke repository
3. Committed: Perubahan telah disimpin di repository

Git juga memiliki tiga section
1. Working Directory: Pengelolaan file didalam repository
2. Staging Index/Area: File siap untuk disimpan
3. Repository: File dan riwayat versi disimpan

## Basic

```
git status 

```
Perintah ini digunakan untuk memeriksa perubahan(Snapshot) apa saja yang telah terjadi di Working Index
```
git add
```
Perintah ini digunakan untuk 
```
git commit
```
Perintah ini digunakan untuk memindahkan file(Snapshot) dari Stagging Index ke Repository

Setiap snapshot didalam git diindentifikasikan dengan sebuah HASH(SHA-1)

HEAD merupakan hash paling akhir

## Perintah

###  Membatalkan Perubahan
```
git clean -f
```
Membatalkan segala perubahan yang ada di Working Index

```git
git restore <file>
```
Mengambalikan file yang telah dimodifikasi. Contoh kasus: apabila function yang kita buat salah, kita bisa kembali ke commit akhir untuk menghapus apa yang telah kita buat atau modifikasi.
```
git restore --staged <file>
```
Memindahkan file yang ada di staging index kembali ke working index

### Commit log
Semakin banyak history yang dibuat, semakin banyak atau besar file git-nya.
```
git log
```
digunakan untuk menampilkan riwayat komit yang telah dilakukan.

```
git log --oneline
```
digunakan untuk menyederhanakan tampilan riwayat
```
git log --oneline --graph
```
digunakan untuk menampilkan graph riwayat
```
git show hash <file>
```