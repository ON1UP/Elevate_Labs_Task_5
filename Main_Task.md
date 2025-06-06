### 🔐 Demonstration: Dangers of HTTP Using Packet Capture on `vulnweb.php`

**Objective:**  
To showcase the security risks of using HTTP by capturing and analyzing unencrypted login credentials transmitted over the network.

**Tools Used:**  
- Wireshark / Burp Suite  
- vulnweb.php test site

**Steps Performed:**
1. Navigated to the `http://testphp.vulnweb.com/login.php` page.
2. Logged in using test credentials:

   `username:- Dhruv_sablaok`
    `Password:- Elevate_Labs`
4. Captured the network traffic during the login attempt using Wireshark.
5. Located the HTTP POST request in the packet capture.
6. Observed the credentials being sent in **plain text**, revealing:
   `POST /login.php HTTP/1.1`  
   `Host: testphp.vulnweb.com`  
   `Content-Type: application/x-www-form-urlencoded`  
   `Content-Length: ...`  
   `uname=Dhruv_Sabloak&pass=Elevate_Labs&login=Login`
![image](https://github.com/user-attachments/assets/0b37b9dc-9e28-476d-b560-36ddeb9e9c64)


**🔎Conclusion:**  
This experiment clearly demonstrates how HTTP transmits sensitive data without encryption. Any attacker with access to the network (e.g., on public Wi-Fi) can intercept such data using packet sniffers. This emphasizes the **critical need for HTTPS** in all web applications handling user credentials or private data.

**✔️Recommendation:**  
Always use TLS/SSL (HTTPS) to encrypt sensitive transmissions and prevent data leakage or man-in-the-middle (MITM) attacks.
