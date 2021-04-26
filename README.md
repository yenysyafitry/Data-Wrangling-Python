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


<details> <summary align="justify"><b>Membaca file dengan menggunakan head()</b></br>Pada suatu kasus, data yang kita baca cukup banyak atau loading yang lama. Untuk memastikan data kita terbaca dengan baik dan bisa menampilkan data sebagian untuk ditampilkan secara benar, kita bisa memakai fungsi head(). Bisa dituliskan kode di bawah ini untuk prakteknya:</br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print(csv_data.head()) </br> </br>
</summary><table align="justify"><i></br>Output : </br></i>
<tr><td></td><td>CustomerID </td><td>Genre</td><td>Age</td><td>Annual Income(k$)</td> <td>Spending Score (1-100)</td></tr>
<tr><td>0</td><td>1</td><td>Male</td><td>19</td><td>15</td><td>39</td></tr>
<tr><td>1</td><td>2</td><td>Male </td><td>21</td><td>15</td><td>81</td></tr>
<tr><td>2</td><td>3</td><td>Female </td><td>20</td><td>16 </td><td>6</td></tr>
<tr><td>3</td><td>4</td><td>Female </td><td>23</td><td>16 </td><td>77</td></tr>
</br>
  </table></details>

<details> <summary align="justify"><b>Melakukan akses data kolom</b></br>Pertama yang harus dilakukan untuk melakukan akses kolom adalah mengetahui nama-nama kolom yang ada. Coba ketikkan kode di bawah ini untuk melihat nama kolom yang ada :</br></br><i>import pandas as pd</br>
csv_data = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/shopping_data.csv")</br>
print(csv_data['Age'])</i>
</summary><table align="justify"><i></br>Output : </br></i>
<tr><td>0  </td><td>    19</td></tr>
<tr><td>1  </td><td>    21</td></tr>
<tr><td>2   </td><td>   20</td></tr>
<tr><td>3   </td><td>   23</td></tr>
<tr><td>4  </td><td>    31</td></tr>
<tr><td>5   </td><td>   22</td></tr>
<tr><td>6  </td><td>    35</td></tr>
<tr><td>7  </td><td>    23</td></tr>
<tr><td>8  </td><td>    64</td></tr>
<tr><td>9   </td><td>   30</td></tr>
<tr><td>10  </td><td>   67</td></tr>
<tr><td>11  </td><td>   35</td></tr>
<tr><td>12  </td><td>   58</td></tr>
<tr><td>13  </td><td>   24</td></tr>
<tr><td>14   </td><td>  37</td></tr>
<tr><td>15   </td><td>  22</td></tr>
<tr><td>16  </td><td>   35</td></tr>
<tr><td>17  </td><td>   20</td></tr>
<tr><td>18  </td><td>   52</td></tr>
<tr><td>19  </td><td>   35</td></tr>
<tr><td>20  </td><td>   35</td></tr>
<tr><td>21  </td><td>   25</td></tr>
<tr><td>22  </td><td>   46</td></tr>
<tr><td>23  </td><td>   31</td></tr>
<tr><td>24  </td><td>   54</td></tr>
<tr><td>25  </td><td>   29</td></tr>
<tr><td>26  </td><td>   45</td></tr>
<tr><td>27  </td><td>   35</td></tr>
<tr><td>28  </td><td>   40</td></tr>
<tr><td>29  </td><td>   23</td></tr>
<tr><td>    </td><td>   ..</td></tr>
<tr><td>170  </td><td>  40</td></tr>
<tr><td>171  </td><td>  28</td></tr>
<tr><td>172  </td><td>  36</td></tr>
<tr><td>173 </td><td>   36</td></tr>
<tr><td>174 </td><td>   52</td></tr>
<tr><td>175 </td><td>   30</td></tr>
<tr><td>176 </td><td>   58</td></tr>
<tr><td>177 </td><td>   27</td></tr>
<tr><td>178 </td><td>   59</td></tr>
<tr><td>179 </td><td>   35</td></tr>
<tr><td>180 </td><td>   37</td></tr>
<tr><td>181  </td><td>  32</td></tr>
<tr><td>182  </td><td>  46</td></tr>
<tr><td>183  </td><td>  29</td></tr>
<tr><td>184  </td><td>  41</td></tr>
<tr><td>185 </td><td>   30</td></tr>
<tr><td>186  </td><td>  54</td></tr>
<tr><td>187  </td><td>  28</td></tr>
<tr><td>188  </td><td>  41</td></tr>
<tr><td>189  </td><td>  36</td></tr>
<tr><td>190 </td><td>   34</td></tr>
<tr><td>191 </td><td>   32</td></tr>
<tr><td>192 </td><td>   33</td></tr>
<tr><td>193 </td><td>   38</td></tr>
<tr><td>194 </td><td>   47</td></tr>
<tr><td>195 </td><td>   35</td></tr>
<tr><td>196 </td><td>   45</td></tr>
<tr><td>197 </td><td>   32</td></tr>
<tr><td>198 </td><td>   32</td></tr>
<tr><td>199 </td><td>   30</td></tr></br>
Name: Age, Length: 200, dtype: int64
</table></details>

<details> <summary align="justify"><b>Melakukan akses data melalui baris</b></br>Selain melakukan akses data melalui kolom, dengan menggunakan pandas juga bisa melakukan akses dengan menggunakan baris. Berbeda dengan akses melalui kolom, fungsi untuk menampilkan data dari suatu baris adalah fungsi .iloc[i] dimana [i] menunjukan urutan baris yang akan ditampilkan yang dimana indexnya diawali dari 0. Coba ketikan code di bawah ini untuk mempermudah : </br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print(csv_data.iloc[5])	
</summary><table align="justify"><i></br>Output : </br></i>
<tr><td>CustomerID    </td><td>                 6</td></tr>
<tr><td>Genre         </td><td>            Female</td></tr>
<tr><td>Age           </td><td>                22</td></tr>
<tr><td>Annual Income (k$)    </td><td>        17</td></tr>
<tr><td>Spending Score (1-100)  </td><td>      76</td></tr></br>
<tr><td>Name: 5 </td><td> dtype: object
</table></details>

<details> <summary align="justify"><b>Menampilkan suatu data dari baris dan kolom tertentu</b></br>
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details>

<details> <summary align="justify"><b>Membaca file dengan menggunakan pandas</b></br>Tidak hanya dengan menentukan dari kolom dan baris, dengan menggunakan pandas kita juga bisa memanggil suatu data dari suatu baris dan kolom tertentu dalam satu waktu. Perhatikan dan coba kode di bawah ini:</br></br> import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print(csv_data['Age'].iloc[1])</br>
print("Cuplikan Dataset:")</br>
print(csv_data.head())				
</summary><table align="justify"><i>Output : </br></i>
 <tr><td></td><td> CustomerID </td><td>   Genre  </td><td> Age </td><td>  Annual Income (k$) </td><td>  Spending Score (1-100)</td></tr>
<tr><td>0   </td><td>         1  </td><td>   Male  </td><td>  19 </td><td>                  15 </td><td>                      39</td></tr>
<tr><td>1   </td><td>         2  </td><td>   Male  </td><td>  21 </td><td>                  15  </td><td>                     81</td></tr>
<tr><td>2   </td><td>         3  </td><td> Female  </td><td>  20  </td><td>                 16  </td><td>                      6</td></tr>
<tr><td>3   </td><td>         4  </td><td> Female  </td><td>  23 </td><td>                  16  </td><td>                     77</td></tr>
<tr><td>4   </td><td>         5  </td><td> Female  </td><td>  31  </td><td>                 17  </td><td>                     40</td></tr>
</table></details>

<details> <summary align="justify"><b>Menampilkan data dalam range tertentu</b></br>Setelah menampilkan suatu kelompok data, bagaimana jika ingin menampilkan data dari baris ke 5 sampai ke 20 dari suatu dataset? Untuk mengantisipasi hal tersebut, pandas juga bisa menampilkan data dalam range tertentu, baik range untuk baris saja, kolom saja, dan range untuk baris dan kolom.
  Akses range pada suatu kolom dan baris tertentu, untuk mencobanya silahkan ketikkan kode di bawah ini :</br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data.csv")</br>
print("Menampilkan data ke 5 sampai kurang dari 10 dalam satu baris:")</br>
print(csv_data.iloc[5:10])
</summary><table align="justify"><i>Output : </br></i>
<tr><td></td><td>CustomerID </td><td>  Genre </td><td> Age </td><td> Annual Income (k$)  </td><td>Spending Score (1-100)</td></tr>
<tr><td>5       </td><td>    6 </td><td> Female  </td><td> 22  </td><td>                17 </td><td>                     76</td></tr>
<tr><td>6       </td><td>    7 </td><td> Female  </td><td> 35   </td><td>               18 </td><td>                      6</td></tr>
<tr><td>7       </td><td>    8 </td><td> Female  </td><td> 23 </td><td>                 18  </td><td>                    94</td></tr>
<tr><td>8       </td><td>    9 </td><td>   Male  </td><td> 64  </td><td>                19  </td><td>                     3</td></tr>
<tr><td>9       </td><td>   10 </td><td> Female  </td><td> 30  </td><td>                19  </td><td>                    72</td></tr>
</table></details>

<details> <summary align="justify"><b>Menampilkan informasi statistik dengan Numpy</b></br>Mengetahui informasi statistik pada suatu data sangat penting. Mulai dari distribusi data, nilai max atau min, hingga standar deviasi dari suatu dataset. Jika datanya berjumlah dibawah 10 mungkin masih dikerjakan secara manual. Namun, bayangkan jika datanya sudah mencapai ratusan bahkan ribuan. Tidak mungkin pastinya untuk dilakukan secara manual. Maka dari itu pentingnya fungsi describe() pada pandas. Fungsi describe() ini memungkinkan untuk mengetahui informasi statistik dari suatu dataset secara cepat. Coba untuk ketikkan kode di bawah ini :</br></br>import pandas as pd</br>
csv_data = pd.read_csv("shopping_data.csv")</br>
print(csv_data.describe(exclude=['O']))
</summary><table align="justify"><i>Output : </br></i>
<tr><td></td><td>        CustomerID </td><td>        Age </td><td> Annual Income (k$)</td><td>  Spending Score (1-100)</td></tr>
<tr><td>count</td><td>  200.000000 </td><td> 200.000000  </td><td>        200.000000  </td><td>            200.000000</td></tr>
<tr><td>mean </td><td>  100.500000  </td><td> 38.850000   </td><td>        60.560000  </td><td>             50.200000</td></tr>
<tr><td>std  </td><td>   57.879185 </td><td>  13.969007   </td><td>        26.264721  </td><td>             25.823522</td></tr>
<tr><td>min </td><td>     1.000000  </td><td> 18.000000  </td><td>         15.000000  </td><td>              1.000000</td></tr>
<tr><td>25% </td><td>    50.750000  </td><td> 28.750000   </td><td>        41.500000  </td><td>             34.750000</td></tr>
<tr><td>50%  </td><td>  100.500000  </td><td> 36.000000   </td><td>        61.500000  </td><td>             50.000000</td></tr>
<tr><td>75%  </td><td>  150.250000 </td><td>  49.000000   </td><td>        78.000000  </td><td>             73.000000</td></tr>
<tr><td>max  </td><td>  200.000000 </td><td>  70.000000   </td><td>       137.000000  </td><td>             99.000000</td></tr>
</table></details>

<details> <summary align="justify"><b>Melakukan pengecekan untuk nilai NULL yang ada</b></br>Dengan menggunakan fungsi pandas, kita tidak perlu melihat satu persatu baris data untuk mengetahui apakah ada nilai kosong atau NULL/NAN pada suatu dataset. Bayangkan jika kita memilki 1000 baris data. Apakah kita harus melihat semua baris data tersebut? Tentu saja tidak. Maka dari itu di pandas disediakan fungsi untuk mengecek apakah ada data yang kosong. Coba praktikkan kode di bawah ini :</br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data_missingvalue.csv")</br>
print(csv_data.isnull().values.any())
</summary><table align="justify"><i>Output : </br>True</i></table></details> 


<details> <summary align="justify"><b>Mengisi dengan Mean</b></br>Fungsi mean sendiri berfungsi untuk menampilkan  nilai mean (rata-rata) dari setiap kolom. Nilai inilah nanti yang akan mengisi nilai kosong dari dataset yang mengalami kasus missing value. Untuk mengisi nilai yang kosong menggunakan fungsi fillna(), coba ketikkan kode di bawah ini :</br></br>import pandas as pd</br>
csv_data = pd.read_csv("https://dqlab-dataset.s3-ap-southeast-1.amazonaws.com/shopping_data_missingvalue.csv")</br>
print(csv_data.mean())</br>
print("Dataset yang masih terdapat nilai kosong ! :")</br>
print(csv_data.head(10))</br>
csv_data=csv_data.fillna(csv_data.mean())</br>
print("Dataset yang sudah diproses Handling Missing Values dengan Mean :")</br>
print(csv_data.head(10))
</summary><table align="justify"><i>Output : </br>25</br>
Academy DQLab</i></table></details> 

<details> <summary align="justify"><b>Mengisi dengan Median</b></br>median digunakan untuk data-data yang memiliki sifat outlier yang kuat. Kenapa median dipilih? Median merupakan nilai tengah yang artinya bukan hasil dari perhitungan yang melibatkan data outlier. Pada beberapa kasus, data outlier dianggap mengganggu dan sering dianggap noisy karena bisa mempengaruhi distribusi kelas dan mengganggu analisa pada klasterisasi (clustering).</br></br>
</summary><table align="justify"><i>Output : </br></i>
<tr><td></td><td>  CustomerID  </td><td> Genre </td><td>       Age </td><td> Annual Income (k$) </td><td> Spending Score (1-100)</td></tr>
<tr><td>0     </td><td>      1  </td><td>  Male </td><td> 19.000000 </td><td>          15.000000 </td><td>              39.000000</td></tr>
<tr><td>1     </td><td>      2  </td><td>  Male </td><td> 38.939698 </td><td>          15.000000  </td><td>             81.000000</td></tr>
<tr><td>2     </td><td>      3  </td><td>Female </td><td> 20.000000  </td><td>         61.005051   </td><td>             6.000000</td></tr>
<tr><td>3     </td><td>      4  </td><td>Female </td><td> 23.000000  </td><td>         16.000000   </td><td>            77.000000</td></tr>
<tr><td>4     </td><td>      5 </td><td> Female </td><td> 31.000000  </td><td>         17.000000   </td><td>            50.489899</td></tr>
<tr><td>5     </td><td>      6 </td><td> Female </td><td> 22.000000  </td><td>         61.005051   </td><td>            76.000000</td></tr>
<tr><td>6     </td><td>      7 </td><td> Female </td><td> 35.000000  </td><td>         18.000000   </td><td>             6.000000</td></tr>
<tr><td>7     </td><td>      8 </td><td> Female </td><td> 23.000000  </td><td>         18.000000   </td><td>            94.000000</td></tr>
<tr><td>8    </td><td>       9 </td><td>   Male </td><td> 64.000000  </td><td>         19.000000    </td><td>           50.489899</td></tr>
<tr><td>9     </td><td>     10 </td><td> Female </td><td> 30.000000  </td><td>         19.000000    </td><td>           72.000000</td></tr>
</table></details> 


<details> <summary align="justify"><b>Praktek Normalisasi menggunakan Scikit Learn pada Python</b></br>Scikit Learn merupakan library pada python yang digunakan untuk machine learning dan data science. Salah satu library yang selalu menjadi favorit dan komunitasnya sangat kuat. Scikit-learn sendiri tidak hanya untuk analytics saja, namun juga untuk pre-processing, feature selection, dan proses analysis lainnya. Melanjutkan dari sesi normalisasi data, mari kita praktekan kode di bawah ini :</br></br>import pandas as pd</br>
import numpy as np</br>
from sklearn import preprocessing</br>
csv_data = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/shopping_data.csv")</br>
array = csv_data.values</br>
X = array[:,2:5] #memisahkan fitur dari dataset</br>
Y = array[:,0:1]  #memisahkan class dari dataset</br>
dataset=pd.DataFrame({'Customer ID':array[:,0],'Gender':array[:,1],'Age':array[:,2],'Income':array[:,3],'Spending Score':array[:,4]})</br>
print("dataset sebelum dinormalisasi :")</br>
print(dataset.head(10))</br>
min_max_scaler = preprocessing.MinMaxScaler(feature_range=(0,1)) #inisialisasi normalisasi MinMax</br>
data = min_max_scaler.fit_transform(X) #transformasi MinMax untuk fitur</br>
dataset = pd.DataFrame({'Age':data[:,0],'Income':data[:,1],'Spending Score':data[:,2],'Customer ID':array[:,0],'Gender':array[:,1]})</br>
print("dataset setelah dinormalisasi :")</br>
print(dataset.head(10))
</summary><table align="justify"><i>Output : </i></br>
<tr><td colspan="6" align="center"> dataset sebelum dinormalisasi :</td></tr>
  <tr><td></td><td>Age</td><td> Customer ID </td><td> Gender</td><td> Income </td><td>Spending Score</td></tr>
<tr><td>0 </td><td> 19  </td><td>         1 </td><td>   Male </td><td>    15 </td><td>            39</td></tr>
<tr><td>1 </td><td> 21  </td><td>         2 </td><td>   Male </td><td>    15  </td><td>           81</td></tr>
<tr><td>2 </td><td> 20  </td><td>         3 </td><td> Female </td><td>    16   </td><td>           6</td></tr>
<tr><td>3 </td><td> 23  </td><td>         4 </td><td> Female </td><td>    16   </td><td>          77</td></tr>
<tr><td>4 </td><td> 31  </td><td>         5 </td><td> Female </td><td>    17   </td><td>          40</td></tr>
<tr><td>5 </td><td> 22  </td><td>         6 </td><td> Female </td><td>    17   </td><td>          76</td></tr>
<tr><td>6 </td><td> 35   </td><td>        7 </td><td> Female </td><td>    18   </td><td>           6</td></tr>
<tr><td>7 </td><td> 23  </td><td>         8 </td><td> Female </td><td>    18   </td><td>          94</td></tr>
<tr><td>8 </td><td> 64  </td><td>         9 </td><td>   Male </td><td>    19   </td><td>           3</td></tr>
<tr><td>9 </td><td> 30  </td><td>        10 </td><td> Female </td><td>    19   </td><td>          72</td></tr></table></br><table>
<tr><td colspan="6" align="center"> dataset setelah dinormalisasi :</td></tr> 
 <tr><td>  </td><td>     Age</td><td> Customer ID </td><td> Gender </td><td>   Income </td><td> Spending Score</td></tr>
<tr><td>0 </td><td> 0.019231 </td><td>          1 </td><td>   Male </td><td> 0.000000  </td><td>      0.387755</td></tr>
<tr><td>1 </td><td> 0.057692  </td><td>         2  </td><td>  Male</td><td>  0.000000  </td><td>      0.816327</td></tr>
<tr><td>2 </td><td> 0.038462  </td><td>         3  </td><td>Female </td><td> 0.008197  </td><td>      0.051020</td></tr>
<tr><td>3 </td><td> 0.096154  </td><td>         4 </td><td> Female </td><td> 0.008197  </td><td>      0.775510</td></tr>
<tr><td>4 </td><td> 0.250000  </td><td>         5 </td><td> Female </td><td> 0.016393  </td><td>      0.397959</td></tr>
<tr><td>5 </td><td> 0.076923  </td><td>         6 </td><td> Female </td><td> 0.016393  </td><td>      0.765306</td></tr>
<tr><td>6 </td><td> 0.326923   </td><td>        7 </td><td> Female </td><td> 0.024590  </td><td>      0.051020</td></tr>
<tr><td>7 </td><td> 0.096154  </td><td>         8 </td><td> Female </td><td> 0.024590  </td><td>      0.948980</td></tr>
<tr><td>8 </td><td> 0.884615  </td><td>         9 </td><td>   Male </td><td> 0.032787  </td><td>      0.020408</td></tr>
<tr><td>9</td><td>  0.230769  </td><td>        10 </td><td> Female </td><td> 0.032787  </td><td>      0.724490</td></tr>
</table></details> 
</br></br></br>
<p align="center"><b>E-Sertifikat Data Wragling Python DQLab</b></br><img src="https://github.com/yenysyafitry/Data-Wrangling-Python/blob/main/e-sertifikat.jpg"></p>
