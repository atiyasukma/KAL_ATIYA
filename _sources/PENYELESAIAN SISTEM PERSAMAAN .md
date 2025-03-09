---
title: 'PENYELESAIAN SISTEM PERSAMAAN '

---

## PENYELESAIAN SISTEM PERSAMAAN LINEAR
### Operasi Baris Elementer
operasi yang dilakukan pada baris suatu matriks untuk mengubahnya menjadi bentuk yang lebih sederhana. OBE dapat digunakan untuk menyelesaikan sistem persamaan linear (SPL) dan menentukan invers matriks.

*  Tiga operasi dasar dalam OBE adalah:
1.  Row scaling: Mengalikan baris matriks dengan konstanta bukan nol.
Notasi: Ri←kRi, dengan k≠0
2.  Row swapping atau pertukaran dua baris: Menukar urutan baris pada sebuah matriks.
Notasi: Ri↔Rj
3. Row replacement: Mengganti baris matriks dengan hasil penjumlahan atau pengurangan baris matriks tersebut dengan baris matriks lainnya.
Notasi: Ri←Ri+kRj

### Eleminasi Gauss
metode untuk operasi nilai-nilai dalam matriks, untuk membuat matriks lebih sederhana lagi. Metode eliminasi gaus dikembangkan dari metode eliminasi, dengan cara menghilangkan atau mengurangi jumlah variabel, untuk mendapatkan nilai variabel bebas.
liminasi Gauss mengubah persamaan linear menjadi bentuk matriks, kemudian diubah ke bentuk Eselon Baris melalui Operasi Baris Elementer. Setelah itu bentuk matriks diselesaikan dengan substitusi balik. pada eliminasi gauss ini matriks hanya akan tersisa satu variabel saja.
* Langkah-langkah eliminasi Gauss
1. Matriks Augmented
 Gabungkan matriks koefisien dan matriks hasil menjadi satu matriks augmented.

2. Membentuk Segitiga Atas (Eliminasi Maju)
 Gunakan Operasi Baris Elementer (OBE) untuk membuat elemen di bawah diagonal utama menjadi nol.

3. Substitusi Mundur
Setelah terbentuk matriks segitiga atas, gunakan substitusi mundur untuk mendapatkan nilai variabel.

Contoh soal:
Selesaikan dengan menggunakan Eliminasi Gauss.
$$
\begin{array}{cc}
x_1+2x_2+3x_3z&=6\\
2x_1+4_2+6x_12&=4\\
x_3-x_24&=2
\end{array}
$$

### Soal 1
Selesaikan dengan menggunakan eliminasi Gauss
$$
\begin{array}{cc}
x_1+2x_2+3x_3&=6\\
2x_1+4x_2+6x_3&=12\\
x_2+x_3&=2
\end{array}
$$
jawab:
$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
2 & 4 & 6 & | &12\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 0 & 0 & | &0\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$

$$
\begin{bmatrix}
1 & 2 & 3 & | &6\\
0 & 1 & 1 & | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_2+x_3 = 2\\
x_2 = 2 - x_3\\
\end{array}
$$
$$
\begin{array}{cc}
x_1+2x_2+3x_3 = 6\\
x_2 = 2 - x_3 \\
\end{array}
$$
$$
\begin{array}{cc}
x_1 + 2(2-x_3)+3x_3 = 6\\
x_1 + 4-2x_3+3x_3 = 6\\
x_1+4+x_3\\
x_1=2-x_3
\end{array}
$$
$$
\begin{array}{cc}
x_1 = 2-x_3\\
x_2=2-x_3\\
x_3=x_3
\end{array}
$$

### Soal 2
Selesaikan dengan menggunakan eliminasi Gauss.
$$
\begin{array}{cc}
x_1+x_2+x_3&=3\\
2x_1+2x_3&=5\\
x_1+2x_2&=3
\end{array}
$$
jawab: 
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
2 & 0 & 2 & | &5\\
1 & 2 & 0 & | &3\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 1 & -1& | &0\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 & 1 & | &3\\
0 & -2 & 0 & | &-1\\
0 & 0 & -1 & | &-1/2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
-x_3=-1/2\\
x_3=1/2
\end{array}
$$
$$
\begin{array}{cc}
-2x_2=-1\\
x_2=1/2
\end{array}
$$
$$
\begin{array}{cc}
x_1+x_2+x_3=3\\
x_1+1/2+1/2=3\\
x_1+1=3\\
x_1=2
\end{array}
$$
hasil akhirnya adalah:
$$
\begin{array}{cc}
(x_1+x_2+x_3)=(2,1/2,1/2)
\end{array}
$$

### Soal 3
Selesaikan dengan menggunakan eliminasi Gauss.
$$
\begin{array}{cc}
2x_1+2x_2&=4\\
x_1+x_2&=2
\end{array}
$$
jawab:
$$
\begin{bmatrix}
2 & 2 &  | &4\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 &  | &2\\
1 & 1 &  | &2\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_1+x_2=2\\
x_1=2-x_2\\
x_2=x_2
\end{array}
$$
$$
\begin{array}{cc}
(x_1,x_2)=(2-x_2,x_2)
\end{array}
$$
$$
\begin{array}{cc}
jika(x_2=0),maka((x_1,x_2)=(2,0))\\
jika(x_2=1),maka((x_1,x_2)=(1,1))\\
jika(x_2=2),maka((x_1,x_2)=(0,2))
\end{array}
$$


### Soal 4
Selesaikan dengan menggunakan eliminasi Gauss.
$$
\begin{array}{cc}
x_1+x_2&=5\\
x_1+2x_3&=6
\end{array}
$$
jawab:
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 2 &| &6\\
\end{bmatrix}
\quad
$$
$$
\begin{bmatrix}
1 & 1 &| &5\\
0 & 1 &| &1\\
\end{bmatrix}
\quad
$$
$$
\begin{array}{cc}
x_2=1\\
x_1+1=5\\
x_1=4
\end{array}
$$
jadi:
$$
\begin{array}{cc}
(x_1,x_2)=(4,1)
\end{array}
$$
