<p align="justify"><b>Pandas</b> merupakan salah satu alternatif library yang sering digunakan untuk proses data wrangling. 
Pandas merupakan toolkit yang powerfull sebagai analisis data diawal dan pengenalan struktur dataset dalam Python. 
Mengaktifkan Pandas sangat mudah didalam python. Cukup dengan melakukan import seperti dibawah ini.</br>
<i>import pandas</i></br>
Untuk mempermudah akses dan mempersingkat penamaan biasanya import pandas menggunakan inisial seperti dibawah ini:</br>
<i>Import pandas as pd</i></br>
Setelah melakukan import Anda sudah bisa menggunakan pandas. Untuk lebih memahami lagi apa itu pandas silahkan membaca dokumentasi dari pandas agar mudah untuk melakukan eksplorasi dengan menggunakan pandas.</p>

<p align="justify"><b>Membaca file dengan menggunakan pandas</b></br>Sebagai salah satu library untuk melakukan proses awal dari analisis data, pandas juga memiliki kemampuan untuk membaca berbagai macam jenis file. Format yang bisa dibaca oleh pandas ada berbagai macam, antara lain .txt, .csv, .tsv, dan lainnya. Pandas tidak hanya bisa membaca file saja, namun juga bisa merubah data dari file menjadi bentuk dataframe yang akhirnya nanti bisa diakses, diagregasi dan diolah. Coba praktikan kode di bawah ini :</br></br>
<i>import pandas as pd </br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print(csv_data)	</i></p>


<details> <summary><b>Membaca file dengan menggunakan head()</b></br>Pada suatu kasus, data yang kita baca cukup banyak atau loading yang lama. Untuk memastikan data kita terbaca dengan baik dan bisa menampilkan data sebagian untuk ditampilkan secara benar, kita bisa memakai fungsi head(). Bisa dituliskan kode di bawah ini untuk prakteknya:</br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print(csv_data.head())
</summary><table align="justify"><i>Output : </br></i>
<tr><td></td><td>CustomerID </td><td>Genre</td><td>Age</td><td>Annual Income (k$)</td><td><Spending Score (1-100)/td></tr>
<tr><td>0</td><td>1</td><td>Male</td><td>19</td><td>15</td><td>39</td></tr>
<tr><td>1</td><td>2</td><td>Male </td><td>21</td><td>15</td><td>81</td></tr>
<tr><td>2</td><td>3</td><td>Female </td><td>20</td><td>16 </td><td>6</td></tr>
<tr><td>3</td><td>4</td><td>Female </td><td>23</td><td>16 </td><td>77</td></tr>
<tr><td>4</td><td>5</td><td>Female </td><td>31</td><td>17</td><td>40</td></tr>
  </table></details>
<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary><b>Membaca file dengan menggunakan pandas</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details> 
