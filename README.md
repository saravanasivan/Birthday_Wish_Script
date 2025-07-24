# 📄 README.md — Birthday WhatsApp Automation

## 🎯 Project Overview

This Python script automates sending **birthday wishes via WhatsApp Web** using contact information stored in an Excel file. It checks each entry for birthdays that match today's date and sends a personalized message through WhatsApp Web.

## 📁 File Structure

BirthdayWish/
├── birthdays.xlsx        # Excel file with name, DOB (DD-MM-YY), and phone number
├── wish by whatsapp.py   # Main Python script
└── README.md             # This file

## ✅ Features

- Reads an Excel file with columns: `Name`, `Date of Birth`, `Mobile Number`
- Sends instant WhatsApp messages using `pywhatkit`
- No scheduled delay — messages are sent immediately
- 60-second delay between each message to prevent blocking
- Closes WhatsApp Web tab automatically after sending

## 📦 Requirements

- Python 3.7+
- `pywhatkit` library
- WhatsApp Web logged in on your default browser (Chrome/Edge)

## 🔧 Installation

### 1. Install Python packages

    pip install pywhatkit pandas openpyxl

### 2. Ensure your `birthdays.xlsx` file follows this format:

| Name         | Date of Birth | Mobile Number |
|--------------|----------------|----------------|
| Alice Singh  | 24-07-95       | 9876543210     |
| Bob Sharma   | 10-12-88       | 9123456789     |

- `Date of Birth` format must be: **DD-MM-YY**

## ▶️ Usage

Run the script using:

    python "wish by whatsapp.py"

- Make sure your default browser is **logged into WhatsApp Web**.
- Keep your internet connection stable.
- A browser tab will open, send the message, and close automatically.

## 📝 Notes

- Works best with **Chrome** or **Edge** browsers.
- Assumes mobile numbers are **Indian (+91)**. Modify the script if using a different country code.
- This tool is ideal for **personal use**. For high-volume or business messaging, use WhatsApp Business API.

## 📅 Automation Tip

To run this script every day automatically:

### On Windows:
1. Open **Task Scheduler**
2. Create Basic Task → Choose Daily → Select script via `pythonw` or `.bat` file

## 💡 Future Improvements

- Support for sending images/files
- Logging system
- GUI to manage contact list

## 📬 Contact

If you have issues or need customization, feel free to open an issue or request features!
