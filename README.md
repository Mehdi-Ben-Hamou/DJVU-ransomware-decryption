# 🛡️ DJVU Ransomware Decryption Tool

This project aims to help victims of the **DJVU/STOP ransomware** by analyzing encrypted files and attempting to restore original data whenever possible.

---

## 🔍 About the Project
The **DJVU ransomware** encrypts user files and appends a variant-specific extension  
(e.g., `.djvu`, `.gero`, `.seto`, `.boop`, etc.).

This tool provides:
- Detection of encrypted DJVU files  
- Analysis of folders containing encrypted content  
- Basic decryption attempts  
  - using known static keys  
  - or comparing encrypted/original files (when available)

---

## 📁 Features
- 🔎 **Automatic detection** of DJVU-encrypted files  
- 📂 **Recursive folder analysis**  
- 🔐 **Decryption attempts** based on known keys or file comparison  
- 📊 **Result report** (success / failure)  
- 🛠️ **Easily extendable** to other STOP/DJVU ransomware variants  

---

## 📂 Project Structure
```text
ransomware_project/
├── test_directory/
│   ├── README.txt
│   ├── Test.jpg
│   ├── Test.pdf
│   └── Test.txt
├── Rapport_Rans.pdf
├── aes_key.txt
├── detect.py
├── fake_rans.py
└── README.md
```
## Getting Started
### Clone the repository
```bash
git clone https://github.com/Mehdi-Ben-Hamou/DJVU-ransomware-decryption
cd DJVU-ransomware-decryption
```
### Test the fake ransomware (for education)
```bash
python fake_rans.py
```
## Run the decryption script
```bash
python decrypt.py
````
## ⚠️ This script is for educational and research purposes ONLY.
Do not use it for malicious activity.

## 📄 Files Description
### File	Description
fake_rans.py	Simulation of DJVU-like encryption (for testing)
decrypt.py	python script for decryption
aes_key.txt	Key used by the fake ransomware
test_directory/	Folder containing test files
Rapport_Rans.pdf	Project report
README.md	Documentation

## 🔗 Notes
- Decrypting DJVU is only possible for specific variants depending on the key used.
- Modern DJVU variants use online keys → usually not decryptable without the attacker’s key.
- This tool focuses on static-key variants and file comparison methods.

## 📜 Disclaimer
**This project is strictly for educational, research, and cybersecurity awareness purposes.**
**I'm not responsible for any misuse.**
