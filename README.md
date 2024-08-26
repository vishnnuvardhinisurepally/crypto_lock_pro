# CryptoLock Pro


This Python app encrypts and decrypts files using AES, emphasizing user-friendly interaction. It includes password setup with PBKDF2 hashing and OTP verification via email for security. The GUI, powered by tkinter and customtkinter, supports single and batch file operations with ease. Ideal for securing files with Python 3.6+ compatibility.

File Encryption and Decryption Application

This Python application provides a graphical user interface (GUI) for encrypting and decrypting files and folders using AES encryption. It includes features for setting up a password and verifying it using OTP (One-Time Password) sent via email.
Features:

    Password Setup and OTP Verification:
        Users can set a password for encrypting and decrypting files. The password is hashed using PBKDF2 for security.
        OTP (One-Time Password) verification via email adds an extra layer of security. An OTP is sent to the user's email for verification.

    File Encryption and Decryption:
        Supports both single file and batch file encryption and decryption.
        Uses AES encryption in CBC mode with random initialization vectors (IVs) to secure files.

    Graphical User Interface (GUI):
        Developed using tkinter and customtkinter libraries for a user-friendly experience.
        Main interface includes options to set up the password, verify it with OTP, and perform file operations seamlessly.

    Error Handling and Feedback:
        Provides error messages and notifications to guide users through the password setup, OTP verification, and file encryption/decryption processes.
        Logs debug messages for email sending and OTP verification processes.

Usage:

    Setting Up Password:
        Enter your email, set a password, and confirm it.
        An OTP will be sent to your email for verification.

    OTP Verification:
        Enter the OTP received in your email to verify your identity.

    Encrypting and Decrypting Files:
        After successful verification, use the interface to select files or folders for encryption or decryption.
        Files are encrypted with the set password and can be decrypted using the same password.

Requirements:

    Python 3.6 or higher
    Required libraries: tkinter, customtkinter, pyotp, Crypto, pycryptodome

Notes:

    Ensure your email settings are correctly configured in send_email() function for OTP delivery.
    Securely store your generated OTP secret for proper OTP verification.

This application provides a secure method for encrypting sensitive files and ensuring only authorized users can decrypt them using a combination of password and OTP verification
