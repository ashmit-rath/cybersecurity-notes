# Cryptography Basics

## 1. Core Purpose
Cryptography is used to secure communication and data.

Key goals:
- Confidentiality → data hidden from unauthorized users
- Integrity → data not modified
- Authentication → verify identity
- Non-repudiation → sender cannot deny

---

## 2. Plaintext vs Ciphertext

- Plaintext → original readable data
- Ciphertext → encrypted unreadable data

Encryption:
Plaintext → Ciphertext

Decryption:
Ciphertext → Plaintext

---

## 3. Encoding vs Encryption vs Hashing

### Encoding
- Reversible without key
- Used for formatting (Base64)

### Encryption
- Requires key
- Reversible
- Used for security

### Hashing
- One-way function
- Cannot be reversed
- Used for passwords

---

## 4. Historical Ciphers

### Caesar Cipher
- Shift letters by fixed value
- Weak and easily breakable

Example:
HELLO → KHOOR (shift 3)

---

## 5. Types of Encryption

### Symmetric Encryption
- Same key for encryption and decryption
- Fast
- Problem: key distribution

Examples:
- AES
- DES (outdated)

---

### Asymmetric Encryption
- Two keys:
  - Public key (encrypt)
  - Private key (decrypt)
- Slower but more secure for key exchange

---

## 6. Basic Math Concepts

### XOR Operation
- Used in many encryption algorithms
- Property:
  A ⊕ B ⊕ B = A

---

### Modulo Operation
- Wrap-around arithmetic
- Used in encryption algorithms (especially RSA)

Example:
17 mod 5 = 2

---

## 7. Key Takeaways

- Encryption protects data
- Hashing protects passwords
- Symmetric = fast, Asymmetric = secure key exchange
- Math is core of cryptography
