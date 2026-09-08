# -UPI-Payment-QR-Code-Generator-Using-Python-
UPI Payment QR Code Generator Using Python is a project that generates QR codes from UPI IDs. It creates a UPI payment URL and converts it into a scannable QR code using Python’s QRCode library. The QR code is saved as an image for easy sharing and digital payments.
# UPI Payment QR Code Generator Using Python

## 📌 Project Overview

UPI Payment QR Code Generator is a Python-based project that generates QR codes from UPI IDs. It creates a UPI payment URL and converts it into a scannable QR code using Python's QRCode library.

## 🎯 Objectives

- Generate UPI payment QR codes.
- Accept UPI ID as user input.
- Create UPI payment URLs.
- Save QR codes as image files.
- Simplify sharing of payment information.

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- QRCode Library
- Pillow

## 📦 Installation

Install the required library using:

```bash
pip install qrcode[pil]

import qrcode

upi_id = input("Enter your UPI ID: ")

upi_url = f"upi://pay?pa={upi_id}&pn=Recipient%20Name"

qr = qrcode.make(upi_url)

qr.save("upi_qr_code.png")

print("UPI QR Code generated successfully!")

UPI-Payment-QR-Code-Generator/
│
├── Untitled4.ipynb
├── upi_qr_code.png
└── README.md
