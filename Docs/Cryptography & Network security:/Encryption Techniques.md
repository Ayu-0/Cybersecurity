
# Encryption:
Encryption is used to protect data from being stolen, changed, or compromised and works by scrambling data into a secret code that can only be unlocked with a unique digital key.

Cipher - Cipher is basically you can say it's encryption algorithm
## How encryption works :
- It converts readable data (plaintext) into an unreadable format (ciphertext) using a mathematical algorithm and a secret key. Only authorized users with the correct decryption key can revert it to its original form. 
- To decode the data back to plaintext requires the use of a decryption key, a string of numbers or a password also created by an algorithm. Secure encryption methods have such a large number of cryptographic keys that an unauthorized person can neither guess      (which one is correct), nor use a computer to easily calculate the correct string of characters by trying every potential combination.


## TYPES OF ENCRYPTIONS :
The two most common types of encryption algorithms are symmetric and asymmetric.

1. Symmetric encryption (shared key or private key algorithm) -
- Uses the same secret key for encryption and decryption. 
- Symmetric key ciphers are considered less expensive to produce and do not take as much computing power to encrypt and decrypt, meaning there is less of delay in decoding the data.

- The drawback is that if an unauthorized person gets their hands on the key, they will be able to decrypt any messages and data sent between the parties. As such, the transfer of the shared key needs to be encrypted with a different cryptographic key, leading to a cycle of dependency. 

- Example Algorithms:
AES (Advanced Encryption Standard) – Most secure, used in government and industry.
DES (Data Encryption Standard) – Older and less secure.
3DES (Triple DES) – More secure than DES but slower.

### AES -
### DES - 
### 3DES -

## Classical Encryption Technique -

- Classical encryption techniques are traditional methods used to secure information by converting plaintext into ciphertext. 
- These methods, though outdated for modern security needs, are significant for understanding the evolution of cryptography. 
- Since it's mostly related to symmetric encryption technique, we'll cover it here
Common examples include:

i.) Substitution Ciphers: Replace each letter with another, such as the Caesar cipher, where letters are shifted by a fixed number.
ii.) Transposition Ciphers: Rearrange letters according to a specific pattern, like reversing the order of letters in a sentence.
iii.) Vigenère Cipher: Uses a keyword to determine the substitution alphabet for each letter, providing polyalphabetic substitution.

### Caesar Cipher
The Caesar Cipher represents one of the earliest and simplest symmetric encryption techniques. Named after Julius Caesar who reportedly used it for military communications, this substitution cipher operates by shifting each letter in the plaintext by a fixed number of positions in the alphabet.
For example, with a shift value of 3:

A becomes D
B becomes E
Z wraps around to C

The encryption and decryption processes are straightforward:

Encryption: C = (P + K) mod 26
Decryption: P = (C - K) mod 26

Where P represents the plaintext letter position, C the ciphertext letter position, and K the shift value (the key).
Despite its historical significance, the Caesar Cipher offers minimal security as it has only 25 possible keys, making it vulnerable to brute force attacks and frequency analysis

### Playfair Cipher 
The Playfair Cipher marked a significant advancement over simple substitution ciphers by encrypting pairs of letters (digraphs) rather than individual characters. This approach disrupts single-letter frequency analysis.
The encryption process requires:

Creating a 5×5 grid of letters based on a keyword (typically omitting J or combining I/J)
Dividing the plaintext into pairs of letters
Applying rules based on the positions of each letter pair in the grid:

Letters in the same row are replaced by letters to their right
Letters in the same column are replaced by letters below
Letters forming a rectangle are replaced by letters at the opposite corners

The Playfair Cipher provided reasonable security for its time but eventually succumbed to cryptanalysis techniques that exploited the limited number of possible digraphs and patterns in English text


### Hill Cipher
The Hill cipher is a polygraphic substitution cipher that encrypts multiple letters at once, typically using matrix multiplication. Here's a simplified explanation of how it works:

Matrix Key: A key matrix is used to encrypt the plaintext. This matrix must be invertible modulo 26 (the number of letters in the alphabet) to ensure decryption is possible.

Plaintext Conversion: Each letter of the plaintext is converted into a number (A=0, B=1, ..., Z=25). These numbers are arranged into a vector.

Matrix Multiplication: The plaintext vector is multiplied by the key matrix. The resulting vector is then converted back into ciphertext letters using modulo 26 arithmetic.

Decryption: To decrypt, the inverse of the key matrix is used. The ciphertext vector is multiplied by this inverse matrix to retrieve the original plaintext vector, which is then converted back into letters.
The decryption requires finding the inverse of the key matrix, which adds complexity to both implementation and cryptanalysis.
The Hill Cipher's strength derives from its mathematical foundation, making it more resistant to basic frequency analysis. However, it remains vulnerable to known-plaintext attacks where portions of both plaintext and corresponding ciphertext are available to an attacker.



2. Asymmetric encryption: (public-key cryptography) -
- Uses two separate keys to encrypt and decrypt data. One is a public key shared among all parties for encryption. Anyone with the public key can then send an encrypted message, but only the holders of the second, private key can decrypt the message. 

- Asymmetric encryption is considered more expensive to produce and takes more computing power to decrypt as the public encryption key is often large, between 1,024 and 2,048 bits. As such, asymmetric encryption is often not suited for large packets of data.

- Example Algorithms:
RSA (Rivest-Shamir-Adleman) – Used for secure data transmission.
ECC (Elliptic Curve Cryptography) – Stronger security with smaller key sizes.
Diffie-Hellman (DH) – Used for key exchange.

## RSA (Rivest-Shamir-Adleman) -

## ECC (Elliptic Curve Cryptography) -

## Diffie-Hellman(DH) - 