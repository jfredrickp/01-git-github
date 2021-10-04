### Tugas 1 MDPL P 

## Langkah-langkah Praktik Git hub

## Instal Git 
1. Sebelum menginstall Git, kita harus memiliki editor teksnya terlebih dahulu. Contoh : Windows disarankan Visual Studio Code atau Notepad++
- Download Git
- Instal Git (ikuti langkah - langkahnya hingga finish)
- Cek instalan
``` 
git --version 
```

## Konfigurasi Git
1. Untuk memberitahukan Git tentang informasi pengguna. Data yang diisikan saat konfigurasi harus sesuai saat didaftarkan di GitHub
``` 
git config --global user.name "jfredrickp" 

git config --global user.email "juanfredrick10@gmail.com 
```

2. Kita dapat cek hasil dan verifikasi perubahan dengan:
``` 
git config --list
```

## Membuat Repo Sendiri 

### Membuat repository 
1. Berikut langkah - langkahnya:
- Klik +, lalu New repository (sebelah kanan tombol notifikasi).
- Isikan Informasi, seperti: nama repo, public atau private reponya, dan lain - lain.
- Klik Create Repository

### Clone repository 
1. Clone disini untuk menduplikasikan file repo di GitHub ke file Lokal komputer
2. Berikut clone repositori tersebut ke komputer lokal 

    ``` 
    $ git clone https://github.com/jfredrickp/01-git-github.git 
    ```

3. Tambahkan .md pada nama folder yang sudah di clone

### Mengelola Repo
### Mengubah isi - push tanpa Branching dan Merging
Perubahan isi bisa terjadi karena satu atau kombinasi berikut:
-  File dihapus
-  File diedit
- Membuat file / direktori baru
- Menghapus direktori
1. Untuk mengetahui status dari repository lokal :
``` 
$ git status 
```
2. Untuk membuat repository yang nantinya file tersebut terdapat .git
``` 
$ git init
```
3. Untuk menambahkan file baru repository
``` 
$ git add namafile.md
```
4. Untuk menyimpan perubahan file
``` 
$ git commit -m 
```
5. Untuk mengirimkan perubahan file setelah di commit ke remote repository
``` 
$ git push -u origin main
```
### Mengubah isi dengan Branching dan Merging
1. Untuk melihat cabang 
``` 
$ git branch
```
Apabila tidak ada maka akan muncul master/main saja
2. Untuk membuat cabang baru
``` 
$ git branch setting
```
3. Untuk pindah kecabang baru
``` 
$ git checkout setting
```
4. Untuk menambahkan file kedalamnya atau sebuah argumen
``` 
$ git add -A
$git commit -m "Add: tugasmdplp.md"
```
5. Untuk menggabungkan cabang dan main
``` 
$ git checkout master
```
6. Untuk berpindah ke main/master dahulu selanjutnya untuk penggabungan 
``` 
$ git merge setting
```

## Sinkronasi
Untuk menyinkronkan repo kita saat sedang mengedit menggunakan komputer lain
``` 
$ git pull
```