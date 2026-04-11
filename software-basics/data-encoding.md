# Data Encoding

## Base64

Encoding example
hello → aGVsbG8=

Decode example
aGVsbG8= → hello

Linux
echo hello | base64

Decode
echo aGVsbG8= | base64 -d

--------------------------------

## URL Encoding

Space = %20

Example
hello world
hello%20world

--------------------------------

## Hex Encoding

hello
68 65 6c 6c 6f

--------------------------------

## Why Encoding

- data transfer
- obfuscation
- web requests
- payload encoding
