
# CryptoLock Pro

**CryptoLock Pro** is a Python application designed to provide robust file encryption and decryption with a focus on security and ease of use. The app features a user-friendly graphical interface that allows users to encrypt and decrypt both single files and batches of files using AES encryption. With integrated password setup, PBKDF2 hashing, and OTP verification via email, CryptoLock Pro ensures that only authorized users can access your encrypted data.

## Features

### Password Setup and OTP Verification
- **Password Setup**: Users can set a secure password for encrypting and decrypting files. The password is hashed using PBKDF2, adding an extra layer of protection.
- **OTP Verification**: An OTP (One-Time Password) is sent to the user's email during the password setup process to verify their identity, enhancing security.

### File Encryption and Decryption
- **Single and Batch File Operations**: The application supports both single file and batch file encryption and decryption, allowing users to secure multiple files in one go.
- **AES Encryption**: Uses AES encryption in CBC mode with random initialization vectors (IVs) to ensure strong file security.

### Graphical User Interface (GUI)
- **User-Friendly Interface**: Developed using `tkinter` and `customtkinter`, the GUI is intuitive and easy to navigate, making file encryption accessible to all users.
- **Seamless Operations**: The main interface provides clear options for setting up a password, verifying it with OTP, and performing file operations effortlessly.

### Error Handling and Feedback
- **Guided Processes**: The application provides informative error messages and notifications, helping users through the password setup, OTP verification, and file encryption/decryption processes.
- **Debug Logging**: Logs are generated for debugging purposes, particularly for email sending and OTP verification processes, aiding in troubleshooting.

## Usage

### Setting Up Password
1. **Enter Email**: Input your email address where the OTP will be sent.
2. **Set and Confirm Password**: Choose a secure password and confirm it.
3. **OTP Verification**: An OTP will be sent to your email. Enter it in the application to verify your identity.

### Encrypting and Decrypting Files
1. **Post-Verification**: Once your identity is verified, select files or folders from the interface to encrypt or decrypt.
2. **File Security**: Files are encrypted using the password you set and can be decrypted using the same password.

## Requirements

- **Python 3.6 or higher**
- Required Python libraries:
  - `tkinter`
  - `customtkinter`
  - `pyotp`
  - `Crypto`
  - `pycryptodome`

## Installation

1. Ensure you have Python 3.6 or higher installed.
2. Install the required libraries using pip:

   ```bash
   pip install tkinter customtkinter pyotp pycryptodome
   ```

3. Clone or download the repository containing the CryptoLock Pro script.

## Configuration

- **Email Settings**: Ensure your email settings are correctly configured in the `send_email()` function for OTP delivery.
- **OTP Secret Storage**: Securely store the generated OTP secret to ensure proper OTP verification during the password setup process.

## Notes

- This application provides a secure method for encrypting sensitive files, ensuring that only authorized users can decrypt them using a combination of password protection and OTP verification.
- Make sure to keep your password and OTP secret safe, as they are crucial for accessing your encrypted files.

