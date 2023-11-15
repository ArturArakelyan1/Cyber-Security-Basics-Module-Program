# Lesson 3 - Understanding Cryptography: Hash Functions

## Basics of Cryptography

**Introduction to Cryptography:**
- Exploration of cryptography as the art of writing and solving codes.
- Evolution from simple ciphers to complex digital algorithms.

**Types of Cryptographic Algorithms:**
- Symmetric (e.g., AES) vs. Asymmetric (e.g., RSA) vs. Hash Functions.
- Role of each in ensuring digital security and integrity.

## Hash Functions: From Basics to SHA-2

**Understanding Hash Functions:**
- Definition: A hash function is a mathematical algorithm that transforms any arbitrary block of data into a new series of characters with a fixed length.
- Key properties: Determinism, fast computation, pre-image resistance, avalanche effect, collision resistance.

**MD5 (Message Digest Algorithm 5):**
- Development and history: Designed by Ronald Rivest in 1991 as a successor to MD4.
- How MD5 works:
  - Processing: MD5 processes data in 512-bit blocks, dividing each block into 16 words of 32 bits each. It uses a 128-bit hash value.
  - Four Main Steps: Each block is processed through four main steps – F, G, H, I – which are functions that operate on three 32-bit words and produce a 32-bit word.
  - Operations: These steps involve bitwise operations, modular addition, and non-linear functions.
  - Final Output: After processing all blocks, the output is a 128-bit hash value.
- Vulnerabilities: Discussion of why MD5 is no longer considered secure, focusing on its susceptibility to collision attacks.

**SHA-2 (Secure Hash Algorithm 2):**
- Evolution: Development as part of SHA series following vulnerabilities in SHA-1.
- Variants: SHA-256, SHA-384, SHA-512, and others – differences mainly in bit length.
- How SHA-2 works:
  - Processing: Similar to MD5, SHA-2 processes data in blocks, but with larger block and hash sizes (e.g., 512-bit blocks for SHA-256).
  - Complex Functions: SHA-2 uses more complex functions and constants in its algorithm, enhancing its security.
  - Steps Involved: The data is expanded and then goes through multiple rounds of processing, involving bitwise operations, rotations, and modular additions.
  - Final Output: Produces a hash value (e.g., 256 bits for SHA-256).
- Security: Explanation of why SHA-2 is considered secure against known attack vectors, including its resistance to collision and pre-image attacks.

## Practical Applications of Hash Functions

**Data Integrity and Verification:**
- Using hash functions to verify the integrity of files and data transmissions.
- Workshop: Calculating and verifying hashes of downloaded files.

**Password Storage:**
- Storing passwords securely using hash functions.
- The concept of adding salt to hashes to prevent rainbow table attacks.

**Digital Signatures and Certificates:**
- Role of hash functions in creating digital signatures and SSL/TLS certificates.
- Activity: Creating a digital signature for a document.

## Advanced Topics

**Hash Function Security Analysis:**
- Exploring the complexity of finding hash collisions.
- Case studies on successful attacks against weaker hash functions.

**Looking Ahead: SHA-3 and Beyond:**
- Overview of SHA-3 and its differences from SHA-2.
- The impact of quantum computing on the future of hash functions.
