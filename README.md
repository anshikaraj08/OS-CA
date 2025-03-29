# OS-CA

# Secure File Management System

## 📌 Overview
This project is a **Secure File Management System** that provides robust security measures such as:
- **Authentication**: Password-based login with **Two-Factor Authentication (2FA)** using Google Authenticator.
- **File Protection**: Encryption using AES (Fernet) encryption.
- **Threat Detection**: Identifies potentially malicious files (e.g., executables, large files).
- **Access Control**: Users can securely upload, delete, and view file metadata.

## 🚀 Features
- **User Authentication**: Secure password storage (SHA-256) with OTP verification.
- **2FA using TOTP**: Time-based One-Time Passwords (TOTP) for enhanced security.
- **File Encryption**: AES encryption ensures data security at rest.
- **Threat Detection**: Detects large or potentially harmful files.
- **File Operations**:
  - Upload & Encrypt files.
  - Delete files securely.
  - View metadata (size, modification time, creation time).
- **Account Reset**: Reset accounts if OTP secret is lost.

## 🛠️ Setup & Installation
### Prerequisites
- Python 3.x
- Required Python Libraries:
  ```bash
  pip install cryptography pyotp
  ```

### Running the Program
1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/secure-file-management.git
   cd secure-file-management
   ```
2. **Run the Program**
   ```bash
   python secure_file_manager.py
   ```

## 🔑 How to Use
### 1️⃣ Register a User
Run the script and choose **Register**. It will generate a secret key for **Google Authenticator**.

### 2️⃣ Setup Google Authenticator
- Install **Google Authenticator** (Android/iOS).
- Add a new account using the **secret key** from the registration step.
- This will generate **time-based OTPs** for logging in.

### 3️⃣ Login with 2FA
- Enter your username and password.
- Input the OTP from Google Authenticator.
- Access file management features.

### 4️⃣ Manage Files Securely
- **Upload** a file → It gets encrypted automatically.
- **List** all your files.
- **Delete** a file securely.
- **View metadata** of a file (size, last modified, creation date).
- **Detect threats** before uploading files.

## 🛡️ Security Measures
- **AES Encryption**: Encrypts files before storage.
- **2FA with OTP**: Ensures only authorized users access files.
- **Threat Detection**: Flags executable and large files.
