# 1. PENJELASAN ARRAY DAN SCRENSHOOT HASIL EKSEKUSI
<img width="195" height="66" alt="image" src="https://github.com/user-attachments/assets/334f57ca-ad53-4bbf-a007-367c6bff9db3" />

1. list = [] di Python berarti membuat sebuah list kosong.
List di Python sering dianggap seperti array di bahasa pemrograman lain.
2. list → nama variabel yang digunakan untuk menyimpan data.
[] → tanda kurung siku yang menandakan list/array.
3. Karena tidak ada isi di dalamnya, maka list tersebut kosong.

<img width="626" height="413" alt="image" src="https://github.com/user-attachments/assets/3b9b3aa4-9bd7-46e5-a842-7fa497feea8e" />

1. Program meminta nilai mahasiswa sebanyak 10 kali.
2. Setiap nilai yang dimasukkan akan disimpan ke dalam array nilai_mahasiswa.
3. Fungsi append() digunakan untuk menambahkan nilai ke dalam array.

<img width="515" height="266" alt="image" src="https://github.com/user-attachments/assets/81529a72-931b-4c9e-9d68-19e2976521e7" />

1. print("List:", nilai_mahasiswa)
Menampilkan semua isi array nilai_mahasiswa.
Jadi akan terlihat kumpulan nilai mahasiswa yang sudah dimasukkan.

2. print("Nilai tertinggi:", max(nilai_mahasiswa))
max() digunakan untuk mencari nilai paling besar yang ada di dalam array nilai_mahasiswa.

3. print("Nilai terendah:", min(nilai_mahasiswa))
min() digunakan untuk mencari nilai paling kecil yang ada di dalam array nilai_mahasiswa.
<img width="684" height="156" alt="image" src="https://github.com/user-attachments/assets/7bcad36a-18a1-46d6-9a70-6390266b0cf2" />

1. print("Rata-rata:", sum(nilai_mahasiswa) / len(nilai_mahasiswa))
2. sum(nilai_mahasiswa)
Digunakan untuk menjumlahkan semua nilai yang ada di dalam array nilai_mahasiswa.
3. len(nilai_mahasiswa)
Digunakan untuk menghitung jumlah data yang ada di dalam array nilai_mahasiswa.
4. sum(nilai_mahasiswa) / len(nilai_mahasiswa)
Total nilai dibagi jumlah data untuk mendapatkan rata-rata.

<img width="479" height="434" alt="image" src="https://github.com/user-attachments/assets/1d567090-8653-498d-b36b-c7913edfd1ad" />

1. Array yang digunakan pada program ini adalah nilai_mahasiswa, yaitu tempat untuk menyimpan kumpulan nilai mahasiswa.
2. Program pertama membuat dua variabel yaitu lulus dan tidak_lulus yang digunakan untuk menghitung jumlah mahasiswa yang lulus dan tidak lulus.
3. Kemudian program melakukan perulangan pada array nilai_mahasiswa. Artinya program akan mengambil setiap nilai yang ada di dalam array tersebut satu per satu.
4. Jika nilai mahasiswa lebih dari atau sama dengan 60, maka mahasiswa dianggap lulus, sehingga jumlah lulus akan bertambah satu.
5. Jika nilai mahasiswa kurang dari 60, maka mahasiswa dianggap tidak lulus, sehingga jumlah tidak_lulus akan bertambah satu.
6. Setelah semua nilai di dalam array diperiksa, program akan menampilkan jumlah mahasiswa yang lulus dan jumlah mahasiswa yang tidak lulus berdasarkan data yang ada di dalam array nilai_mahasiswa.
<img width="720" height="817" alt="image" src="https://github.com/user-attachments/assets/3b33044f-9fdc-4a94-9aec-04d746c10f88" />

1. Pada program ini array (list) digunakan untuk menyimpan data yang akan ditampilkan dalam grafik.
2. Array pertama adalah kategori. Array ini berisi teks “Lulus” dan “Tidak Lulus” yang digunakan sebagai nama kategori pada grafik.
3. Array kedua adalah data. Array ini berisi dua nilai yaitu jumlah mahasiswa yang lulus dan jumlah mahasiswa yang tidak lulus. Nilai ini diambil dari variabel lulus dan tidak_lulus yang sudah dihitung sebelumnya.
4. Program kemudian membuat grafik batang (bar chart).
Array kategori digunakan sebagai label pada sumbu bawah (x), sedangkan array data digunakan sebagai tinggi batang grafik yang menunjukkan jumlah mahasiswa.
5. Setelah itu program memberi judul grafik “Grafik Data Kelulusan Mahasiswa”, memberi keterangan jumlah mahasiswa pada sumbu y, mengatur batas maksimal jumlah sampai 10, lalu menampilkan grafik.
6. Jadi, array pada program ini berfungsi untuk menyimpan kategori dan jumlah data yang akan ditampilkan dalam grafik kelulusan mahasiswa.

<img width="780" height="841" alt="image" src="https://github.com/user-attachments/assets/51d7d3e5-fd69-4be6-9f4a-ac1d88cb171b" />

1. Pada program ini array (list) digunakan untuk menyimpan kategori dan nilai yang akan ditampilkan dalam grafik.
2. Array pertama adalah kategori. Array ini berisi dua teks yaitu “Tertinggi” dan “Terendah”. Fungsinya sebagai nama kategori pada grafik batang.
3. Kemudian program mencari nilai dari array nilai_mahasiswa:
a. nilai_tertinggi diambil dari nilai paling besar dalam array nilai_mahasiswa menggunakan fungsi max().
b. nilai_terendah diambil dari nilai paling kecil dalam array nilai_mahasiswa menggunakan fungsi min().
4. Setelah itu dibuat array data, yang berisi nilai tertinggi dan nilai terendah tersebut.
5. Saat grafik dibuat:
a. Array kategori digunakan sebagai label pada sumbu X (nama batang grafik).
b. Array data digunakan sebagai tinggi batang grafik yang menunjukkan besar nilainya.
6. Jadi, array pada program ini berfungsi untuk menyimpan kategori dan nilai yang akan ditampilkan dalam grafik nilai tertinggi dan terendah mahasiswa. 

# 2. Analisis kompleksitas tiap operasi
1. Input 10 nilai mahasiswa → O(10) ≈ O(1)
Program meminta input nilai sebanyak 10 kali. Karena jumlahnya tetap (tidak berubah), maka dianggap O(1) atau konstan.

2. Mencari nilai tertinggi dan terendah → O(n)
Untuk mencari nilai tertinggi dan terendah, program harus memeriksa semua nilai dalam array nilai_mahasiswa satu per satu.
Jika jumlah data n, maka prosesnya n kali, sehingga kompleksitasnya O(n).

3. Menghitung rata-rata → O(n)
Untuk menghitung rata-rata, program harus menjumlahkan semua nilai dalam array terlebih dahulu, lalu dibagi jumlah data.
Karena semua data diperiksa, kompleksitasnya O(n).

4. Menghitung jumlah mahasiswa lulus → O(n)
Program melakukan perulangan pada seluruh isi array nilai_mahasiswa untuk mengecek apakah nilai ≥ 60 atau tidak.
Karena setiap data diperiksa satu per satu, kompleksitasnya juga O(n).

5. Membuat grafik → O(1)
Grafik hanya menggunakan 2 data atau data yang sangat sedikit, sehingga waktu prosesnya konstan dan dianggap O(1).

# 3. REFLEKSI PEMBELAJARAN
Apa yang saya pelajari dari kode ini?

Pemahaman struktur data list (array) sangat penting untuk mengelola kumpulan data seperti nilai mahasiswa. List membuat data terorganisir dan mudah diproses.

Operasi dasar pada list seperti penambahan data (append), pencarian nilai terendah/tertinggi (max, min), dan penghitungan total (sum) memperlihatkan bagaimana Python memudahkan manipulasi data.

Penggunaan loop (for) memungkinkan kita mengakses dan memproses setiap elemen data secara efisien, misalnya untuk menghitung berapa mahasiswa yang lulus.

Analisis kompleksitas mengajarkan bahwa meskipun operasi kita sederhana, penting untuk memahami berapa lama waktu yang dibutuhkan operasi terhadap data yang bertambah besar (meskipun di kasus ini jumlah datanya kecil dan tetap).

Visualisasi data dengan grafik membuat hasil pengolahan data lebih mudah dipahami dan menarik, terutama saat menyajikan hasil ke orang lain.
