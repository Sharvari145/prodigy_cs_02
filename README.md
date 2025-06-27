# prodigy_cs_02
🔐 Image Encryption & Decryption using Python

This Python script provides a simple method to **encrypt and decrypt images** using pixel-level transformation. 
The encryption technique shifts pixel values by a fixed key and wraps them using modulo 256 logic, ensuring image data remains valid.

📌 Features

* Encrypts any image by shifting pixel values
* Decrypts the encrypted image using the same key
* Works with common image formats like PNG, JPG, BMP
* Uses `PIL` (Pillow) and `NumPy` for efficient image processing
* Handles overflow and underflow using `int16` casting
* CLI-based interaction (simple input prompts)

🔧 Requirements

* Python 3.x
* Pillow
* NumPy

Install dependencies using:

bash
pip install pillow numpy


🚀 How to Use

1. Run the Script:

bash
python image_encrypt_decrypt.py


2. Choose Mode:

* Type `'e'` to encrypt
* Type `'d'` to decrypt

3. Follow Prompts:

Enter image paths and output file paths as asked

🔒 Encryption Logic

Encrypt:(pixel + KEY) % 256`
Decrypt:(pixel - KEY) % 256`

> The key value is fixed at `50`. For secure applications, use dynamic or cryptographic keys.

📁 Sample Output

* Encrypted image looks visually distorted (unreadable)
* Decrypted image restores original content


 📌 License

MIT License
