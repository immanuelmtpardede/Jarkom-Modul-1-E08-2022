# Jarkom-Modul-1-E08-2022
Laporan Resmi Praktikum I Jaringan Komputer oleh Kelompok E08

### Kelompok E08

| **No** | **Nama** | **NRP** |
| - | - | - |
| 1. | Immanuel Maruli Tua Pardede | 5025201166 |
| 2. | Muhammad Ismail | 5025201223 |
| 3. | Halyusa Ard Wahyudi | 5025201088 |

## No. 1
### Soal
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!
### Jawaban
## No. 2
### Soal
Ishaq sedang bingung mencari topik TA untuk semester ini, lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id”, judul TA apa yang dibuka oleh ishaq?
### Jawaban
## No. 3
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!
### Jawaban
## No. 4
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
### Jawaban
## No. 5
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
### Jawaban
## No. 6
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id!
### Jawaban
## No. 7
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari IP kalian!
### Jawaban
Untuk soal 8-10, silahkan baca cerita di bawah ini!

Di sebuah planet bernama Viltrumite, terdapat Kementerian Komunikasi dan Informatika yang baru saja menetapkan kebijakan baru. Dalam kebijakan baru tersebut, pemerintah dapat mengakses data pribadi masyarakat secara bebas jika memang dibutuhkan, baik dengan maupun tanpa persetujuan pihak yang bersangkutan. Sebagai mahasiswa yang sedang melaksanakan program magang di kementerian tersebut, kalian mendapat tugas berupa penyadapan percakapan mahasiswa yang diduga melakukan tindak kecurangan dalam kegiatan Praktikum Komunikasi Data dan Jaringan Komputer 2022. Selain itu, terdapat sebuah password rahasia (flag) yang diduga merupakan milik sebuah organisasi bawah tanah yang selama ini tidak sejalan dengan pemerintahan Planet Viltrumite. Tunggu apa lagi, segera kerjakan tugas magang tersebut agar kalian bisa mendapatkan pujian serta kenaikan jabatan di kementerian tersebut!
## No. 8
### Soal
Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.
### Jawaban
Hal yang pertama kali dilakukan adalah membuka file resource soal8-10.pcapng yang sudah didownload. Kemudian, pada Wireshark, dilakukan penelusuran percakapan sesuai yang diminta pada soal dengan cara klik kanan pada paket yang berada di baris no. 1 dan memilih **Follow** ke **TCP Stream** seperti yang ditunjukkan oleh gambar di bawah.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.1.png" width=50%>

Setelah itu, akan muncul jendela Follow TCP Stream. Pada jendela tersebut, di bagian kanan bawah, terdapat input stream yang nilainya bisa kita ubah menggunakan tombol panah atas dan bawah yang tersedia.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.2.png" width=50%>

Dengan mengeklik tombol panah atas tersebut terus-menerus sambil mengamati data yang ditampilkan di situ, kita mendapatkan percakapan yang kita cari. Terdapat 3 percakapan dan 2 link.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.3.png" width=30%><img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.4.png" width=30%><img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.5.png" width=30%><img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.6.png" width=30%><img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/8.7.png" width=30%>

## No. 9
### Soal
Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama “flag.txt”.
### Jawaban
Berdasarkan transkrip percakapan yang pertama, kita tahu bahwa file yang dimaksud berada pada port 9002. Oleh karena itu, pada Wireshark, di kolom display filter, kita tulis perintah `tcp.port == 9002` untuk menampilkan semua paket dengan protokol TCP yang menuju ke atau berasal dari port 9002. Setelah itu, klik kanan pada paket yang berada di baris no. 1 dan memilih **Follow** ke **TCP Stream** seperti yang ditunjukkan oleh gambar di bawah.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/9.1.png" width=50%>

Setelah itu, di kolom **show data as**, dipilih **Raw**.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/9.2.png" width=50%>

Kemudian, data tersebut di-save as dengan nama E08.des3.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/9.3.png" width=100%>

**Kendala:** Pada pengerjaan di hari-H praktikum, kami tidak mengubah **show datas as** menjadi **Raw**. Kami membiarkan **show data as** tetap **ASCII**. Hal ini membuat kami tidak mendapatkan hasil yang benar pada pengerjaan soal berikutnya.

## No. 10
### Soal
Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!
### Jawaban
