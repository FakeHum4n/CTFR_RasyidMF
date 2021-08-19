# First_Flag
#cryptography #First_flag #ctfr #rasyidmf #LAY0ut_team

Pada soal ini kita disuguhkan sekumpulan angka sebagai berikut :
```
72721798973508317998010221759715603442488699336903823695032175490877440550933707738215915097249162010936760632656546551213097571155720293246858222618614687119941380089920829
```
Dengan hint: 

> Semua Challenge ada Hint yang akan membantu kalian untuk menyelesaikan challenge, dan pastinya Hint harus dibayar menggunakan point skor kalian. Dan untuk First Flag ini gratis, Kalian hanya konversi angka tersebut menjadi _deadbeef_, Kemudian hasil nya di konversi lagi dan lagi sampai mendapatkan flag! Easy kok.

Maka dari itu, hal pertama yang Saya lakukan adalah melakukan konversi nilai dari desimal ke deadbeef:
![2021-08-18 14_51_56-Window](https://user-images.githubusercontent.com/46299092/129859760-6ec8e984-c5bd-4305-86ac-b264de6edd42.png)


link : [deadbeef base converter](https://deadbeef.app/)

Sehingga didapatlah nilai hex:
```
4b455956455232564e5a324441594b45495a354651365347504a4d44473344574d524d45555a53324e4a444853595a544b4a544655334c5847424e44474d434c42493d3d3d3d3d3d
```

Yang mana jika nilai hex ini dikonvesikan menjadi ASCII, maka didapatlah sebuah string dalam format Base32:
```
KEYVER2VNZ2DAYKEIZ5FQ6SGPJMDG3DWMRMEUZS2NJDHSYZTKJTFU3LXGBNDGMCLBI======
```

Setelah string ini didecode, maka didapatlah string dalam bentuk Base64:
```
Q1RGUnt0aDFzXzFzX3lvdXJfZjFyc3RfZmw0Z30K
```

Lalu, Saya lakukan decode lagi dan diapatlah flagnya
![2021-08-18 14_40_15-Window](https://user-images.githubusercontent.com/46299092/129859577-a89158ed-785b-4ccc-b659-d76f18216165.png)
link : https://gchq.github.io/CyberChef/
