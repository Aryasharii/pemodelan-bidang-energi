# Pemodelan Matematika Kompetisi Penjualan Mobil di Indonesia

## Daftar Isi
1. [Pendahuluan](#pendahuluan)
2. [Metode Penelitian](#metode-penelitian)
3. [Hasil Penelitian dan Pembahasan](#hasil-penelitian-dan-pembahasan)
   - [Data Penjualan Mobil Tahunan](#data-penjualan-mobil-tahunan)
   - [Hasil Prediksi Model](#hasil-prediksi-model)
   - [Tabel Nilai Parameter](#tabel-nilai-parameter)
   - [Analisis Hasil dan Pembahasan](#analisis-hasil-dan-pembahasan)
4. [Kesimpulan](#kesimpulan)

## Pendahuluan
Mobilitas menjadi aspek krusial di Indonesia, mendorong persaingan antara produsen mobil seperti Toyota dan Daihatsu. Penelitian ini mengadopsi model Lotka-Volterra untuk menjelaskan dinamika kompetisi penjualan mobil di Indonesia.

## Metode Penelitian
Model Lotka-Volterra digunakan untuk memodelkan kompetisi antara dua produsen mobil, dengan parameter diestimasi menggunakan metode Particle Swarm Optimization (PSO).

## Hasil Penelitian dan Pembahasan
### Data Penjualan Mobil Tahunan
![Gambar 1](https://github.com/Aryasharii/pemodelan-bidang-energi/blob/tubes/image/image1.png)  
*Gambar 1. Data penjualan mobil tahunan untuk produsen pertama*

![Gambar 2](https://github.com/Aryasharii/pemodelan-bidang-energi/blob/tubes/image/image2.png)  
*Gambar 2. Data penjualan mobil tahunan untuk produsen kedua*

### Hasil Prediksi Model
![Gambar 3](https://github.com/Aryasharii/pemodelan-bidang-energi/blob/tubes/image/image3.png)  
*Gambar 3. Perbandingan hasil prediksi model dan data produsen pertama*

![Gambar 4](https://github.com/Aryasharii/pemodelan-bidang-energi/blob/tubes/image/image4.png)  
*Gambar 4. Perbandingan hasil prediksi model dan data produsen kedua*

### Tabel Nilai Parameter
| Parameter | Nilai |
|-----------|-------|
| a<sub>1</sub> | 0.9977860363287 |
| b<sub>1</sub> | 2.9099777961044e-8 |
| K<sub>1</sub> | 434854 |
| a<sub>2</sub> | 0.9995091245261 |
| b<sub>2</sub> | 3.7132213037454e-8 |
| K<sub>2</sub> | 202738 |

### Analisis Hasil dan Pembahasan
Dengan menyubstitusikan nilai-nilai parameter pada Tabel 1 ke dalam persamaan (1)-(2), model matematika persaingan penjualan mobil di Indonesia antara dua produsen, dapat digambarkan sebagai berikut:
\[
\frac{dx_1}{dt} = 0.9977860363287x_1 \left(1-\frac{x_1}{434854}\right) - 2.9099777961044 \times 10^{-8} x_1 x_2 \tag{3}
\]
\[
\frac{dx_2}{dt} = 0.9995091245261x_2 \left(1-\frac{x_2}{202738}\right) - 3.7132213037454 \times 10^{-8} x_1 x_2 \tag{4}
\]

Model matematis persaingan penjualan mobil pada persamaan (3) - (4) memiliki empat kesetimbangan, yaitu:
- Ekuilibrium saat kedua produsen mengalami kebangkrutan \(P_1(y_1, y_2) = (0, 0)\)
- Ekuilibrium kebangkrutan produsen kedua \(P_2(x_1, x_2) = (434854,0)\)
- Ekuilibrium kebangkrutan produsen pertama \(P_3(x, x_2) = (0, 202738)\)
- Ekuilibrium koeksistensi \(P_4(y_1, y_2) = (434854, 202738)\)

Dengan menggunakan metode eigen dapat dilihat bahwa \(P_4\) stabil secara asimtotik sehingga kesetimbangan terjadi pada situasi nyata, sedangkan \(P_1\), \(P_2\), dan \(P_3\) tidak stabil. Dengan penjualan yang stabil produsen utama akan tetap berada di posisi atas dalam penjualan mobil.

## Kesimpulan
Model Lotka-Volterra efektif mengungkap dinamika persaingan penjualan mobil di Indonesia, dengan produsen pertama mendominasi pasar.


### Kesimpulan
Model Lotka-Volterra efektif mengungkap dinamika persaingan penjualan mobil di Indonesia, dengan produsen pertama mendominasi pasar.
