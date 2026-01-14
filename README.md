# End-to-End Encrypted File Sharing System (E2EE)

A secure, client-side encrypted file storage and sharing system using **Flask (backend)** and **Web Crypto API (frontend)**.  
All encryption and decryption happens **in the browser**. The server never sees plaintext files or private keys.

---

## 📁 Project Structure

```text
c:\Users\himan\Downloads\E2EE\
├── backend/
│   ├── app.py                 # Flask application entry point
│   ├── config.py              # Configuration settings
│   ├── models.py              # SQLite database models
│   ├── routes/
│   │   ├── __init__.py
│   │   ├── auth.py            # Authentication endpoints
│   │   ├── files.py           # File upload/download endpoints
│   │   └── sharing.py         # File sharing endpoints
│   ├── utils/
│   │   ├── __init__.py
│   │   └── security.py        # Server-side security utilities
│   └── requirements.txt
├── frontend/
│   ├── index.html             # Main entry point
│   ├── css/
│   │   └── styles.css         # Global styles with design system
│   └── js/
│       ├── app.js             # Main application logic
│       ├── crypto.js          # Client-side cryptography (Web Crypto API)
│       ├── auth.js            # Authentication logic
│       ├── files.js           # File upload/download logic
│       └── ui.js              # UI components and feedback
└── secure_files.db            # SQLite database (created at runtime)
