# Remote Instance with SSH putty

1. Pastikan sudah install Putty 

![alt text](image-13.png)

2. Konversi file Public Key dari .pem menjadi .ppk di putty
 - buka puttyGen
 - load File .pem
 - Save as .ppk

![alt text](image-14.png)

3. Set Up Putty untuk Remote SSH
 - buka apps Putty
 - Isi IP Public sesuai instance
 - isi Port untuk SSH sesuai Security Group di Instance
 - isi Nama session agar saat connect lagi tinggal load saja
 - load file .ppk (Klik SSH-> Auth -> Credentials ->load file .ppk)
 - Kembali ke Session klik Save
 - Klik Open
 - Masukan username sesuai instance

![alt text](image-15.png)

![alt text](image-16.png)
![alt text](image-17.png)

4. "Sudo apt-get Update" (Update OS) lanjut "sudo apt-get Upgrade"

![alt text](image-18.png)

5. Pembuktian Remote SSH secara visual
 - Copy public IP Address instance paste ke Browser
 ![alt text](image-19.png)
 - Install Web Server seperti Apache/Nginx 
 - sudo apt install apache2
 - Reload Browser
 ![alt text](image-20.png)

6. Matikan Instance agar tidak kena tagihan
 - sudo shutdown now 
 ![alt text](image-21.png)