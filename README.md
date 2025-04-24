🔐 Secure File Storage using Hybrid Cryptography
A secure cloud-based file storage system that utilizes hybrid cryptography to ensure confidentiality and integrity of user data.

🚀 Objective
To create a secure platform for storing files on the cloud using a combination of cryptographic algorithms in a round-robin manner. The system ensures that both data and encryption keys are protected, providing a robust mechanism for secure file storage and retrieval.

🛠️ Methodology
🔒 Encryption Process
Upload File: The user uploads a file to the server.

File Segmentation: The uploaded file is split into N parts.

Hybrid Encryption: Each part is encrypted using a different cryptographic algorithm in a round-robin sequence.

Key Protection: The encryption keys are then encrypted using a separate algorithm.

Key Delivery: The key for decrypting the encryption keys is securely shared with the user as a public key file.

Storage: Encrypted file parts are stored on the server.

🔓 Decryption Process
Upload Key: The user uploads their public key file.

Key Decryption: The encrypted encryption keys are decrypted using the provided key.

File Decryption: Each file part is decrypted using the respective algorithm.

File Reconstruction: Decrypted parts are combined to reconstruct the original file.

Download: The user can download the fully restored original file.

⚙️ How to Run
Note: This project is based on Python 2.7.15. Running it on other versions may result in compatibility issues.

📥 Step-by-Step Setup
Clone the Repository

bash
Copy
Edit
git clone https://github.com/yourusername/Secure_File_Storage_Hybrid_Cryptography.git
cd Secure_File_Storage_Hybrid_Cryptography
Install Requirements

bash
Copy
Edit
pip install -r requirements.txt
Run the Application

bash
Copy
Edit
python app.py
Access via Browser Visit http://localhost:5000 to use the application.

📁 Folder Structure
php
Copy
Edit
.
├── app.py                     # Main application file
├── requirements.txt           # Python dependencies
├── templates/                 # HTML templates
├── static/                    # Static files (CSS, JS)
└── uploads/                   # Directory for file parts
🔐 Cryptographic Techniques Used
AES (Advanced Encryption Standard)

DES (Data Encryption Standard)

RSA (Rivest–Shamir–Adleman)

Custom round-robin encryption methodology

Each file part is encrypted using a different algorithm to ensure additional layers of security.

✨ Author
Gouri Nandana
B.Tech in CSE (Cybersecurity & Digital Forensics)
Email: nandanagouri47@gmail.com
Phone: +91-9207141944
