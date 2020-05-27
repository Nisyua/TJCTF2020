# Titanic

## Deskripsi
I wrapped tjctf{} around the lowercase version of a word said in the 1997 film "Titanic" and created an MD5 hash of it: 9326ea0931baf5786cde7f280f965ebb.


## Flag
```
tjctf{marlbrough's}
```


## Solusi
pertama, download script eng subtittle Film Titanic 1997 pada [link](https://yts-subs.com/subtitles/titanic-english-yify-100199 . lalu convert subtittle dari srt menjadi text memakai https://toolslick.com/conversion/subtitle/srt-to-txt). setelah itu Buka notepad, replace semua special characters kecuali ' (tanda petik satu), replace spasi menjadi enter (\n) , lalu tambahkan kata tjctf{} pada sebelum dan akhir kata, terakhir convert semua kata menjadi lowercase. Buka linux, gunakan `hashcat` untuk mem-**bruteforce** tiap kata agar dapat menemukan flagnya. format command untuk hashcat `hashcat -m 0 hashfile.txt message.txt`. hashfile.txt berisi kunci hash, message.txt adalah dictionary nya.

![](https://github.com/nissyua/TJCTF2020/blob/master/Cryptography/Titanic/flag.png)
