<div align="center">
<h1><code>Chromium Based Browsers Secrets Dump</code></h1>
<p>A Rust application for extracting and decrypting sensitive data from various web browsers' local storage. This tool decrypts saved passwords and other encrypted data using DPAPI and AES-256-GCM, providing insights into browser-stored credentials securely and efficiently.</p>
</div>

---

## Features
- Cross-Browser Support: Extracts data from a variety of popular web browsers including Google Chrome, Brave, Microsoft Edge, and more.
- Encryption Decryption: Utilizes AES-256-GCM for decrypting sensitive data encrypted by browsers.
- Flexible Queries: Supports customizable SQL queries to extract specific data types such as passwords, credit card details, and more.
  - Logins
    - URL
    - Email addresses
    - Passwords
  - Credit cards
    - Card number
    - Expiration date
    - Name on card
  - Cookies

## How It Works
The application works by locating browser data directories, decrypting stored secrets using the DPAPI and AES-256-GCM algorithms, and executing SQL queries on the decrypted databases to retrieve relevant information.

## Installation
### Prerequisites
- Rust programming language and Cargo build system installed.

### Build from Source

1. Clone the repository:

```bash
git clone https://github.com/Fastiraz/chromium-based-browsers-secrets-dump.git
cd chromium-based-browsers-secrets-dump
```

2. Run the project:

```bash
cargo run
```

## Usage
The application will automatically search for supported browsers' data directories on your system. Ensure to run the application with administrative or appropriate permissions to access browser data directories and decrypt secrets.

## List of supported browsers

- Avast
- Amigo
- Torch
- Kometa
- Orbitum
- Cent Browser
- 7star
- Sputnik
- Vivaldi
- Google Chrome sxs
- Google Chrome
- Epic Privacy Browser
- Microsoft Edge
- Uran
- Yandex
- Brave Browser
- Iridium