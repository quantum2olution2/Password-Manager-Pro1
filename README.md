# Password Manager: Secure as a Crypto Wallet

## Overview
This project presents a highly secure, offline password manager inspired by the cryptographic robustness of cryptocurrency wallets. Designed for maximum security, the password manager stores, manages, and generates credentials using cutting-edge encryption, all while operating entirely offline to minimize exposure to online threats.

## Features
- **State-of-the-Art Encryption**: Employs AES-CBC encryption alongside PBKDF2 key derivation for maximum security.
- **Offline Operation**: Ensures that no data is exposed to the internet; all credentials remain on the local device.
- **Encrypted Local Storage**: Utilizes an SQLite database secured with advanced encryption techniques.
- **Customizable Password Generation**: Allows users to create strong, unique passwords based on predefined criteria.
- **User-Friendly Interface**: Built with PyQt5 to provide a seamless and intuitive user experience.
- **Advanced Search Capabilities**: Enables efficient filtering by client, category, site, username, or custom notes.

## Technical Details
### Encryption Mechanisms
- **AES-CBC (Advanced Encryption Standard - Cipher Block Chaining)**: Used for encrypting stored credentials.
- **PBKDF2 (Password-Based Key Derivation Function 2)**: Enhances security by deriving cryptographic keys from the master password, mitigating brute-force attacks.

### Secure Storage
- Data is stored in an encrypted SQLite database.
- Each entry includes:
  - Website or service name.
  - Username.
  - Encrypted password.
  - Optional notes or metadata.

### Localized and Offline Functionality
- The application does not connect to the internet, ensuring total isolation from potential network-based attacks.
- All encryption and decryption processes occur locally on the user's device.

## Usage Guide
1. **Initial Setup**
   - On first use, the user creates a master password. This password serves as the only key for encrypting and decrypting stored credentials.
   - Note: The master password cannot be recovered if lost.

2. **Password Management**
   - Add, view, edit, and delete password entries.
   - Passwords are displayed only when explicitly decrypted, ensuring visual security.

3. **Secure Password Generation**
   - Generate complex passwords with options for length, character sets, and special symbols.

4. **Search Functionality**
   - Filter and locate specific credentials using advanced search criteria.

## Key Benefits
- **Unparalleled Security**: Offline-only functionality coupled with robust encryption eliminates external threats.
- **Simple Yet Powerful**: User-friendly interface ensures ease of use without sacrificing security.
- **Complete Control**: Users retain full ownership and control of their data, stored locally.

## Deployment
- **Executable Format**: Distributed as a standalone executable file (.exe) to simplify installation and ensure compatibility.
- **Platform Compatibility**: Designed primarily for desktop environments; future expansions may include additional platforms.

## Limitations
- The application does not support cloud backup or syncing to maintain offline integrity.
- Users are responsible for securely storing their master password.

## License
This project is open-source and released under the MIT License. Refer to the LICENSE file for more details.

## Acknowledgments
We extend our gratitude to the open-source community and cryptographic researchers whose work has inspired this project. Special thanks to the developers of PyQt5, SQLite, and modern cryptographic libraries for enabling secure and innovative solutions.

## Future Enhancements
- Multi-platform support (macOS, Linux).
- Integration with hardware security modules (HSMs) for additional layers of protection.
- Advanced audit logs for monitoring password access and changes.
