# Tugas Eliminasi Gauss

## 1. Sistem Persamaan Linear (SPL) {#sistem-persamaan-linear-spl .unnumbered}

$$\begin{aligned}
x_1 + x_2 + x_3 + x_4 + x_5 &= 15 \\
2x_1 + x_2 + x_3 + x_4 + x_5 &= 16 \\
2x_1 + 2x_2 + x_3 + x_4 + x_5 &= 18 \\
2x_1 + 2x_2 + 2x_3 + x_4 + x_5 &= 21 \\
2x_1 + 2x_2 + 2x_3 + 2x_4 + x_5 &= 25
\end{aligned}$$

## 2. Matriks Augmented {#matriks-augmented .unnumbered}

$$\left[
\begin{array}{ccccc|c}
1 & 1 & 1 & 1 & 1 & 15 \\
2 & 1 & 1 & 1 & 1 & 16 \\
2 & 2 & 1 & 1 & 1 & 18 \\
2 & 2 & 2 & 1 & 1 & 21 \\
2 & 2 & 2 & 2 & 1 & 25
\end{array}
\right]$$

## 3. Eliminasi Gauss (OBE) {#eliminasi-gauss-obe .unnumbered}

### Langkah 1 {#langkah-1 .unnumbered}

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

### Langkah 2 {#langkah-2 .unnumbered}

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

### Langkah 3 {#langkah-3 .unnumbered}

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

### Langkah 4 {#langkah-4 .unnumbered}

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

### Langkah 5 {#langkah-5 .unnumbered}

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

### Langkah 6 {#langkah-6 .unnumbered}

Hilangkan elemen di atas pivot kedua

$$R_1 = R_1 - R_2$$

### Hasil Akhir {#hasil-akhir .unnumbered}

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