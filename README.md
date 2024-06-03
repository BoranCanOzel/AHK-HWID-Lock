# 🔐 AHK Login System

This repository contains a simple software copy protection system implemented in AutoHotkey (AHK). It consists of two main scripts: `admin_ini_generator.ahk` and `user.ahk`.

## 📂 Files

- `admin_ini_generator.ahk`: This script generates an INI file containing user registration information.
- `user.ahk`: This script checks the user's registration information to ensure that the software is registered and authorized for use.

## 🛠️ Requirements

- AutoHotkey Version: 1.0.39+
- Platform: Windows 2000/XP

## 📜 Usage

1. **Admin Script (`admin_ini_generator.ahk`)**
    - Prompts for the user's name, email, and PC fingerprint.
    - Generates an unlock code based on the provided information.
    - Writes the user information and unlock code to `SafeSW.ini`.

2. **User Script (`user.ahk`)**
    - Reads the user information and unlock code from `SafeSW.ini`.
    - Validates the current user's PC fingerprint against the stored unlock code.
    - If validation fails, prompts the user to register.

## 🔒 Crypto Functions

The scripts use the TEA cipher and XCBC-MAC for encryption and authentication. These functions ensure secure processing of user data and PC fingerprints.
``` &#8203;:citation[【oaicite:0】]&#8203;
