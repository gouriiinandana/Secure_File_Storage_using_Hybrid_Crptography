# Secure_File_Storage_using_Hybrid_Cryptography

Objective: To Achieve a secure plateform for storing of files on Cloud using Hybrid Cryptography.

#Methodology

To achieve the above goal, the following methodology needs to be followed:

Load the file on the server.
Dividing the uploaded file into N parts.
Encrypting all the parts of the file using any one of the selected algorithms (Algorithm is changed with every part in round robin fashion).
The keys for cryptography algorithms is then secured using a different algorithm and the key for this algorithm is provided to the user as public key.
After the above 4 steps you will have a N files which are in encrypted form which are stored on the server and a key which is downloaded as public key for decrypting the file and downloading it.

To restore the file, follow the following steps:

Load the key on the server.
Decrypt the keys of the algorithms.
Decrypt all the N parts of the file using the same algorithms which were used to encrypt them.
Combine all the N parts to form the original file and provide it to the user for downloading.
How to Run
NOTE: The project is based on Python 2.7.15 plateform running it on any other plateform might create some issues.

Step 1: Install Requirements
pip install -r requirements.txt

Step 2: Run the application
python app.py

Step 3: Visit the localhost from your browser

Step 4: Enjoy :)
