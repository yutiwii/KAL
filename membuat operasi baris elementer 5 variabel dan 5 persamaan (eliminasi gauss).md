<script src="https://sagecell.sagemath.org/static/embedded_sagecell.js"></script>

<script>
sagecell.makeSagecell({
inputLocation: ".sage"
});
</script>

# Operasi baris  elementer 5 variabel dengan 5 persamaan

$$
x_1 &​+& x_2 &​+& x_3 &​+& x_4​ &+& x_5 &​=& 5\\
2x_1 &​+& 3x_2​ &​+& x_3​ &​+& 4x_4​ &​+& x5 &​=& 12\\
x_1​ &​+& 2x_2​ &​+& 3x_3​ &​+& x_4​ &​+& 2x_5 &=& 10\\
​3x_1​ &​+& x_2​ &​+& 2x_3​ &​+& 2x_4​ &​+& x_5 &=& 11\\
​2x_1​ &​+& x_2​ &​+& x_3​ &​+& 3x_4​ &​+& 2x_5 &​​=& 10​
$$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
2 & 3 & 1 & 4 & 1 & 12\\
1 & 2 & 3 & 1 & 2 & 10\\
3 & 1 & 2 & 2 & 1 & 11\\
2 & 1 & 1 & 3 & 2 & 10
\end{bmatrix}
$$

###### Langkah 1 
$R_2 \rightarrow R_2 - 2R_1$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
1 & 2 & 3 & 1 & 2 & 10\\
3 & 1 & 2 & 2 & 1 & 11\\
2 & 1 & 1 & 3 & 2 & 10
\end{bmatrix}
$$

$R_3 \rightarrow R_3 - R_1$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 1 & 2 & 0 & 1 & 5\\
3 & 1 & 2 & 2 & 1 & 11\\
2 & 1 & 1 & 3 & 2 & 10
\end{bmatrix}
$$

$R_4 \rightarrow R_4 - 3R_1$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 1 & 2 & 0 & 1 & 5\\
0 & -2 & -1 & -1 & -2 & -4\\
2 & 1 & 1 & 3 & 2 & 10
\end{bmatrix}
$$

$R_5 \rightarrow R_5 - 2R_1$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 1 & 2 & 0 & 1 & 5\\
0 & -2 & -1 & -1 & -2 & -4\\
0 & -1 & -1 & 1 & 0 & 0
\end{bmatrix}
$$

###### Langkah 2
$R_3 \rightarrow R_3 - R_2$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & -2 & -1 & -1 & -2 & -4\\
0 & -1 & -1 & 1 & 0 & 0
\end{bmatrix}
$$

$R_4 \rightarrow R_4 + 2R_2$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & -3 & 3 & -4 & 0\\
0 & -1 & -1 & 1 & 0 & 0
\end{bmatrix}
$$

$R_5 \rightarrow R_5 + R_2$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & -3 & 3 & -4 & 0\\
0 & 0 & -2 & 3 & -1 & 2
\end{bmatrix}
$$

###### Langkah 3
$R_4 \rightarrow R_4 + R_3$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & 0 & 1 & -2 & 3\\
0 & 0 & -2 & 3 & -1 & 2
\end{bmatrix}
$$

$R_5 \rightarrow 3R_5 + 2R_3$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & 0 & 1 & -2 & 3\\
0 & 0 & 0 & 5 & 1 & 12
\end{bmatrix}
$$

###### Langkah 4
$R_5 \rightarrow R_5 - 5R_4$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & 0 & 1 & -2 & 3\\
0 & 0 & 0 & 0 & 11 & -3
\end{bmatrix}
$$

###### Langkah 5
$R_5 \rightarrow \dfrac{1}{11}R_5$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 2\\
0 & 0 & 3 & -2 & 2 & 3\\
0 & 0 & 0 & 1 & -2 & 0\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

###### Langkah 6
$R_4 \rightarrow R_4 + 2R_5$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 0\\
0 & 0 & 3 & -2 & 2 & 4\\
0 & 0 & 0 & 1 & 0 & \dfrac{27}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_3 \rightarrow R_3 - 2R_5$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & -1 & 0\\
0 & 0 & 3 & -2 & 0 & \dfrac{50}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_2 \rightarrow R_2 + R_5$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 1 & 5\\
0 & 1 & -1 & 2 & 0 & -\dfrac{3}{11}\\
0 & 0 & 3 & -2 & 0 & \dfrac{50}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_1 \rightarrow R_1 - R_5$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 0 & \dfrac{55}{11}\\
0 & 1 & -1 & 2 & 0 & -\dfrac{3}{11}\\
0 & 0 & 3 & -2 & 0 & \dfrac{50}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

###### Langkah 7 
$R_3 \rightarrow R_3 + 2R_4$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 0 & \dfrac{55}{11}\\
0 & 1 & -1 & 2 & 0 & -\dfrac{3}{11}\\
0 & 0 & 3 & 0 & 0 & \dfrac{38}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_2 \rightarrow R_2 - 2R_4$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 1 & 0 & \dfrac{55}{11}\\
0 & 1 & -1 & 0 & 0 & \dfrac{9}{11}\\
0 & 0 & 3 & 0 & 0 & \dfrac{38}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_1 \rightarrow R_1 - R_4$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 0 & 0 & \dfrac{61}{11}\\
0 & 1 & -1 & 0 & 0 & -\dfrac{15}{11}\\
0 & 0 & 3 & 0 & 0 & \dfrac{38}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

###### Langkah 8
$R_3 \rightarrow \dfrac{1}{3}R_3$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 0 & 0 & \dfrac{61}{11}\\
0 & 1 & -1 & 0 & 0 & -\dfrac{15}{11}\\
0 & 0 & 1 & 0 & 0 & \dfrac{38}{33}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_2 \rightarrow R_2 + R_3$

$$ 
\begin{bmatrix}
1 & 1 & 1 & 0 & 0 & \dfrac{61}{11}\\
0 & 1 & 0 & 0 & 0 & \dfrac{46}{11}\\
0 & 0 & 1 & 0 & 0 & \dfrac{38}{33}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_1 \rightarrow R_1 - R_3$

$$ 
\begin{bmatrix}
1 & 1 & 0 & 0 & 0 & \dfrac{23}{11}\\
0 & 1 & 0 & 0 & 0 & \dfrac{46}{11}\\
0 & 0 & 1 & 0 & 0 & \dfrac{38}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

$R_1 \rightarrow R_1 - R_2$

$$ 
\begin{bmatrix}
1 & 0 & 0 & 0 & 0 & -\dfrac{23}{11}\\
0 & 1 & 0 & 0 & 0 & \dfrac{46}{11}\\
0 & 0 & 1 & 0 & 0 & \dfrac{38}{11}\\
0 & 0 & 0 & 1 & 0 & -\dfrac{6}{11}\\
0 & 0 & 0 & 0 & 1 & -\dfrac{3}{11}
\end{bmatrix}
$$

#### 1. Membuat Matriks Augmented

Sistem persamaan diubah menjadi matriks diperluas.

$$
\begin{aligned}
x_1 + x_2 + x_3 + x_4 + x_5 &= 5 \\
2x_1 + 3x_2 + x_3 + 4x_4 + x_5 &= 12 \\
x_1 + 2x_2 + 3x_3 + x_4 + 2x_5 &= 10 \\
3x_1 + x_2 + 2x_3 + 2x_4 + x_5 &= 11 \\
2x_1 + x_2 + x_3 + 3x_4 + 2x_5 &= 10
\end{aligned}
$$

<div class="sage">
<script type="text/x-sage">
A = Matrix([
[1,1,1,1,1,5],
[2,3,1,4,1,12],
[1,2,3,1,2,10],
[3,1,2,2,1,11],
[2,1,1,3,2,10]
])

A
</script>
</div>

#### 2. Operasi Baris 1 (Eliminasi kolom pertama)
$$
𝑅_2 = 𝑅_2 − 2𝑅_1
$$	​

<div class="sage">
<script type="text/x-sage">
A[1] = A[1] - 2*A[0]
A
</script>
</div>

$$
R_3​ = R_3 ​− R_1​
$$

<div class="sage">
<script type="text/x-sage">
A[2] = A[2] - A[0]
A
</script>
</div>

$$
R_4 ​= R_4 ​− 3R_1​
$$

<div class="sage">
<script type="text/x-sage">
A[3] = A[3] - 3*A[0]
A
</script>
</div>

$$
R_5 ​= R_5 ​− 2R_1​
$$

<div class="sage">
<script type="text/x-sage">
A[4] = A[4] - 2*A[0]
A
</script>
</div>

#### 3. Eliminasi Kolom Kedua

Pivot di $R_2$

$$
R_3 ​= R_3 ​− R_2​
$$

<div class="sage">
<script type="text/x-sage">
A[2] = A[2] - A[1]
A
</script>
</div>

$$
R4​ = R_4​ + 2R_2​
$$

<div class="sage">
A[3] = A[3] + 2*A[1]
A
</script>
</div>

$$
R_5 ​= R_5 ​+ R_2​
$$

<div class="sage">
<script type="text/x-sage">
A[4] = A[4] + A[1]
A
</script>
</div>

#### 4. Eliminasi Kolom Ketiga

$$
R_4 ​= R_4 ​− 3R_3​
$$

<div class="sage">
<script type="text/x-sage">
A[3] = A[3] - 3*A[2]
A
</script>
</div>

$$
R_5 = R_5 − 2R_3
$$

<div class="sage">
<script type="text/x-sage">
A[4] = A[4] - 2*A[2]
A
</script>
</div>

5. Membuat Matriks Eselon

Untuk melihat hasil langsung di Sage:

<div class="sage">
<script type="text/x-sage">
A.echelon_form()
</script>
</div>

atau

<div class="sage">
<script type="text/x-sage">
A.rref()
</script>
</div>

#### 6. Mendapatkan Nilai Variabel

<div class="sage">
<script type="text/x-sage">
A = Matrix([
[1,1,1,1,1],
[2,3,1,4,1],
[1,2,3,1,2],
[3,1,2,2,1],
[2,1,1,3,2]
])

b = vector([5,12,10,11,10])

A.solve_right(b)
</script>
</div>
