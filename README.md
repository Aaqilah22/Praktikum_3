# Praktikum3
## 1. Membuat Class Pegawai
![Kelas Pegawai](https://github.com/user-attachments/assets/9dfbcdc1-db53-45bc-a949-1f78c5bcadd4)

Penjelasan:
a. Atribut :
- nama (tipe String): Untuk menyimpan nama pegawai.
- gajiPokok (tipe double): Untuk menyimpan gaji pokok pegawai
b. Setter dan Getter :
- setNama(String nama): Method ini digunakan untuk memberikan nilai pada atribut nama.
- getNama(): Method ini mengembalikan nilai dari atribut nama.
- setGajiPokok(double gajiPokok): Method ini digunakan untuk memberikan nilai pada atribut gajiPokok.
- getGajiPokok(): Method ini mengembalikan nilai dari atribut gajiPokok.
c. Method cetakInfo() :
Adalah method untuk mencetak informasi pegawai, seperti nama dan gaji pokok. Method ini tidak menerima parameter dan tidak mengembalikan nilai (void).

## 2. Membuat Kelas Manager
![Kelas Manager](https://github.com/user-attachments/assets/363af9ac-c3aa-4d8e-ad10-354db43e3965)

Penjelasan :
a. Atribut :
tunjangan (tipe double): Atribut tambahan untuk menyimpan tunjangan yang diterima oleh seorang manager.
b. Setter dan Getter :
- setTunjangan(double tunjangan): Method ini digunakan untuk memberikan nilai pada atribut tunjangan.
- getTunjangan(): Method ini mengembalikan nilai dari atribut tunjangan.
c. Method cetakTunjangan() :
Method ini khusus untuk mencetak nilai tunjangan seorang manager. Berbeda dengan cetakInfo(), method ini hanya fokus pada tunjangan saja.
d. Override Method cetakInfo() :
Di kelas Manager, method cetakInfo() di-override (diganti) untuk menampilkan informasi tambahan, yaitu tunjangan. Method super.cetakInfo() digunakan untuk memanggil cetakInfo() dari kelas Pegawai dan kemudian ditambah dengan informasi tunjangan.

## 3. Membuat Kelas Programmer
![Kelas Programmer](https://github.com/user-attachments/assets/2f1a4728-0897-4e3a-a325-f5d733fbf429)

Penjelasan :
*Atribut :*
bonus (tipe double): Atribut tambahan yang digunakan untuk menyimpan bonus yang diterima oleh programmer.
*Setter dan Getter :*
- setBonus(double bonus): Method ini digunakan untuk memberikan nilai pada atribut bonus.
- getBonus(): Method ini mengembalikan nilai dari atribut bonus.
*Method cetakBonus() :*
Method ini khusus digunakan untuk mencetak nilai bonus seorang programmer.
*Override Method cetakInfo() :*
Sama seperti pada kelas Manager, method cetakInfo() di-override untuk menambahkan informasi tentang bonus di samping informasi pegawai standar. Method super.cetakInfo() digunakan untuk memanggil method dari kelas induk.

## 4. Membuat Kelas Main
![Kelas Main](https://github.com/user-attachments/assets/47ea8a38-6587-42f9-875a-51e915fba967)

Penjelasan :
- Pertama, kita membuat objek Manager bernama Budi dan mengatur gajiPokok serta tunjangan. Kemudian, method cetakInfo() akan mencetak semua informasi yang dimiliki oleh objek tersebut.
- Selanjutnya, kita membuat objek Programmer bernama Andi dan mengatur gajiPokok serta bonus. Sama seperti sebelumnya, method cetakInfo() akan mencetak informasi lengkap programmer.

## Out put
![Out put](https://github.com/user-attachments/assets/eec16604-8a4a-47ba-a910-4fe39b18282f)
