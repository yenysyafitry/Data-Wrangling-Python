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
<tr><td></td><td>CustomerID </td><td>Genre</td><td>Age</td><td>Annual Income(k$)</td> <td>Spending Score (1-100)</td></tr>
<tr><td>0</td><td>1</td><td>Male</td><td>19</td><td>15</td><td>39</td></tr>
<tr><td>1</td><td>2</td><td>Male </td><td>21</td><td>15</td><td>81</td></tr>
<tr><td>2</td><td>3</td><td>Female </td><td>20</td><td>16 </td><td>6</td></tr>
<tr><td>3</td><td>4</td><td>Female </td><td>23</td><td>16 </td><td>77</td></tr>
<</br>
  </table></details>

<details> <summary><b>Melakukan akses data kolom</b></br>Pertama yang harus dilakukan untuk melakukan akses kolom adalah mengetahui nama-nama kolom yang ada. Coba ketikkan kode di bawah ini untuk melihat nama kolom yang ada :</br></br><i>import pandas as pd</br>
csv_data = pd.read_csv("https://storage.googleapis.com/dqlab-dataset/shopping_data.csv")</br>
print(csv_data['Age'])</i>
</summary><table align="justify"><i>Output : </br></i>
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
<tr><td>199 </td><td>   30</td></tr>
Name: Age, Length: 200, dtype: int64
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
