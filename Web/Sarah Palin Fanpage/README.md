# Sarah Palin Fanpage

## Deskripsi
Are you a true fan of Alaska's most famous governor? Visit the [Sarah Palin fanpage](https://sarah_palin_fanpage.tjctf.org/).

## Flag
```
tjctf{wkDd2Pi4rxiRaM5lOcLo979rru8MFqVHKdTqPBm4k3iQd8n0sWbBkOfuq9vDTGN9suZgYlH3jq6QTp3tG3EYapzsTHL7ycqRTP5Qf6rQSB33DcQaaqwQhpbuqPBm4k3iQd8n0sWbBkOf}
```

## Solusi
Pertama, klik menu VIP area pada web tersebut. Lalu buka cookie dari website tersebu dengan cara inspect element. Value dari cookie tersebut merupakan hasil encode dengan metode Base64. Lalu, copy semua value dari cookie tersebut. Penulis akan melakukan decode dengan bantuan [Base64 Encode and Decode](https://www.base64decode.org/). Hasil decode tampak seperti ini : 
`{"1":false,"2":false,"3":false,"4":false,"5":false,"6":false,"7":false,"8":false,"9":false,"10":false}` . Kemudian, ubah kata `false` menjadi `true` dan lakukan encode kembali dengan base64. Dan, masukkan kembali ke value pada data cookie dan refresh page.
Flag akan langsung muncul pada halaman web tersebut.
