# Jarkom-Modul-1-I04-2023
## **Lapres Praktikum Jarkom Modul 1 Kelompok I-04**
### **I04**
|**Name**|**NRP**|
|--------|-------|
|Muhammad Dzaky Farhan       |5025211069|
|Satria Surya Prana          |5025211073|

## **Number 1**
**The user is performing various activities using the FTP protocol. One of them is uploading a file..**

**Solution :**

Since the user wants to perform activities using the FTP (File Transfer Protocol) protocol, we will filter based on the FTP protocol only. After applying the filter, we will search for message info with the STOR command followed by the filename (because the user wants to upload a file).

![1A,B](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Nomor%201ab.png)

#### A. What is the raw sequence number in the packet that indicates this activity?

As seen in the above image, the raw sequence number in frame number 147 is **258040667**.

#### B. What is the raw acknowledge number in the packet that indicates this activity?

Based on the above image, the raw acknowledge number in frame number 147 is **1044861039**.

To view the response from the STOR activity, we just need to search for the message info with the uploaded file's name. In this case, the response is shown in frame number 149.

#### C. What is the raw sequence number in the packet that indicates the response to this activity?


![1C,D](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/nomor%201cd.png)

As seen in the above image, the raw sequence number in frame number 149 is **1044861039**, which is the same as the raw acknowledge number in frame number 147.

#### D. What is the raw acknowledge number in the packet that indicates the response to this activity?

Based on the above image, the raw acknowledge number in frame number 149 is **258040696**.

## **Number 2**
**Sebutkan web server yang digunakan pada portal praktikum Jaringan Komputer!**

**Solution:**
to find out which server is used for the Jarkom website we look at the file in wireshark that has a protocol HTTP and we follow through the stream and we can see as stated on the image below that the server used in the website is "gunicorn"

![2](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2018.33.48.png)

## **Number 3**
**Dapin sedang belajar analisis jaringan. Bantulah Dapin untuk mengerjakan soal berikut:
a. Berapa banyak paket yang tercapture dengan IP source maupun destination address adalah 239.255.255.250 dengan port 3702?
b. Protokol layer transport apa yang digunakan?**

**Solution:**
to find the package that has been captured from source or destination from the IP of 239.255.255.250 and port 3702 we use the syntax of ip.src == 239.255.255.250||ip.dst==239.255.255.250 dan tcp.port==3702||udp.port==3702 and for point b we can see on the wireshark that it has the protocol of UDP

![3](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2018.46.49.png)

## **Number 4**
**Berapa nilai checksum yang didapat dari header pada paket nomor 130?**

**Solution:**
On the wireshark we can see the package number 130 and we can see the details and it has the checksum of 0x18e5

![4](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2018.51.22.png)

## **Number 5**
**Elshe menemukan suatu file packet capture yang menarik. Bantulah Elshe untuk menganalisis file packet capture tersebut.
a. Berapa banyak packet yang berhasil di capture dari file pcap tersebut?
b. Port berapakah pada server yang digunakan untuk service SMTP?
c. Dari semua alamat IP yang tercapture, IP berapakah yang merupakan public IP?**

**Solutions:**
To open the zip file on the website decoding is needed in Wireshark and has information about the password, and when followed it will show a password that has not been decoded and to decode it using the website from Base64 and you will get the password 5implepas5word.

![5](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2018.58.19.png)

and for point a we can get the total packets that is captured from the bottom right corner and it shows 60

![5a](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2019.02.47.png)

For point b we did a test where the required port was between 25 or 1470 and the correct one was 25

![5b](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2019.04.55.png)

For point c, the same logic is implemented on the IP used, there are only 2 IPs used and I tried 10.10.1.4 and 74.53.140.153 and the correct one is 74.53.140.153

![5c](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2019.07.09.png)

## **Number 6**
**Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.**

**Solution :**

![6](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/nomor%206.png)


In the package number 7812 the source address is 104.18.14.101. By using the hint on the question that hinted a1 e5 u21 it shows an alphabet, therefore what we need to do is to change the ip address given on the package number 7812 into alphabet. Then we get 10 = J, 4 = D, 18 = R, 14 = N, 10 = J, 1 = A, So the answer that we looking for is **JDRNJA**

## **Number 7**
**How many package that go to IP 184.87.193.88?**

**Solution :**
![7](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/nomor%207.png)


To find the package that go to IP 184.87.193.88 we can type on the filter bar **ip.dst == 184.87.193.88** Then it will shows how many package that goes into IP 184.87.193.88, Therefore **there will be 6 package**.

## **Number 8**

**Provide a filter query so that Wireshark only captures all protocol packets destined for port 80! (If there are multiple ports, then sort them alphabetically)**

![8](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/nomor%208.png)


## **Number 9**
**Provide a filter query so that Wireshark only captures packets originating from the address 10.51.40.1 but not destined for the address 10.39.55.34!**

**Solution :**
![9](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/nomor%209.png)

The query filter is : ```ip.src == 10.51.40.1 && ip.dst != 10.39.55.34```

## **Number 10**
**Sebutkan kredensial yang benar ketika user mencoba login menggunakan Telnet**

**Solution:**
For number 10, I followed the telnet file and got the login credentials and password as stated below.

![10](https://github.com/idzakyfarhan/Jarkom-Modul-1-I04-2023/blob/main/IMG/Screenshot%202023-09-22%20at%2019.10.50.png)









