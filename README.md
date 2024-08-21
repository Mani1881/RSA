# RSA
RSA Encryption - Decryption
The RSA algorithm is a widely used cryptographic algorithm for secure communication, encryption, and digital signatures. It is named after its inventors, Ron Rivest, Adi Shamir, and Leonard Adleman. The RSA algorithm is based on the mathematical properties of large prime numbers and modular arithmetic. RSA Algorithm follows the below steps for encoding and decoding

Key Generation: Two distinct prime numbers, p and q, are selected. Their product, n = p * q, is calculated. This is the modulus used in encryption and decryption. Euler's totient function of n, φ(n) = (p - 1) * (q - 1), is calculated. This function calculates the count of positive integers less than n that are coprime (have no common factors) with n. An integer e is chosen, such that 1 < e < φ(n), and e is coprime with φ(n). This is the public exponent and will be part of the public key. The modular multiplicative inverse of e modulo φ(n) is calculated. This is a number d such that (d * e) % φ(n) = 1. d is the private exponent and will be part of the private key.

Encryption: The plaintext message is converted to a numeric representation. In RSA, this is often done using the ASCII values of the characters. The ciphertext c is computed by raising the plaintext message m to the power of the public exponent e modulo n: c = (m^e) % n.

Decryption: The ciphertext c is retrieved. The plaintext message m is computed by raising the ciphertext to the power of the private exponent d modulo n: m = (c^d) % n.


