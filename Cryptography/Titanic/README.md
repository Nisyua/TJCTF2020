# Titanic

## Deskripsi
I wrapped tjctf{} around the lowercase version of a word said in the 1997 film "Titanic" and created an MD5 hash of it: 
```
9326ea0931baf5786cde7f280f965ebb.
```


## Flag
```
tjctf{marlbrough's}
```


## Solusi

1. Download script eng subtittle Film Titanic 1997 pada [yts-subs](https://yts-subs.com/subtitles/titanic-english-yify-100199) .
2. Convert subtittle dari srt menjadi text memakai [converter](https://toolslick.com/conversion/subtitle/srt-to-txt).
3. Buka notepad++, replace semua special characters kecuali `'` (tanda petik satu). Selain itu *replace* spasi menjadi *enter (\n)* agar dapat menjadi dictionary, lalu tambahkan kata tjctf{} pada sebelum `(^)` dan akhir kata `($)` , jangan lupa untuk `search-mode` diganti ke `regular-expression`
4. terakhir convert semua kata menjadi lowercase. Lalu save.
5. Buka linux, gunakan `hashcat` untuk mem-**bruteforce** tiap kata agar dapat menemukan flagnya. 
6. Buka terminal, format command untuk hashcat `hashcat -m 0 hashfile.txt message.txt`. hashfile.txt berisi kunci hash, message.txt adalah dictionary nya.

![](https://github.com/nissyua/TJCTF2020/blob/master/Cryptography/Titanic/flag.png)
