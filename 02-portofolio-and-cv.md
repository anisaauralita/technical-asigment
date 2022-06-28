1. Membuat sebuah folder kosong dengan namamu sendiri
>mkdir anisa

2. membuat sebuah file di dalam folder tersebut dengan nama README.md, isi file tersebut dengan kalimat
"Halo perkenalkan aku halaman utama"
>cd anisa
>echo "Halo perkenalkan aku halaman utama" >> README.md

3. inisialisasi folder tersebut dengan Git, kemudian simpan perubahan menggunakan commit dengan pesan
"Inisialisasi GIT Repository"
>git config --global user.name "anisaauralita"
>git config --global user.email "anisaauralita@gmail.com"
>git init .
>git add .
>git commit -m "Inisialisasi GIT Repository"

4. Ganti teks sebelumnya dengan "Hello world"
>echo "Hello world" > README.md
>git add .
>git commit -m "Second commit, hello world"

5. Tampilkan isi teks tersebut pada command line menggunakan command cat
>cat README.md

6. Ternyata kamu tidak ingin perubahan tersebut, dan ingin kembali ke perubahan seperti commit yang terakhir. Lakukan teknik git backtracking untuk mengembalikan ke perubahan commit yang terakhir.
>git reset --hard b2e7d37a90afeddc7a5a378d587da4230bbd11bb

7. buat branch baru dengan nama cv, hal ini berguna agar histori kita tidak tercampur
>git branch cv

8. pindah branch ke dalam cv, kemudian buat file dengan nama cv.txt dan isi file tersebut dengan kalimat:
"Ini adalah file CV"
>git checkout cv
>echo "Ini adalah file CV" >> cv.txt

9. kemudian simpan perubahan menggunakan commit dengan pesan "Initial CV"
>git add .
>git commit -m "Initial CV"


10. tambahkan 3 perusahaan yang akan kamu lamar, dan setiap menuliskan 1 nama perusahaan kamu harus melakukan dokumentasi dan menyimpan perubahan menggunakan commit

>nano cv.txt
>Ctrl + O, ENTER, Ctrl + X
>git add .
>git commit -m "Menambahkan perusahaan pertama"

>nano cv.txt
>Ctrl + O, ENTER, Ctrl + X
>git add .
>git commit -m "Menambahkan perusahaan kedua"

>nano cv.txt
>Ctrl + O, ENTER, Ctrl + X
>git add .
>git commit -m "Menambahkan perusahaan ketiga"

11. kembali ke branch master
>git checkout master

12. ubah file README.md menjadi
"Halo perkenalkan aku halaman utama
Ini adalah update pertama pada branch master"

jangan lupa untuk menyimpan perubahan menggunakan commit dengan pesan
"update master pertama"

>nano README.md
Halo perkenalkan aku halaman utama
Ini adalah update pertama pada branch master
>Ctrl + O, ENTER, Ctrl + X
>git add .
>git commit -m "Update master pertama"

13. gabungkan branch cv ke dalam branch master menggunakan perintah git merge
>git commit -m "Merge branch CV"
>git merge cv

14. Unggah Git Repository project tersebut tersebut ke dalam GitHub
>git remote add github https://github.com/anisaauralita/02-portofolio-and-cv.git
>
>git push github master
