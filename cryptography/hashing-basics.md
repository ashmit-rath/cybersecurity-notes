# Hashing Basics

## Overview
Hashing is a one-way deterministic function that converts input data into a fixed-length digest.  
Used for data integrity and password storage.

---

## Hashing Files (CLI)

### Syntax
```bash
<tool> <file>
```

### Examples
```bash
md5sum file.txt
sha1sum file.txt
sha256sum file.txt
sha512sum file.txt
```

### Output Format
```
<hash_value>  <filename>
```

---

## Generate & Store Hash

```bash
sha256sum file.txt > file.sha256
```

---

## Verify Hash

```bash
sha256sum -c file.sha256
```

---

## Hashing Strings

### Syntax
```bash
echo -n "<input>" | <tool>
```

### Examples
```bash
echo -n "password" | md5sum
echo -n "password" | sha256sum
```

---

## Common Algorithms

| Algorithm | Output | Status |
|----------|--------|--------|
| MD5      | 128-bit | Broken |
| SHA1     | 160-bit | Weak |
| SHA256   | 256-bit | Secure |
| SHA512   | 512-bit | Strong |

---

## Hash Properties

- One-way (irreversible)
- Same input → same output
- Small change → completely different hash

---

## Salt

```
hash(password + salt)
```

Purpose:
- Prevent rainbow table attacks
- Ensure unique hashes

---

## Hash Identification

| Length | Likely |
|--------|--------|
| 32     | MD5 |
| 40     | SHA1 |
| 64     | SHA256 |
| 128    | SHA512 |

---

## Hashcat

### Syntax
```bash
hashcat -m <mode> -a <attack_mode> <hash_file> <wordlist_or_mask>
```

---

### Attack Modes

| Mode | Type |
|------|------|
| 0    | Dictionary |
| 3    | Mask |
| 6    | Hybrid |

---

### Examples

#### MD5 Dictionary Attack
```bash
hashcat -m 0 -a 0 hashes.txt rockyou.txt
```

#### SHA256 Dictionary Attack
```bash
hashcat -m 1400 -a 0 hashes.txt rockyou.txt
```

#### Mask Attack (6 chars)
```bash
hashcat -m 0 -a 3 hashes.txt ?a?a?a?a?a?a
```

#### 4-digit PIN
```bash
hashcat -m 0 -a 3 hashes.txt ?d?d?d?d
```

#### Hybrid Attack
```bash
hashcat -m 0 -a 6 hashes.txt rockyou.txt ?d?d
```

---

### Output File
```bash
hashcat -m 0 -a 0 hashes.txt rockyou.txt -o cracked.txt
```

---

### Show Results
```bash
hashcat --show hashes.txt
```

---

### Resume Session
```bash
hashcat --restore
```

---

### Common Modes

| Mode | Algorithm |
|------|----------|
| 0    | MD5 |
| 100  | SHA1 |
| 1400 | SHA256 |
| 1700 | SHA512 |

---

### Mask Charset

| Symbol | Meaning |
|--------|--------|
| ?l     | lowercase |
| ?u     | uppercase |
| ?d     | digits |
| ?s     | special |
| ?a     | all |

---

## Encoding vs Encryption vs Hashing

| Type       | Reversible | Purpose |
|------------|-----------|--------|
| Hashing    | No        | Integrity |
| Encoding   | Yes       | Representation |
| Encryption | Yes       | Confidentiality |

---

## Base64 (Encoding)

### Encode
```bash
echo "hello" | base64
```

### Decode
```bash
echo "aGVsbG8=" | base64 -d
```

---

## Key Points

- Hashing is irreversible
- MD5/SHA1 are insecure
- Use salted hashing for passwords
- Base64 is not encryption
