# PPL-SQL
Tugas 1 MK PPL TIF RP 17 CID B Kelompok 2:
  * Andri Ilham (17111322)
  * Hesty Sugesty (17111328)
  * Ikhsan Alfath (17111050)
  * Siti Muayanah (17111139)
  
  Dalam tugas ini kami membuat sebuah database barang dengan nama db_barang menggunakan mySQL.
  
 ## Perintah Tugas
  * Create Table
  * Insert
  * Select

### Code!
* Membuat Table
  
  Sebelum membuat tabel, terlebih dahulu untuk membuat database, kemudian menggunakan database tersebut. Perhatikan query berikut:
  ```
  CREATE DATABASE db_barang;
  USE db_barang;
  ```
  Membuat tb_barang menggunakan query berikut
  ```
  CREATE TABLE tb_barang ( 
  id_barang INT(11) NOT NULL AUTO_INCREMENT , 
  nama_barang VARCHAR(50) NOT NULL , 
  stok INT(11) NOT NULL , 
  harga INT(11) NOT NULL , 
  PRIMARY KEY (id_barang));
  ```
  Dari query diatas, maka dihasilkan tabel sbb:
  ```
  +=============+=================================+
  | coloumn     | type                            |
  +=============+=================================+
  | id_barang   | int(11)                         |
  +-------------+---------------------------------+
  | nama_barang | varchar(50) utf8mb4_general_ci  |
  +-------------+---------------------------------+
  | stok        | int(11)                         |
  +-------------+---------------------------------+
  | harga       | int(11)                         |
  +-------------+---------------------------------+
  ```
  
* Insert
  Memasukkan data kedalam tabel
  ```
  INSERT INTO `tb_barang` (`id_barang`, `nama_barang`, `stok`, `harga`) VALUES 
  (NULL, 'Aqua Gelas', '75', '500'), 
  (NULL, 'Teh Pucuk', '30', '3500');
  ```
  
* Select/
  Query SELECT dalam mySQL merupakan query untuk menampilkan data yang ada pada tabel
  ```
  SELECT * FROM tb_barang
  ```
  Dari query diatas akan ditampilkan data yang baru kita masukkan kedalam tabel tb_barang seperti berikut
  ```
  +===========+=============+======+=======+
  | id_barang | nama_barang | stok | harga |
  +===========+=============+======+=======+
  | 1         | Aqua Gelas  | 75   | 500   |
  +-----------+-------------+------+-------+
  | 2         | Teh Pucuk   | 30   | 3500  |
  +-----------+-------------+------+-------+
  ```


END
