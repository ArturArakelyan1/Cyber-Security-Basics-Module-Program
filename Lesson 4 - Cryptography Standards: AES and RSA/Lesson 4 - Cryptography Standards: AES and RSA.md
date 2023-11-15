# Lesson 4 - Cryptography Standards: AES and RSA

## Introduction to Symmetric and Asymmetric Cryptography

**Symmetric vs. Asymmetric Cryptography:**
- Defining and differentiating the two primary types of cryptography.
- Symmetric uses the same key for encryption and decryption, while asymmetric uses a pair of public and private keys.

**Real-World Applications:**
- Exploring where each type is used in practice, such as symmetric for data at rest and asymmetric for data in transit.

## Advanced Encryption Standard (AES)

**Development and Adoption of AES:**
- History: Developed to replace the older DES (Data Encryption Standard).
- Adoption as a federal standard by the U.S. government.

**How AES Works:**
- Key Sizes: AES operates with key sizes of 128, 192, or 256 bits.
- Encryption Process:
  - Data Block and Key Expansion: AES encrypts data in 128-bit blocks and expands the key using the Rijndael's key schedule.
  - Rounds of Encryption: Depending on the key size, AES performs 10, 12, or 14 rounds of encryption. Each round consists of several processing steps: SubBytes, ShiftRows, MixColumns, and AddRoundKey.
  - Final Round: Involves all the steps except MixColumns.
- Security Aspects: Discussing its resistance to all known attacks, making it suitable for securing top-secret information.

**Practical Demonstration:**
- Encrypting and decrypting a text file using AES-256.

## RSA Algorithm

**Development and Importance:**
- Historical context of RSA, developed by Rivest, Shamir, and Adleman.
- Importance in digital signatures and secure key exchanges.

**How RSA Works:**
- Key Generation:
  - Selecting two large prime numbers.
  - Computing their product (n) and the totient.
  - Choosing an encryption key (e) and calculating the decryption key (d).
- Encryption and Decryption Process:
  - Encryption: \(c \equiv m^e \mod n\), where \(m\) is the message.
  - Decryption: \(m \equiv c^d \mod n\).
- Security Considerations: Discussing the difficulty of factoring large primes as the basis of RSA's security.

**Practical Application:**
- Conducting a secure message exchange using RSA encryption.

## Cryptography in Practice

**Using AES and RSA Together:**
- Common practice in SSL/TLS: RSA for key exchange and AES for encrypting data.
- Demonstration: Setting up a simple SSL/TLS session.

**Best Practices in Cryptographic Implementations:**
- Importance of proper key management.
- Avoiding common pitfalls in cryptographic implementations.

## Future Directions

**Post-Quantum Cryptography:**
- Discussion on how quantum computing might impact the security of AES and RSA.
- Introduction to post-quantum cryptographic algorithms.
