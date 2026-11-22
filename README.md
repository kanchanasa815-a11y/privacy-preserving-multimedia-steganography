# Privacy-Preserving Multimedia Steganography

## 📌 Project Overview

Privacy-Preserving Multimedia Steganography is a web-based application developed using Python and Flask to securely hide confidential information inside multimedia files.

The system combines AES-128-GCM encryption and steganography techniques to protect sensitive data. It supports hiding and retrieving information in text, images, audio, and video files.

It also maintains operation records using a blockchain-based verification mechanism and stores user information securely in an SQLite database.

## 🎯 Objectives

- Protect sensitive information using encryption.
- Hide confidential data inside multimedia files.
- Support text, image, audio, and video steganography.
- Provide secure user registration and login.
- Maintain operation records using blockchain technology.
- Verify the integrity of blockchain records.
- Provide a simple web-based interface for users.

## ✨ Key Features

1. **Text Steganography** – Hide encrypted text inside an image using the Least Significant Bit (LSB) technique.
2. **Image Steganography** – Hide an encrypted image inside another image.
3. **Audio Steganography** – Hide encrypted audio data inside WAV audio files.
4. **Video Steganography** – Hide encrypted video data inside video files.
5. **AES Encryption** – Protect hidden data using AES-128-GCM encryption.
6. **User Authentication** – Register, log in, and manage user sessions.
7. **Blockchain Integration** – Maintain tamper-evident records of encryption operations.
8. **Admin Dashboard** – View user information, operation records, and failed login attempts.
9. **Blockchain Verification** – Check the integrity of stored blockchain records.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Backend programming |
| Flask | Web application framework |
| HTML | Web page structure |
| CSS | User interface styling |
| JavaScript | Frontend functionality |
| SQLite | Database management |
| AES-128-GCM | Data encryption |
| LSB | Steganography technique |
| Blockchain | Operation record verification |
| Pillow | Image processing |
| NumPy | Numerical and audio data processing |
| PyCryptodome | Cryptographic operations |

## 📂 Project Structure

```text
PRIVACY_PRESERVING/
│
├── app.py
├── blockchain.py
├── blockchain.json
├── crypto_utils.py
├── database.py
├── steganography.db
│
├── static/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── uploads/
│
└── templates/
    ├── admin.html
    ├── audio_steganography.html
    ├── base.html
    ├── blockchain_view.html
    ├── dashboard.html
    ├── image_steganography.html
    ├── index.html
    ├── login.html
    ├── register.html
    ├── text_steganography.html
    └── video_steganography.html
```

## ⚙️ Installation and Setup

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/privacy-preserving-multimedia-steganography.git
```

### Step 2: Open the Project Folder

```bash
cd privacy-preserving-multimedia-steganography
```

### Step 3: Install Required Libraries

```bash
pip install Flask numpy Pillow pycryptodome Werkzeug
```

**Additional requirement:** Install FFmpeg and add it to your system PATH if you want to use supported non-WAV audio formats.

### Step 4: Run the Application

```bash
python app.py
```

### Step 5: Open in Browser

```text
http://127.0.0.1:5000/
```

Register an account and log in to access the application.

## 🔐 Security Features

- AES-128-GCM encryption for confidentiality and authentication of hidden data.
- Password hashing for user authentication.
- Session-based access protection.
- SHA-256 hashing for blockchain records.
- Blockchain integrity verification.
- Logging of failed login attempts.

## 🔄 Working Process

1. User registers and logs into the application.
2. User selects the required steganography module.
3. User uploads the carrier file and confidential data.
4. The confidential data is encrypted.
5. The encrypted data is hidden inside the selected multimedia carrier.
6. The application generates an output file and encryption key.
7. Operation details are recorded in the blockchain.
8. During extraction, the user provides the output file and correct encryption key.
9. The system decrypts and retrieves the original hidden data.

## 🚀 Future Enhancements

- Improve encryption and key management.
- Add support for additional multimedia formats.
- Enhance performance for large multimedia files.
- Implement stronger access control and security monitoring.
- Improve blockchain record management.

## 👩‍💻 Author

**Developed as an academic project.**

## 📜 License

This project is intended for educational and research purposes.
