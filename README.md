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
