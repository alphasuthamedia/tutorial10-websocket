![websocket photo](resource/Screenshot%20From%202025-05-21%2016-19-00.png)

Sebenarnya ini demonstrasi websocket biasa, serer akan membuka tunnel dan melakukan listening terhadap port yang terbuka itu, dimana nantinya client akan mengirim sebuah request atau data ke alamat dan port yang terbuka tersebut dan client akan mendapatkan response dari server. perlu diingat response ya bisa bisa aja kosong tapi di tutorial kali ini responsenya terisi dengan kiriman pesan dari client yang mengirim sebuah pesan tersebut. jadi client yang hanya listen ke server juga dapat info yang terbaru. bidireksoinal


seperti yang sudah saya katakan tadi, kalau kita salah setup tunning nya (entah itu protokol, alamat, atau port) ya enggak aakan bisa. jadi disini clientnya (tokio) gagal mendapatkan token websocketnya dengan demikian dia langsung return errror. kalau mau ganti port ya servernya juga musti diganti juga portnya dengan port yang sama (dengan client).