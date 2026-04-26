# Isi

## 1. Persamaan Linear






## 2. Eliminasi Gauss

### Tugas Eliminasi Gauss

#### 1. Sistem Persamaan Linear (SPL) 

$$\begin{aligned}
x_1 + x_2 + x_3 + x_4 + x_5 &= 15 \\
2x_1 + x_2 + x_3 + x_4 + x_5 &= 16 \\
2x_1 + 2x_2 + x_3 + x_4 + x_5 &= 18 \\
2x_1 + 2x_2 + 2x_3 + x_4 + x_5 &= 21 \\
2x_1 + 2x_2 + 2x_3 + 2x_4 + x_5 &= 25
\end{aligned}$$

#### 2. Matriks Augmented 

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 1 & 1 & 1 & 1 & 16 \\
2 & 2 & 1 & 1 & 1 & 18 \\
2 & 2 & 2 & 1 & 1 & 21 \\
2 & 2 & 2 & 2 & 1 & 25
\end{array}
\right]$$

#### 3. Eliminasi Gauss (OBE) 

##### Langkah 1 

Hilangkan elemen di bawah pivot pertama

$$\begin{aligned}
R_2 &= R_2 - 2R_1 \\
R_3 &= R_3 - 2R_1 \\
R_4 &= R_4 - 2R_1 \\
R_5 &= R_5 - 2R_1
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 0 & -1 & -1 & -1 & -12 \\
0 & 0 & 0 & -1 & -1 & -9 \\
0 & 0 & 0 & 0 & -1 & -5
\end{array}
\right]$$

##### Langkah 2 

Ubah pivot menjadi 1

$$\begin{aligned}
R_2 &= -R_2 \\
R_3 &= -R_3 \\
R_4 &= -R_4 \\
R_5 &= -R_5
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 1 & 1 & 1 & 14 \\
0 & 0 & 1 & 1 & 1 & 12 \\
0 & 0 & 0 & 1 & 1 & 9 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

##### Langkah 3 

Hilangkan elemen di atas pivot kelima

$$\begin{aligned}
R_4 &= R_4 - R_5 \\
R_3 &= R_3 - R_5 \\
R_2 &= R_2 - R_5 \\
R_1 &= R_1 - R_5
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 0 & 10 \\
0 & 1 & 1 & 1 & 0 & 9 \\
0 & 0 & 1 & 1 & 0 & 7 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

##### Langkah 4 

Hilangkan elemen di atas pivot keempat

$$\begin{aligned}
R_3 &= R_3 - R_4 \\
R_2 &= R_2 - R_4 \\
R_1 &= R_1 - R_4
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 0 & 0 & 6 \\
0 & 1 & 1 & 0 & 0 & 5 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

##### Langkah 5 

Hilangkan elemen di atas pivot ketiga

$$\begin{aligned}
R_2 &= R_2 - R_3 \\
R_1 &= R_1 - R_3
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 0 & 0 & 0 & 3 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

##### Langkah 6 

Hilangkan elemen di atas pivot kedua

$$R_1 = R_1 - R_2$$

##### Hasil Akhir 

$$\left[
\begin{array}{ccccc|c}
1 & 0 & 0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

![Original image](https://cdn.mathpix.com/snip/images/WTpqR5aPXVTS8cBNsk0NRvljB53KMiftwlZNgFQKGhY.original.fullsize.png)


## UTS

### 1. Sistem Persamaan Linear (SPL) 

$$\begin{aligned}
x_1 + x_2 + x_3 + x_4 + x_5 &= 15 \\
2x_1 + x_2 + x_3 + x_4 + x_5 &= 16 \\
2x_1 + 2x_2 + x_3 + x_4 + x_5 &= 18 \\
2x_1 + 2x_2 + 2x_3 + x_4 + x_5 &= 21 \\
2x_1 + 2x_2 + 2x_3 + 2x_4 + x_5 &= 25
\end{aligned}$$

### 2. Matriks Augmented 

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 1 & 1 & 1 & 1 & 16 \\
2 & 2 & 1 & 1 & 1 & 18 \\
2 & 2 & 2 & 1 & 1 & 21 \\
2 & 2 & 2 & 2 & 1 & 25
\end{array}
\right]$$

### 3. Eliminasi Gauss (OBE) 

#### Langkah 1 

Hilangkan elemen di bawah pivot pertama

$$\begin{aligned}
R_2 &= R_2 - 2R_1 \\
R_3 &= R_3 - 2R_1 \\
R_4 &= R_4 - 2R_1 \\
R_5 &= R_5 - 2R_1
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & -1 & -1 & -1 & -1 & -14 \\
0 & 0 & -1 & -1 & -1 & -12 \\
0 & 0 & 0 & -1 & -1 & -9 \\
0 & 0 & 0 & 0 & -1 & -5
\end{array}
\right]$$

#### Langkah 2 

Ubah pivot menjadi 1

$$\begin{aligned}
R_2 &= -R_2 \\
R_3 &= -R_3 \\
R_4 &= -R_4 \\
R_5 &= -R_5
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
0 & 1 & 1 & 1 & 1 & 14 \\
0 & 0 & 1 & 1 & 1 & 12 \\
0 & 0 & 0 & 1 & 1 & 9 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

#### Langkah 3 

Hilangkan elemen di atas pivot kelima

$$\begin{aligned}
R_4 &= R_4 - R_5 \\
R_3 &= R_3 - R_5 \\
R_2 &= R_2 - R_5 \\
R_1 &= R_1 - R_5
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 0 & 10 \\
0 & 1 & 1 & 1 & 0 & 9 \\
0 & 0 & 1 & 1 & 0 & 7 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

#### Langkah 4 

Hilangkan elemen di atas pivot keempat

$$\begin{aligned}
R_3 &= R_3 - R_4 \\
R_2 &= R_2 - R_4 \\
R_1 &= R_1 - R_4
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 0 & 0 & 6 \\
0 & 1 & 1 & 0 & 0 & 5 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

#### Langkah 5 

Hilangkan elemen di atas pivot ketiga

$$\begin{aligned}
R_2 &= R_2 - R_3 \\
R_1 &= R_1 - R_3
\end{aligned}$$

Hasil

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 0 & 0 & 0 & 3 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

#### Langkah 6 

Hilangkan elemen di atas pivot kedua

$$R_1 = R_1 - R_2$$

#### Hasil Akhir 

$$\left[
\begin{array}{ccccc|c}
1 & 0 & 0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 & 0 & 2 \\
0 & 0 & 1 & 0 & 0 & 3 \\
0 & 0 & 0 & 1 & 0 & 4 \\
0 & 0 & 0 & 0 & 1 & 5
\end{array}
\right]$$

### Determinan Matrix $A$

Kita gunakan matriks koefisien:

A = 
$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 \\
2 & 1 & 1 & 1 & 1 \\
2 & 2 & 1 & 1 & 1 \\
2 & 2 & 2 & 1 & 1 \\
2 & 2 & 2 & 2 & 1
\end{array}
\right]$

Gunakan eliminasi baris (tidak mengubah determinan jika hanya operasi $R_i - kR_j$).

Langkah:

$$R_2 = R_2 - 2R_1$$
$$R_3 = R_3 - 2R_1$$
$$R_4 = R_4 - 2R_1$$
$$R_5 = R_5 - 2R_1$$

Hasil:

$$
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 \\
0 & -1 & -1 & -1 & -1 \\
0 & 0 & -1 & -1 & -1 \\
0 & 0 & 0 & -1 & -1 \\
0 & 0 & 0 & 0 & -1
\end{bmatrix}
$$

Sekarang matriks menjadi **segitiga atas**, maka:

$$ \det(A) = 1 \times (-1) \times (-1) \times (-1) \times (-1) $$

$$ \det(A) = 1 $$

### Adjoin Matriks

Contoh Perhitungan (Beberapa Elemen)
#### a. Elemen $C_{11}$

Hilangkan baris 1 kolom 1:

$$
\begin{vmatrix}
1 & 1 & 1 & 1 \\
2 & 1 & 1 & 1 \\
2 & 2 & 1 & 1 \\
2 & 2 & 2 & 1
\end{vmatrix}
$$

Hasil determinannya = 1

Karena posisi (1,1):

$$ \Downarrow $$

$$ C_{11} = (+1)(1) = 1 $$

#### b. Elemen $C_{12}$

Hilangkan baris 1 kolom 2:

$$
\begin{vmatrix}
2 & 1 & 1 & 1 \\
2 & 1 & 1 & 1 \\
2 & 2 & 1 & 1 \\
2 & 2 & 2 & 1
\end{vmatrix}
$$

Determinannya = 0 (karena ada baris sama)

$$ C_{12} = (-1)(0) = 0 $$

#### Pola yang terjadi

Karena matriks ini berbentuk segitiga, maka
- Banyak minor menjadi 0
- kofaktor membentuk pola sederhana

#### Hasil Adjoin Matriks

Hasil akhirnya:

$$
\text{adj}(A) =
\begin{bmatrix}
-1 & 1 & 0 & 0 & 0 \\
2 & -1 & 1 & 0 & 0 \\
0 & 2 & -1 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 \\
0 & 0 & 0 & 2 & -1
\end{bmatrix}
$$

(Pola ini muncul karena bentuk matriks yang bertingkat/segitiga).

### Invers Matriks

Rumus:

$$ A^{-1} = \frac{1}{\det(A)} \cdot \text{adj}(A) $$

Karena:

$$ \det(A) = 1 $$

maka:

$$ A^{-1} = \text{adj}(A) $$

Jadi, hasil invers:

$$
A^{-1} = \begin{bmatrix}
-1 & 1 & 0 & 0 & 0 \\
2 & -1 & 1 & 0 & 0 \\
0 & 2 & -1 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 \\
0 & 0 & 0 & 2 & -1
\end{bmatrix}
$$

## Evaluasi Determinan dan Invers

#### 1. Matriks 2 x 2

$$A = \begin{bmatrix} -7 & -5 \\ 1 & 4 \end{bmatrix}$$

Kita gunakan ekspansi baris pertama ($i=1$):

* $a_{11} = -7, M_{11} = \det[4] = 4$
* $a_{12} = -5, M_{12} = \det[1] = 1$

$$ \det(A) = (-1)^{1+1}(-7)(4) + (-1)^{1+2}(-5)(1) $$

$$ \det(A) = (1)(-28) + (-1)(-5) $$

$$ \det(A) = -28 + 5 = \mathbf{-23} $$

#### 2. Matriks 3 x 3

$A = \begin{bmatrix} 0 & 2 & -3 \\ 1 & -2 & -1 \\ 0 & 0 & 1 \end{bmatrix}$

Untuk memudahkan, kita gunakan ekspansi **baris ketiga** ($i = 3$) karena memiliki banyak angka nol:

* $a_{31} = 0, a_{32} = 0$
* $a_{33} = 1, M_{33} = \det \begin{bmatrix} 0 & 2 \\ 1 & -2 \end{bmatrix} = (0)(-2) - (2)(1) = -2$

$$ \det(A) = 0 + 0 + (-1)^{3+3}(1)(-2) $$

$$ \det(A) = (1)(1)(-2) = -2 $$

#### 3. Matriks 4 x 4

$A = \begin{bmatrix} 1 & -3 & 1 & 1 \\ -3 & 1 & 1 & 1 \\ 1 & 1 & -3 & 1 \\ 1 & 1 & 1 & -3 \end{bmatrix}$

Kita gunakan ekspansi baris pertama ($i = 1$):

$$ \det(A) = 1 \cdot C_{11} + (-3) \cdot C_{12} + 1 \cdot C_{13} + 1 \cdot C_{14} $$

Setelah menghitung kofaktor masing-masing submatriks $3 \times 3$:

*   $C_{11} = +16$
*   $C_{12} = -(-16) = 16$
*   $C_{13} = +16$
*   $C_{14} = -(-16) = 16$

$$ \det(A) = 1(16) + (-3)(16) + 1(16) + 1(16) $$

$$ \det(A) = 16 - 48 + 16 + 16 = \mathbf{0} $$

(Karena jumlah setiap baris adalah 0, maka determinannya pasti 0)

### B: Menghitung Invers (Matriks Adjoin)
Rumus: $A^{-1} = \frac{1}{\det(A)}\text{adj}(A)$, dengan $\text{adj}(A) = (\text{Kofaktor } A)^T$.

#### 4. Matriks 2 x 2

$A = \begin{bmatrix} -7 & -5 \\ 1 & 4 \end{bmatrix}$

Dari soal nomor 1, $\det(A) = -23$.

*   Kofaktor: $C_{11} = 4, C_{12} = -1, C_{21} = 5, C_{22} = -7$
*   $\text{adj}(A) = \begin{bmatrix} 4 & 5 \\ -1 & -7 \end{bmatrix}$

$$ A^{-1} = \frac{1}{-23} \begin{bmatrix} 4 & 5 \\ -1 & -7 \end{bmatrix} = \begin{bmatrix} -4/23 & -5/23 \\ 1/23 & 7/23 \end{bmatrix} $$

#### 5. Matriks 3 x 3

$A = \begin{bmatrix} 0 & 2 & -3 \\ 1 & -2 & -1 \\ 0 & 0 & 1 \end{bmatrix}$

Dari soal nomor 2, $\text{det}(A) = -2$. Cari semua kofaktor $C_{ij}$:

*   $C_{11} = -2, C_{12} = -1, C_{13} = 0$
*   $C_{21} = -2, C_{22} = 0, C_{23} = 0$
*   $C_{31} = -8, C_{32} = -3, C_{33} = -2$

$$ \text{adj}(A) = \begin{bmatrix} -2 & -2 & -8 \\ -1 & 0 & -3 \\ 0 & 0 & -2 \end{bmatrix} $$

$$ A^{-1} = \frac{1}{-2} \begin{bmatrix} -2 & -2 & -8 \\ -1 & 0 & -3 \\ 0 & 0 & -2 \end{bmatrix} = \begin{bmatrix} 1 & 1 & 4 \\ 0.5 & 0 & 1.5 \\ 0 & 0 & 1 \end{bmatrix} $$