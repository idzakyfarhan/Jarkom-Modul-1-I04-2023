# Jarkom-Modul-1-I04-2023
## **Lapres Praktikum Jarkom Modul 1 Kelompok I-04**

|Muhammad Dzaky Farhan       |5025211069|
|Satria Surya Prana          |5025211...|

## **Number 1**
**The user is performing various activities using the FTP protocol. One of them is uploading a file..**

**Solution :**

Since the user wants to perform activities using the FTP (File Transfer Protocol) protocol, we will filter based on the FTP protocol only. After applying the filter, we will search for message info with the STOR command followed by the filename (because the user wants to upload a file).

-----------

#### A. What is the raw sequence number in the packet that indicates this activity?

As seen in the above image, the raw sequence number in frame number 147 is **258040667**.

#### B. What is the raw acknowledge number in the packet that indicates this activity?

Based on the above image, the raw acknowledge number in frame number 147 is **1044861039**.

To view the response from the STOR activity, we just need to search for the message info with the uploaded file's name. In this case, the response is shown in frame number 149.

#### C. What is the raw sequence number in the packet that indicates the response to this activity?

As seen in the above image, the raw sequence number in frame number 149 is **1044861039**, which is the same as the raw acknowledge number in frame number 147.

#### D. What is the raw acknowledge number in the packet that indicates the response to this activity?

Based on the above image, the raw acknowledge number in frame number 149 is **258040696**.

## **Number 6**
**Seorang anak bernama Udin Berteman dengan SlameT yang merupakan seorang penggemar film detektif. sebagai teman yang baik, Ia selalu mengajak slamet untuk bermain valoranT bersama. suatu malam, terjadi sebuah hal yang tak terdUga. ketika udin mereka membuka game tersebut, laptop udin menunjukkan sebuah field text dan Sebuah kode Invalid bertuliskan "server SOURCE ADDRESS 7812 is invalid". ketika ditelusuri di google, hasil pencarian hanya menampilkan a1 e5 u21. jiwa detektif slamet pun bergejolak. bantulah udin dan slamet untuk menemukan solusi kode error tersebut.**

**Solution :**

In the package number 7812 the source address is 104.18.14.101. By using the hint on the question that hinted a1 e5 u21 it shows an alphabet, therefore what we need to do is to change the ip address given on the package number 7812 into alphabet. Then we get 10 = J, 4 = D, 18 = R, 14 = N, 10 = J, 1 = A, So the answer that we looking for is **JDRNJA**

## **Number 7**
**How many package that go to IP 184.87.193.88?**

**Solution :**

To find the package that go to IP 184.87.193.88 we can type on the filter bar **ip.dst == 184.87.193.88** Then it will shows how many package that goes into IP 184.87.193.88, Therefore **there will be 6 package**.

## **Number 8**

**Provide a filter query so that Wireshark only captures all protocol packets destined for port 80! (If there are multiple ports, then sort them alphabetically)**

## **Number 9**
**Provide a filter query so that Wireshark only captures packets originating from the address 10.51.40.1 but not destined for the address 10.39.55.34!**

**Solution :**
The query filter is : ```ip.src == 10.51.40.1 && ip.dst != 10.39.55.34```











