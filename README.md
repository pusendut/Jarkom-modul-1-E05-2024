# Jarkom-modul-1-E05-2024

### Kelompok E05:
- Azhar Abiyu Rasendriya H. / 5025211177
- Daffa Diandra Rizky Aghnia / 5025221261

# No. 1
### Soal 
a. Berapa banyak packet yang terekam pada file pcapng?

b. Ada berapa jenis protocol yang terekam pada traffic?

c. sebutkan secara berurutan berdasarkan alfabet menurun dengan koma sebagai separator dan dalam bentuk uppercase, contoh: PROTOCOL1,PROTOCOL2

### Penyelesaian
a. Untuk mengetahui berapa banyak packet yang terekam pada file pcapng dapat dilihat pada tulisan `Packets:` pada bawah window wireshark.
![](images/1a.png)  
Namun untuk mendapatkan packet yang secara spesifik hanya bisa dikirim dengan FTP, dapat menggunakan display filter `ftp contains "STOR"` karena command STOR hanya bisa dilakukan melalui FTP  
![](images/1b.png)  
Setelah packet didapatkan, tinggal dilihat sequence number (raw) dan acknowledgement number (raw) dengan membuka section Transmission Control Protocol seperti berikut:  
![](images/1c.png)  
Untuk mendapatkan packet response, display filter yang digunakan adalah `ftp contains "zip"` karena command STOR digunakan untuk upload file zip.  
![](images/1d.png)  

### Perolehan flag:  
![](images/1e.png)  
