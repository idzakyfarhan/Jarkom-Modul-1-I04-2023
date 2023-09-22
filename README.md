# Jarkom-Modul-1-I04-2023
## **Lapres Praktikum Jarkom Modul 1 Kelompok I-04**

|Muhammad Dzaky Farhan       |5025211069|
|Satria Surya Prana          |5025211...|

## **Nomor 1**
**The user is performing various activities using the FTP protocol. One of them is uploading a file..**

**Solustion :**

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

