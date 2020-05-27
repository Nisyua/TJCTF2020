# Zipped Up

## Deskripsi
My friend changed the password of his Minecraft account that I was using so that I would stop being so addicted. Now he wants me to work for the password and sent me this zip file. I tried unzipping the folder, but it just led to another [zipped file](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Zipped%20Up/0(2).zip). Can you find me the password so I can play Minecraft again?

## Flag
```
tjctf{}
```

## Solusi
Unzip file 0(2).zip , lalu buka terminal. Jalankan script tarautounzip.py , setelah itu semua folder akan terunzip.
![](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Zipped%20Up/unzip.png)
untuk mengetahui file pada folder berapa flag tersebut berada, kita dapat menggunakan command 
```
cat */*.txt
```
dan hasilnya seperti berikut
![](https://github.com/nissyua/TJCTF2020/blob/master/Miscellaneous/Zipped%20Up/flag.png)
