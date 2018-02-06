### Topics Cryptography 3253.3

#### 01 Introduction

### 01 Introduction

* Why do we need cryptography?
  * *To keep stuff safe*
  * *To break safe stuff*


* Basic Terminology
  * Computer security : *Generic name for the tools designed to protect data*
  * Network security : *Protect data during transmission*
  * Internet security : *Protect data during transmission over networks*
  * Cypher : *Encrypted message*


* Cryptology: Cryptography and Cryptanalysis
    * Cryptology : *science of the secret*
    * Cryptography :   *Cryptography (Secret writing),
      mathematical methods to ensure data Integrity*
    * Cryptanalysis : *Discipline of decryption of information without
    knowing the method of encryption/decryption*


* Symmetric/Asymmetric, Hash, Protocols
  * Symmetric : *Block sypher, stream cypher*
    * *Sender and recipient share the same key*
    * *All classical encryption algorithms are private key*
    * *Only type before public key in 1970*
  * Asymmetric : *Key exchange, Confidentiality, digital signature*
  * Hash : *String of hexadecimals chars obtained after an encryption with an hash function*
  * Protocols : *Abstract or concrete protocole that describes how algorithms should be used to apply cryptographic methods*

* Block vs Stream
  * Stream cypher :
    * *Infinite cryptographic keystream, encrypting one bit/byte at a time*
    * *Usually faster and uses less memory*
    * *More difficult to implement*
    * *No integrity protection*
  * Block cypher :
    * *Work on large chunks of data*
    * *Can be combined for additional security*
    * *Uses more memory*
    * [Truc sur stack overflow, j'ai pas tout compris](https://security.stackexchange.com/questions/334/advantages-and-disadvantages-of-stream-versus-block-ciphers)

* Digital Signature
  * *Mathematical scheme for demonstrating the authenticity of a message*

* Computer vs Network vs Internet Security
  * *Voir Basic terminology*

* Security Attack: Passive, Active: Replay, Message Modification, Denial of Service
* Security Service: signatures, protection from disclosure, tampering, destruction
* X.800: Authentication, Access Control, Data Confidentiality, Data Integrity, Non-repudiation
* Security Mechanism: Designed to detect, prevent, or recover from a security attack
* Specific Security Mechanisms: encipherment (encryption), digital signatures, access control, data
integrity, authentication, traffic padding, routing control, notarization
* Pervasive Security Mechanisms: trusted functionality, security labels, event detection, security
audit trails, security recovery
* Steganography
* Skytale
  * *Oldest military cryptographyc tool known*
  * *We roll a skin around a stick of a certain diameter in order to be able to read it*
  * *The exact diameter has to be used*


* Kerckhoff’s principle
* Uncoditional security vs Computational security
* Substitution ciphers
* Shift ciphers: Caesar, ROT13, etc.
* Vigenere cipher
* Permutation Ciphers
* Enigma
* Vernam cipher (one time pad): Advantages and disadvantages

#### 02 Block Ciphers and Feisteldocs

* Block vs Stream Ciphers
* Substitution-Permutation Networks (S-box and P-box)
* Confusion and diffusion
* Feistel Cipher structure: Lucifer, 3 rounds enough
* Feistel decryption

#### 03 Modular Algebra Introductiondocs

* Definition
* Negative numbers
* Large Numbers
* Number to power to power to power to ...
* Neutral and inverse elements
* Subtraction and division
* Square roots and logaritms


#### 04 Number Theory

* Definition of modulo
* Prime numbers and prime factorization
* Co-prime and gcd
* Euler totient function
* Euler (Totient) theorem
* Algebraic structures: groups, rings, fields
* Primitive element of a finite field
* Sieve of Eratosthenes
* Euclid Algorithm, Bezout lemma and Extended Euclid Algorithm
* Modular multiplicative inverse and the Extended Euclid Algorithm
* Little Fermat Theorem
* Modular Inverse
* Modular exponent: three algorithms


#### 05 Public Key Cryptography and Diffie-Hellman

* Example Alice and Bob
* Public vs Private Key Cryptography
* Public Key Applications: Secrecy and Authentication
* Requirements for Public Key Cryptography
* Trapdoor one-way function
* Diffie-Hellman (p, g, a, b, A, B, s, c, m, Fermat)
* Discrete Logarithms
* How to choose primitive roots?
* Diffie Hellman: setup and encryption/decryption
* Security of DH / Breaking the code
* Example
* Man-in-the-middle attack


#### 06 RSA

* RSA setup
* Euler Totient Function * Why RSA works?
* Factorization
* Generating large primes


#### 07 Generating large prime numbers – primality testings

#### 08 Data Encryption Standard (DES)

* Scheme, Number of rounds, size of the key * Initial Permutation
* DES Round structure
* Substitution Boxes
* Key schedule and rotation of the keys
* Expansion function and permutation
* DES decryption
* Avalanche effect
* Type of attacks: Key size, Timing attacks, Analytic attacks
* Cryptanalysis of DES: differential, linear, breaking DES
* Improvements of DES: 3-DES, GDES, DES-X, AES
* DES modes: ECB, CBC, CFB, OFB, CTR
* Electronic Code Book (ECB): Advantages and Limitations
* Cipher Block Chaining (CBC): Advantages and Limitations
* Cipher FeedBack (CFB): Advantages and Limitations
* Output FeedBack (OFB): Advantages and Limitations
* Counter (CTR): Advantages and Limitations
* Triple DES (3DES): Single key, two keys, and three keys
* Why not 2DES? Meet-in-the-middle attack

#### 09 Advanced Encryption Standard (AES), Stream Ciphers and Random Number Generators

* Motivation for AES
* Rijndael
* Structure AES
* Round AES
* Byte Substitution
* Shift Rows
* Mix Columns
* Rijndael Algebra
* Round Keys and Key expansion * AES Decryption
* Stream Ciphers
* RC4
* Random number generation


#### 10 Cryptanalysis

* Shannon’s maxim
* Kerckhofs’s principle
* Types of attack
* Ciphertext only, known-plaintext, chosen-plaintext, chosen-ciphertext, related-key, adaptive * Frequency analysis of the text
* Kasiski test
* Friedman test – index of coincidence
* Linear cryptanalysis
* Differential cryptanalysis
* Typical attack for symmetric ciphers
* Typical attacks fro asymmetric ciphers
* Side channel attacks
* Quantum computers


#### 11 Digital Signatures

* Requirements for digital signature * Algorithms
* Trapdoor
* Signing the hash
* Illustration
* Direct digital signatures
* Arbitrated digital signatures
* Authentication protocols
* Mutual authentication
* One-way authentication
* Replay attacks
* Symmetric encryption approaches
* Needham-Schroeder protocol
* Denning protocol
* Asymmetric approaches
* Denning AS
* Woo and Lam
* Digital Signature standard
* DSA


#### 12 Cryptographic Hash Functions and Applications

* Properties of the Hash function * Use of the hash functions
* Examples
* Resistance and Difficulty
* Birthday problem and rainbow table
* Hash-functions
* Merkle-Damgard
* Hash Algorithms
* SHA
* Applications
* Voice 2G/3G/4G * Mobile data
* WiMax
* Wi-Fi
* Bluetooth
* RFID
* Sensor Networks
* Zigbee
* Embedded technologies
* Linux
* Email
* Data storage security
* Cryptocurrency
* Blockchains
