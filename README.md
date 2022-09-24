# Jarkom-Modul-1-E08-2022
Laporan Resmi Praktikum I Jaringan Komputer oleh Kelompok E08

### Kelompok E08

| **No** | **Nama** | **NRP** | **Kontribusi (No.)** |
| - | - | - | - |
| 1. | Halyusa Ard Wahyudi | 5025201088 | 1, 2, dan 7 |
| 2. | Muhammad Ismail | 5025201223 | 3, 4, 5, dan 6 |
| 3. | Immanuel Maruli Tua Pardede | 5025201166 | 8, 9, dan 10 |

## No. 1
### Soal
Sebutkan web server yang digunakan pada "monta.if.its.ac.id"!
### Jawaban 
1. Pertama, kita harus membuka file pcapng untuk soal nomor 1-2. Lalu setelah terbuka di wireshark, masukkan display filter http.

![Nomor 1 1](https://user-images.githubusercontent.com/100200062/192067109-75a2e81c-5aca-4e95-afb7-00d9b7caa7fc.png)

2. Lalu klik kanan pada internet protocol, pilih follow, dan pilih tcp stream. 

![Nomor 1 2](https://user-images.githubusercontent.com/100200062/192067120-aa8db2ae-2438-4df7-88d5-dcd6809388f4.png)

3. Setelah itu, bisa kita lihat bahwa web server yang digunakan pada website "monta.if.its.ac.id" adalah "nginx".

![Nomor 1 3](https://user-images.githubusercontent.com/100200062/192068036-50a52777-b18f-4d35-92f3-5ab808844168.png)

## No. 2
### Soal
Ishaq sedang bingung mencari topik TA untuk semester ini, lalu ia datang ke website monta dan menemukan detail topik pada website “monta.if.its.ac.id”, judul TA apa yang dibuka oleh ishaq?
### Jawaban
1. Pertama, kita harus membuka file pcapng untuk soal nomor 1-2. Lalu setelah terbuka di wireshark, masukkan display filter http.

![Nomor 2 1](https://user-images.githubusercontent.com/100200062/192066975-a3d5afce-3c90-4402-a8e4-443e19953090.png)

2. Lalu cari **detail topik** sesuai dengan yang diminta oleh soal pada website "monta.if.its.ac.id"

![Nomor 2 2](https://user-images.githubusercontent.com/100200062/192067086-a8ea3b58-da95-46ed-b54b-d05948280650.png)

3. Bisa dilihat bahwa nomor atau nama file dari detail topiknya adalah "194". Untuk melihat judul apa yang ada di dalam file tersebut, maka kita harus mendownload atau export file tersebut. Maka, pilih "Export Object" lalu "HTTP"

![Nomor 2 3](https://user-images.githubusercontent.com/100200062/192067422-72964f67-2897-4945-865f-b954356701bc.png)

4. Setelah itu, pilih file dengan nama "194" sesuai dengan detail topik yang telah dicari sebelumnya, lalu klik save. 

![Nomor 2 4](https://user-images.githubusercontent.com/100200062/192067746-9b7dc0e4-759e-47aa-8ccc-669e82800036.png)

5. Setelah file ter-save, buka file tersebut untuk melihat isinya. 

![Nomor 2 5](https://user-images.githubusercontent.com/100200062/192067784-7fcf8889-8451-429b-aa2a-197ae16a5e5e.png)

6. Maka bisa dilihat, bahwa judul TA yang dilihat Ishaq pada detail topik adalah "Evaluasi untuk Kerja User Space Filesystem(FUSE)"

![Nomor 2 6](https://user-images.githubusercontent.com/100200062/192067845-d9eb4000-0cb3-4bff-bc78-5faa714649ff.png)

## No. 3
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju port 80!
### Jawaban
1. Langkah Pertama yaitu mendownload resource yang ada di drive soal-shift modul 1 (soal 3-6.pcapng)

![Nomor 3 langkah 1][]

2. Langkah Selanjutnya yaitu masuk ke dalam file yang sudah kita download dengan menggunakan wireshark
![Nomor 3 langkah 2][]

3. Langkah terakhir yaitu tulis ke display portnya (***tcp.dstport == 80***) agar menampilkan paket yang ***menuju*** ke port 80

![Nomor 3 langkah 3][]
## No. 4
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 21!
### Jawaban

> Langkah pertama sama kayak soal sebelumnya

> Setelah masuk ke dala wiresharknya, kita tulis ke display portnya (***tcp.srcport == 21***) agar menampilkan paket yang ***berasal*** dari port 21

![Nomor 4][]
## No. 5
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari port 443!
### Jawaban
> Langkah pertama sama kayak soal sebelumnya

> Setelah masuk ke dala wiresharknya, kita tulis ke display portnya (***tcp.srcport == 443***) agar menampilkan paket yang ***berasal*** dari port 443

![Nomor 5][]
## No. 6
### Soal
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id!
### Jawaban
> Langkah pertama sama kayak soal sebelumnya

> Setelah masuk ke dala wiresharknya, kita tulis ke display portnya (***http contains == "lipi.go.id"***) agar menampilkan paket yang ***menuju*** lipi.go.id
![Nomor 6][]

## No. 7
### Soal
Filter sehingga wireshark hanya mengambil paket yang berasal dari IP kalian!
### Jawaban
1. Buka command prompt, lalu ketik "ipconfig" untuk mendapatkan IP Address kita.

![Nomor 7 1](https://user-images.githubusercontent.com/100200062/192068267-164691f2-13d5-40d0-aa60-8b00900e71a3.png)

2. Lalu menggunakan capture filter pada Wireshark, masukkan filter "src host [IP Address]". Maka akan terlihat paket-paket yang ada pada IP kita. 

![Nomor 7 2](https://user-images.githubusercontent.com/100200062/192068320-dd1a58b8-3361-42e3-85c9-0d5b1b1c4608.png)


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
Berdasarkan hint pada transkrip percakapan pertama, file E08.des3 yang sudah dibuat didekripsikan menggunakan OpenSSL dengan metode des3. Lalu, outputnya disimpan dalam file dengan nama flag.txt, sesuai yang diminta pada soal no. 9. Perintah yang digunakan adalah `des3 -d -salt -in "E08.des3" -out "flag.txt"`. Akan ditanya password dekripsinya. Berdasarkan hint pada transkrip percakapan kedua dan ketiga, password yang benar adalah **nakano**, marga dari 5 kembar bersaudara pada "anime 5-toubun no Hanayome".

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/10.1.png" width=100%>

Kita berhasil mendapatkan password rahasianya, yaitu **JaRkOm2022{8uK4N_CtF_k0k_h3h3h3}**.

<img src="https://github.com/immanuelmtpardede/Jarkom-Modul-1-E08-2022/blob/main/img/10.2.png" width=100%>

**Kendala:** Pada pengerjaan di hari-H praktikum, kami tidak mendapatkan jawaban yang benar. Alasannya sudah dijelaskan pada soal no. 9 di bagian Kendala. Namun, cara pengerjaannya sama. Selain itu, kami juga jadi tidak tahu bahwa password yang benar adalah **nakano**. Kami sempat mengira bahwa passwordnya adalah judul dari animenya, **gotoubunnohanayome**.
