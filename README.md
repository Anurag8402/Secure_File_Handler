# 🔒 Secure File Hider - Java Desktop App

A Java-based application to securely hide, encrypt, and manage files using email-based OTP authentication.
![image](https://github.com/user-attachments/assets/5fced007-74a8-4a7d-9e2c-05d1931f7859)


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

---

## 📂 Project Structure
```
SecureFileHider/
├── src/
│   └── in/ay/
│       ├── AuthService.java
│       ├── EncryptionUtils.java
│       ├── FileService.java
│       └── MainApp.java
├── lib/
│   └── mail.jar
└── db/
    └── secure_file_hider.sql
```

---

## 🧪 Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/Anurag8402/secure-file-hider.git
   ```
2. Import into Eclipse as a Java Project
3. Create MySQL database and tables:
   ```sql
   CREATE DATABASE secure_files;

   CREATE TABLE users (
       id INT AUTO_INCREMENT PRIMARY KEY,
       email VARCHAR(100),
       otp VARCHAR(10)
   );

   CREATE TABLE files (
       id INT AUTO_INCREMENT PRIMARY KEY,
       user_id INT,
       filename VARCHAR(200),
       filepath TEXT,
       is_hidden BOOLEAN,
       FOREIGN KEY (user_id) REFERENCES users(id)
   );
   ```
   
4. Configure email credentials and DB details in the code
5. Run `MainApp.java` to start the application

---

## 📸 Screenshots
![Screenshot 2025-06-24 225121](https://github.com/user-attachments/assets/d6f73c30-1289-47d9-b9c1-29f795544f12)


---

## 👨‍💻 Author
**Anurag Yadav**  
[GitHub Profile](https://github.com/Anurag8402)

---

## 📄 License
This project is licensed under the MIT License.
