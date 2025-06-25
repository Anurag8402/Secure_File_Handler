# 🔒 Secure File Hider - Java Desktop App

A Java-based application to securely hide, encrypt, and manage files using email-based OTP authentication.



---

## 🔐 Features
- User authentication using email and OTP
- Secure OTP transmission using JavaMail API
- File hiding and unhiding
- Encryption and decryption of sensitive files
- MySQL database for user and file metadata

---

## 🛠️ Technologies Used
- Java (Swing, Core Java)
- MySQL
- JDBC
- JavaMail API
- Eclipse IDE



## 🧪 Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/Anurag8402/secure-file-hider.git
   ```
2. Import into Eclipse as a Java Project
3. Create MySQL database and tables:
   ```sql
   CREATE DATABASE secure_file;

   CREATE TABLE users (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name varchar(100),
       email VARCHAR(100),
       path varchar(100)
   );

   CREATE TABLE data (
       id INT AUTO_INCREMENT PRIMARY KEY,
       filepath TEXT,
       bin_data Blob
   );
   ```
   
4. Configure email credentials and DB details in the code
5. Run `MainApp.java` to start the application

---

## 📸 Screenshots
![Screenshot 2025-06-24 225121](https://github.com/user-attachments/assets/d6f73c30-1289-47d9-b9c1-29f795544f12)
![image](https://github.com/user-attachments/assets/2877257e-7d2b-48e6-8916-15f32a93db22)



---

## 👨‍💻 Author
**Anurag Yadav**  
[GitHub Profile](https://github.com/Anurag8402)

---

## 📄 License
This project is licensed under the MIT License.
