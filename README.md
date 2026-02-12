BlackShield – Secure Password Manager

BlackShield is a secure, desktop-based password manager built with Python and Tkinter.
It provides encrypted local credential storage, master password protection, Two-Factor Authentication (2FA), automatic session locking, and a secure password generator.

BlackShield is designed as a security-focused application demonstrating encryption, authentication, and secure session management principles.

🚀 Features

🔐 Master password authentication

🛡 AES-256 encrypted vault storage

📱 TOTP-based Two-Factor Authentication (Google Authenticator compatible)

⏳ Automatic inactivity auto-lock system

🔑 Cryptographically secure password generator (Python secrets module)

📊 Password strength analyzer

🖥 Modern Tkinter-based graphical interface

📁 Fully local encrypted storage (no cloud dependency)

---

🛡 Security Architecture

BlackShield follows a secure design model:

The master password is never stored directly.

A secure key derivation function generates an encryption key.

Vault data is encrypted before being saved to disk.

The same password regenerates the same key for decryption during login.

TOTP-based 2FA adds an additional authentication layer.

Auto-lock protects the vault during inactivity.

---



