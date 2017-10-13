# TCT01
Apa itu Git
	Git adalah version control system yang digunakan para developer untuk mengembangkan software secara bersama-bersama.Git itu sebuah software, bukanlah sebuah 	bahasa seperti halnya HTML,CSS atau Js bukan pula sebuah konsep atau aturan baku dalam pemrograman.
Instalasi
	Git dapat berjalan dikomputer anda dengan menginstallnya terlebih dahulu. Anda dapat mendownload installer Git di situs http://git-scm.com/

Persiapan
  1. Buat repositori baru
     buat lah direktori baru, buka dan jalankan
	git init
     untuk membuat repositori git baru.
  2. Periksa repositori
     buat lah salinan kerja dari repositori lokal dengan menjalankan perintah
               git clone /jalur/ke/repositori
     saat menggunakan server jarak-jauh, perintahnya menjadi
               git clone namapengguna@host:/jalur/ke/repositori
   3. Alur Kerja
      repositori lokal kamu terdiri dari tiga bagian pokok yang disebut "trees" dikelola oleh git. yang pertama adalah Direktori Kerja yang menyimpan berkas aktual. 	kedua adalah Indeks yang berperan sebagai pengolah data dan terakhir HEAD yang mengarah pada komit terakhir. 
   4. Tambah & Komit
      kamu bisa melakukan perubahan (penambahan ke Indeks) menggunakan
                  git add <namaberkas>
                  git add *
      Ini merupakan langkah awal alur-kerja dasar git. Untuk komit sepenuhnya gunakan
                  git commit -m "Pesan komit"
      Sekarang berkas telah berkomit di HEAD, tapi belum di repositori jarak-jauh.
   5. Mengirim Perubahan
      Saat ini perubahan telah tersimpan di HEAD salinan kerja lokal kamu. Untuk mengirimkannya ke repositori jarak-jauh, lakukan
                   git push origin master
      Ubah master sesuai cabang yang kamu inginkan.
      Jika repositori yang ada belum dikloning dan ingin dihubungkan ke server jarak-jauh, kamu perlu menambahkan
                    git remote add origin <server>
      Sekarang kamu bisa mengirimkan perubahan ke server jarak-jauh yang dituju.
   6. Perbaru & Gabung
       untuk memperbarui repositori lokal ke komit terkini, lakukan
                    git pull
      dari direktori kerja kamu untuk mengambil dan menggabungkan perubahan jarak-jauh.
   7. Menandai
     Sangat dianjurkan membuat penanda atau tags untuk perangkat lunak yang dirilis.Hal ini amat lah lazim, yang juga terjadi di SVN. Kamu bisa membuat penanda baru 	dengan nama 1.0.0 dengan menjalankan
                    git tag 1.0.0 1b2e1d63ff
     1b2e1d63ff adalah 10 karakter pertama dari identitas komit yang ingin kamu referensikan ke penanda. Kamu bisa mendapatkan identitas komit dengan melihat... 
    8. Log
      dalam bentuknya yang paling sederhana, kamu bisa mempelajari riwayat repositori menggunakan.. 
                    git log
      kamu bisa menambahkan banyak parameter untuk menampilkan log sesuai keinginan. Untuk melihat komit penulis tertentu:
                     git log --author=bob


