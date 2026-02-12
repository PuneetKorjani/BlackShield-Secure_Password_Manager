# BlackShield-Secure_Password_Manager
BlackShield is a secure, local-first password manager built in Python, featuring AES-256 encryption, TOTP-based two-factor authentication, auto-lock protection, and a modern GUI interface.
# 🛡 BlackShield

**BlackShield** is a secure, desktop-based password manager built with Python and Tkinter.  
It provides encrypted local credential storage, master password protection, Two-Factor Authentication (2FA), automatic session locking, and a secure password generator.

BlackShield is designed as a security-focused application demonstrating encryption, authentication, and secure session management principles.

---

## 🚀 Features

- 🔐 Master password authentication
- 🛡 AES-256 encrypted vault storage
- 📱 TOTP-based Two-Factor Authentication (Google Authenticator compatible)
- ⏳ Automatic inactivity auto-lock system
- 🔑 Cryptographically secure password generator (Python `secrets` module)
- 📊 Password strength analyzer
- 🖥 Modern Tkinter-based graphical interface
- 📁 Fully local encrypted storage (no cloud dependency)

---

## 🛡 Security Architecture

BlackShield follows a secure design model:

- The master password is never stored directly.
- A secure key derivation function generates an encryption key.
- Vault data is encrypted before being saved to disk.
- The same password regenerates the same key for decryption during login.
- TOTP-based 2FA adds an additional authentication layer.
- Auto-lock protects the vault during inactivity.

---

## 📂 Project Structure





blackshield/
├── main.py # Application entry point
├── app.py # App controller
├── auth.py # Master password & authentication logic
├── encryptor.py # Encryption & key derivation logic
├── vault.py # Vault operations
├── totp.py # TOTP-based 2FA implementation
│
├── gui/
│ ├── screens/
│ │ ├── welcome.py
│ │ ├── login.py
│ │ ├── register.py
│ │ └── vault.py
│
├── assets/ # QR code images & UI assets
├── data/ # Encrypted vault storage (excluded from version control)
├── LICENSE
└── README.md


---

## ⚙️ Installation

### Requirements

- Python 3.8+
- pip

### Install Dependencies

```bash
pip install -r requirements.txt
python main.py

🔐 How It Works

Registration

User sets a master password

A key is derived using a secure key derivation function

A TOTP secret is generated for 2FA setup

Vault encryption key is created

Login

Master password is entered

Encryption key is regenerated

Encrypted vault file is decrypted

2FA verification is required

Vault unlocks upon successful authentication


🎯 Educational Purpose

BlackShield demonstrates:

Practical encryption implementation

Secure credential storage concepts

Two-factor authentication integration

Secure session timeout handling

GUI-based security application design

📜 License

This project is licensed under the MIT License.

BlackShield is an extended and enhanced version of an MIT-licensed open-source vault application, redesigned with additional security features and UI improvements.
