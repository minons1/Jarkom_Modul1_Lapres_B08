# Lapres Modul 1 Jarkom - Kelompok B08

Dimas Adhitya 05111840000015

Salim Bin Usman 05111840000104

1. Sebutkan webserver yang digunakan pada "testing.mekanis.me"!

Jawab :

`http contains testing.mekanis.me`
![Screenshot_3](https://user-images.githubusercontent.com/55347970/96372061-52147500-118f-11eb-9ed4-90ec9c88793c.png)


webserver nya ialah : nginx/1.14.0 (Ubuntu)
![alt text](https://lh5.googleusercontent.com/WF7IQ9Hp1XwkcWEGv17HtVkvUrBGgA9MHIq1gvhkDCGrqcFx6fJtVXDoOsK27KmUuvCwRzwIeW6Lve4mGlHpjT9EEA6G-B_xDI0bFzgWrk_0aOSiMniHjYXnki8L5QsVKc1AkHqF)

2. Simpan gambar "Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg"!

Jawab :

Proses download :

Pilih menu export -> http, kemudian masukkan nama file gambar :
![alt text](https://lh6.googleusercontent.com/EG8xxNKouAFOrfQggbVJ4T3VG4fD3KTLp5vh2JHTCDazuLPJ_KEIrr0-mVp9ADUyCi3fse2_QKUX8RLQafW_U8ip5EdkZiYaVqED5gjYcz5qspBXagmMYRRQCoRkKocHaDtfOcoV)

Foto yang didapat :
![alt text](https://lh4.googleusercontent.com/IJKz8_GQ1ev1OFzzICFb07xCpphEWkhCN4MFkzHGDPDp__QqLjXxK2_JHykzMStSbqGVl6zMZGLhabDEOI0LJNIt7t1vwRIagPM52N1eQuwIyHPre6USxNrOugqjmJ2A57W1snj-)

3. Cari username dan password ketika login di "ppid.dpr.go.id"!

Jawab :

Display filter : http.request.uri contains “login”
![alt text](https://lh6.googleusercontent.com/yjBDhaP246r1pANhVmb8EfPjK4CAa9nhhxYlX5MGi_1Fzs2tN_RAS5G_F7lvz_OYfSz61xVLltRlbouFmKM-qg1-7kghIWZp0z0DNv_AVPl5EShPTKy5uOKLYYpWwq8pOPQOaSsp)

Method POST akan menyimpan username dan password yang akan dikirim ke server.

4. Temukan paket dari web-web yang menggunakan basic authentication method!

Jawab :

Display filter : tcp.contains.authentication
![alt text](https://lh3.googleusercontent.com/X6IEB8NVOIRKn3QMdDcJzhorZ8trIfFlCyPm0NlKhC8QuA50Hx2aXHeLFepHwCxNsYb2e8DBMrfqonveUSdNfxiHqx0X2TufIbVxWxdzIBI6bJXSTGeJoTXJqaAzSbs_tBUTlnE3)

5. Ikuti perintah di aku.pengen.pw! Username dan password bisa didapatkan dari file .pcapng!

Jawab :

Pencarian username dan password :
![alt text](https://lh3.googleusercontent.com/IKrdpO08MA-rMz2WsbW97BQAw715wl-UxlXxgv4BYmkwx2_MCVsmLrG1rUO784CtltDOX6LtoOpaIKu0hM_MXV24SEssqcfrlYJm_lX0ZewwyXSrYLHDH458ERw2lVs_etPb3z6n)

	username : kakakgamtenk
  
	pass	: hartatahtabermuda
  
Kemudian hasil dari aku.pengen.pw :	
![alt text](https://lh3.googleusercontent.com/OptqxZPAEtME1ArB91px30QKfS3zJlh113SCTltM8H_k8dYtYDQJyVCp___6AHjSaHAHgQDtBYPKV13wFD7NwXmeBbuVH1Uus3h7tiSRGHEnZpzpUl9e2uFfV5eJednmCNNbIh2d)

6. Seseorang menyimpan file zip melalui FTP dengan nama "Answer.zip". Simpan dan Buka file "Open This.pdf" di Answer.zip. Untuk mendapatkan password zipnya, temukan dalam file zipkey.txt (passwordnya adalah isi dari file txt tersebut).

Jawab :

Untuk mencari answer.zip, digunakan display filter : tcp contains .pdf, kemudian follow tcp stream yang mengandung perindah STOR Answer.zip :
![alt text](https://lh6.googleusercontent.com/8B4wbqnAKcYIsHa1OOmz8SWf5o4hwXiAjeoRNFRz0kuXUSkN9kn4UlG4XUT3l5EzQ7i2NPI0YFj6yUh-pPtGX-k243mHgswuSJv78Pj_YX4cuuHpQ_VrCZZYhjkOUnexBnHjr_cw)

Untuk file zipkey.txt, digunakan Display capture : ftp-data
![alt text](https://lh5.googleusercontent.com/PWlnaMlSoK3pWVNZcEiVknkvFk2J3KH9lxCtZT5z81Ssz57XAlsK_EzrWTE8oZqNbzhYgBZWx3vw6n2yK4OIs5haXdk6xxd-NPFwB5xj-dXKaq8zD3I8Unh74bR086UPXlhdXxQh)

password : hey997400323051

![alt_text](https://lh4.googleusercontent.com/VvyukJjKt_LE3fMWhE_uX4sZjDKw57Wb6h6uVkgeop9l2kBdD1njzt9odNuB7e5OtX80vRyplh13Yo8Ml2MmvSKa-r83-jNbBFlmZsLTl_0Lc0hyQs45qBJ57pFZMQk-LpKcWeBz)

7. Ada 500 file zip yang disimpan ke FTP Server dengan nama 1.zip, 2.zip, ..., 500.zip. Salah satunya berisi pdf yang berisi puisi. Simpan dan Buka file pdf tersebut.
Your Super Mega Ultra Rare Hint = nama pdf-nya "Yes.pdf".

Jawab :

Display filter : ftp contains “Yes.pdf”
![alt text](https://lh6.googleusercontent.com/z_yVZa9lIkk9MStiKxszs3NrT_LbdGQBkF2AcXmAlxNmnYU8w0Tac37W0BXYeaECcOBAm1iQqVIDFkVxiB7L9B3xhvbze3WZgnODbFFSdaXD-KgZoTtm07CoFN4g3VfUABaK2GGn)

Kemudian didapatkan 473.zip, lalu follow Tcp stream dan kemudian download file zip tersebut.
![alt text](https://lh3.googleusercontent.com/GXTqrEfNTDCUhvnBDxyE1hKXiKQzHiMnaZ6icjRtIQPQhKN7pGTv0S4KxEkSPbzjIZimCI0yF_VpPBmw1ZHU8ukKbjZkaqFxxV0Qwn_5hJ-OS6Qzw9XEQToxr_SSW9Q-9wh9zy0g)

Hasil pada yes.pdf :
![alt text](https://lh5.googleusercontent.com/Fd7bzq8A3O5AktNwcqCnuMANlPnquHUI26PAZWwLP34LHZ94HGWekSvdbKNttNrYI2EotoZdJk9dIWF4A1PUCmlYgGYXVlfwVF7gGDrGq4oNVAaGD3QEW_Cqv9HtsocsQd4FGv5e)

8. Cari objek apa saja yang didownload (RETR) dari koneksi FTP dengan Microsoft FTP Service!

Jawab :

Display filter : ftp contains RETR

![alt text](https://lh6.googleusercontent.com/CpT0pm7bGrITNTMX6I-h5Ug6X7uzJYLqVD2W3aTlfltCNICNrFLXGwr4Mc_90wdOHqaPegkCh1mkLqpep6jIbXHuL5HzfyuRJGNJdEz3guPbw8CuOzADbp_oSJUHl8fA6lxTbZlD)

File Readme dan licence.txt

9. Cari username dan password ketika login FTP pada localhost!

Jawab :

Display filter : ftp contains "USER" || ftp contains "PASS"
![alt text](https://lh4.googleusercontent.com/KsakNKyphcAsK31hWok8r5SmG7OWRMf7FKu--ZIQBkmE42kR0pJgZOv_Em0TadUvdGzqNe-Yh1G8n8nEofwgJeGaLnUAXAET8s_uziFL7FCKXFuPdXOUZMIBuCvm4PJCmqu6yt2H)

user : dhana

pass : dhana123

10. Cari file .pdf di wireshark lalu download dan buka file tersebut!
clue: "25 50 44 46" 

Jawab :

Diketahui jika angka “25 50 44 46” diubah menjadi text, menghasilkan text “%pdf”. Sehingga jika kita mengubah pencarian berdasarkan Hex value, kemudian masukkan “25 50 44 46” akan menghasilkan :
![alt text](https://lh6.googleusercontent.com/ODIQiemUK-HtnBOXSRqd1gwAbhjeZEjq6B4FfsTm7weZZGPXL0PYBsoawvyS21fPAHqkNFwwZso5X1_Q4UhrOUkDYF1qsyi9Onkoy5QxSNtIUmoy0DTA2vCuAEit6HK-7BpUlIsd)

Kemudian follow tcp stream paket tersebut, dan ubah ‘show and save data as’ menjadi raw. Dan save as sebagai file pdf
![alt text](https://lh4.googleusercontent.com/36_6JA-9vpGAng00WOLM2SErVc9YtTOO68Va_jyaGVag8AEeAMfOtQgF8kSi5ItpyH4pnOUuWDbUK3F8LZ5JWboV6XA5tJlSGhq5fpFGfdNMweSu2EI70XzmxJ7GrxxVLDrA5M-R)

File hasil :
![alt text](https://lh6.googleusercontent.com/C1P17yJtKFxBhNpnMI7fuWXe_vcTTlODEWTP9ZYeGaFFzI2-90V4Ld3BCfsMG-wm6PovAfdBsOs0WS6G1-rFZ8aBz0jEy5Xn8UWcFZW30_ODh33oTQcPx54ayWx_9lSi-XCl9guH)

11. Filter sehingga wireshark hanya mengambil paket yang mengandung port 21!

Jawab :

Capture filter: port 21
![alt text](https://lh6.googleusercontent.com/UvszcJh0KtsipYGCPL26l7Qmgy5Kr8tASZZthgTi4HeftUbKDzu8ca_EUHCag2hVJOc1E4_yxcKuwBJgMqfxdZmj8Eh62w-6SPwugpdBxBzLtHCMeLMIRydMyPgrw7F0hNPXcg5x)

12. Filter sehingga wireshark hanya mengambil paket yang berasal dari port 80!

Jawab :

Capture filter: src port 80
![alt text](https://lh3.googleusercontent.com/4eSZFPGGmVzuj9khwWjXBcD4MOL9S__G8LIYaGevBJ1NXZCy7adw43FU1r40duZQU-Hls0wPu5x6MoZae7IBopvV_YSZxXzurPteePnqvFVky6S9joL1GLPAEG7qHDEXUhmdMnLs)

13. Filter sehingga wireshark hanya menampilkan paket yang menuju port 443!

Jawab :

Capture filter: dst port 443
![alt text](https://lh3.googleusercontent.com/45aSnanFsjE4HpSUQg-8d71qaA_pRtJ_4Jv3lGvXddtgmnbO78Nz50J3E3ozP8ejD3G39GlSkLRJncHAEd4zdpxkb7VaeUCvG_Ejk_65MZFnomFzmIJKt8Tv8vgjS3Fi-xEPxmsL)

14. Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

Jawab :

Capture filter: src host 192.168.43.225
![alt text](https://lh4.googleusercontent.com/IgHBldJgreMJL12yIcHoSD6I2XOaVqB9GbxQylBYK7ktzPUEDtZi1uXpLJJ76lb6zMHbexOMqe6NFe_kEusoIcjt_Zy8h2q08GmIG4AbEf0KVARVxzg7s4hIsvmo4WyZZr1GChFA)

15. Filter sehingga wireshark hanya mengambil paket yang tujuannya ke monta.if.its.ac.id!

Jawab :

Capture filter: dst host 103.94.190.11
![alt text](https://lh6.googleusercontent.com/KOW7KFa4NeLagfMeDsboWywBdgXCEA5NeAbBQd7RxGev6gZ6z1ra1KUiKK3eLVJDyILZViQdPFc1QoTjvPp5trVYNchpSctH7obm_BZaHmAzAp2B9WtSG2-ERT_OeWsjcZVeEnOx)

