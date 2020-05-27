# Censorship

## Deskripsi
My friend has some top-secret government intel. He left a message, but the government censored him! They didn't want the information to be leaked, but can you find out what he was trying to say?
```
nc p1.tjctf.org 8003
```
## Flag

```
tjctf{TH3_1llum1n4ti_I_R3aL}
```

## Solusi

Jalankan wireshark pada Linux. 
Setelah wireshark dijalankan, maka buka terminal baru untuk menjalankan nc p1.tjctf.org 8003. Jawab pertanyaan penjumlahan sederhana yang diberikan. Akan muncul flag tjctf{[CENSORED]}.

![](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Censorship/terminal.png)
![](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Censorship/ws.png)
![](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Censorship/flag.png)
