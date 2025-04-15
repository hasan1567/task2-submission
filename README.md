# Task 2 – Securing a Node.js Web Application

## 🔐 Objective
To implement basic web security measures in a mock Node.js user management system by applying industry best practices.

## 🧪 Environment
- Kali Linux (VMware)
- Node.js v20.19.0
- Express.js
- Terminal + curl for testing

## 🛠️ Tools & Libraries Used
- **Express.js** – Web server
- **validator.js** – Input validation
- **bcrypt** – Password hashing
- **jsonwebtoken** – Token-based authentication
- **helmet** – HTTP security headers

## ✅ Security Features Implemented

### 1. **Input Validation**
- Validates email input using `validator.isEmail()`
- Rejects invalid or unsafe input formats

### 2. **Password Hashing**
- Uses `bcrypt` to hash passwords before storing or comparing
- Prevents raw passwords from being leaked

### 3. **JWT Authentication**
- Generates secure token on login with 1-hour expiry
- Used `jsonwebtoken` to sign and verify payloads

### 4. **Secure Headers**
- Integrated `helmet` middleware to add security headers
- Helps prevent XSS, clickjacking, and other attacks

## 🧪 Testing & Verification
- `curl` commands used to POST test email and password
- JWT returned in response on successful login
- Invalid email input returns proper error
- Verified headers via `curl -I` (Helmet)

## 📂 Files Included
- `index.js` – Main application logic
- `task2_report.txt` – Task summary and implementation steps
- Screenshots – Terminal outputs, code setup, curl responses

## 📌 Conclusion
Successfully secured a simple web app using key practices:
- Input validation
- Hashing
- Auth tokens
- Secure headers
All features tested and verified in a controlled Kali Linux environment.

---
