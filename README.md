# 🔐 Secure Steganography-Based Communication System using AES, LSB & Digital Watermarking

This project introduces a **robust and secure data communication system** combining **AES-256 encryption**, **LSB-based image steganography**, and **DCT-DWT watermarking**. It ensures **confidentiality**, **integrity**, and **non-repudiation** in transmitting secret messages over untrusted channels.

Both **MATLAB** (for encryption, watermarking, and image processing simulations) and **Python** (for GUI-based implementation) have been used.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [System Architecture](#-system-architecture)
- [How It Works](#-how-it-works)
  - [Sender Side Workflow](#sender-side-workflow)
  - [Receiver Side Workflow](#receiver-side-workflow)
- [Technologies Used](#-technologies-used)
- [Security Objectives](#-security-objectives)
- [Conclusion](#-conclusion)

---

## 🔍 Overview

This project focuses on **image-based steganography** enhanced with **Advanced Encryption Standard (AES-256)** and **digital watermarking**. It ensures secure message transfer by embedding an encrypted message inside an image using the **Least Significant Bit (LSB)** method. Additional robustness is achieved using **DCT-DWT watermarking** and **multi-part image transmission**.

---

## 💡 Key Features

- ✅ AES-256 Encryption for message and image security  
- ✅ LSB-based Image Steganography  
- ✅ DCT-DWT Watermarking for non-repudiation  
- ✅ GUI-based Python Application for ease of use  
- ✅ Image Fragmentation and Stitching for added security  
- ✅ MATLAB Simulation of watermarking and steganography techniques

---

## 🧠 System Architecture


---

## ⚙️ How It Works

### 📤 Sender Side Workflow

1. User inputs:
   - Secret message
   - Cover image
   - Symmetric key
2. Secret message is encrypted using AES-256.
3. Image is encrypted using AES-256.
4. Message is embedded in the image using the LSB technique.
5. A digital watermark is added using DCT-DWT.
6. The result is embedded into a secondary cover image.
7. The stego image is split into 16 parts.
8. Each image part is transmitted independently.

### 📥 Receiver Side Workflow

1. Reassemble the 16 image fragments using their index.
2. Extract the embedded image from the secondary cover.
3. Retrieve the encrypted image and message via LSB extraction.
4. Decrypt the image and message using AES-256.
5. Final secret message is recovered.

---

## 🛠️ Technologies Used

| Tool         | Purpose                              |
|--------------|---------------------------------------|
| **MATLAB**   | Image processing, simulation, watermarking |
| **Python**   | GUI application, AES + LSB implementation |
| **NumPy**    | Matrix and pixel manipulation         |
| **OpenCV**   | Image processing and transformations  |
| **Tkinter**  | GUI development                       |
| **PyCryptodome** | AES-256 encryption and decryption     |

---

## 🔐 Security Objectives

- **Confidentiality**: AES encryption ensures message secrecy.
- **Integrity**: Data is protected from unauthorized access or corruption.
- **Non-Repudiation**: DCT-DWT watermarking confirms sender authenticity.
- **Robustness**: Withstands processing operations and attacks.
- **Privacy**: Steganography ensures covert message transmission.
- **Embedding Effectiveness**: High probability of successful embedding in arbitrary images.
- **Security**: Multi-layer encryption and embedding make detection extremely difficult.

---

## ✅ Conclusion

This project presents a **secure hybrid system** that integrates **cryptography**, **steganography**, and **digital watermarking** for covert and authenticated communication. The **AES + LSB + Watermarking** combination makes it extremely difficult for adversaries to detect or alter the data. It also ensures **non-repudiation**, a unique feature missing in many other stego systems.


