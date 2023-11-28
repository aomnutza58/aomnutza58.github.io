# asymmetric encryption

## What is asymmetric encryption?

There are two sides in an encrypted communication: the sender, who encrypts the data, and the recipient, who decrypts it. As the name implies, asymmetric encryption is different on each side; the sender and the recipient use two different keys. Asymmetric encryption, also known as public key encryption, uses a public key-private key pairing: data encrypted with the public key can only be decrypted with the private key.

TLS (or SSL), the protocol that makes HTTPS possible, relies partially on asymmetric encryption. A client will obtain a website's public key from that website's TLS certificate (or SSL certificate) and use that to initiate secure communication. The website keeps the private key secret.

## What is asymmetric cryptography?

Asymmetric cryptography, also known as public-key cryptography, is a process that uses a pair of related keys -- one public key and one private key -- to encrypt and decrypt a message and protect it from unauthorized access or use.

A public key is a cryptographic key that can be used by any person to encrypt a message so that it can only be decrypted by the intended recipient with their private key. A private key -- also known as a secret key -- is shared only with key's initiator.

When someone wants to send an encrypted message, they can pull the intended recipient's public key from a public directory and use it to encrypt the message before sending it. The recipient of the message can then decrypt the message using their related private key.

If the sender encrypts the message using their private key, the message can be decrypted only using that sender's public key, thus authenticating the sender. These encryption and decryption processes happen automatically; users do not need to physically lock and unlock the message.

Many protocols rely on asymmetric cryptography, including the transport layer security (TLS) and secure sockets layer (SSL) protocols, which make HTTPS possible.

The encryption process is also used in software programs that need to establish a secure connection over an insecure network, such as browsers over the internet, or that need to validate a digital signature.

Increased data security is the primary benefit of asymmetric cryptography. It is the most secure encryption process because users are never required to reveal or share their private keys, thus decreasing the chances of a cybercriminal discovering a user's private key during transmission.

## What's the difference between asymmetric vs. symmetric cryptography?

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/6fa62360-ade2-4734-a60d-caf760f5d7cc)

The main difference between asymmetric versus symmetric cryptography is that asymmetric encryption algorithms make use of two different but related keys. One key encrypts data and another key decrypts it. Symmetric encryption uses the same key to perform both encryption and decryption functions.

Another difference between asymmetric and symmetric encryption is the length of the keys. In symmetric cryptography, the length of the keys -- which is randomly selected -- are typically set at 128 bits or 256 bits, depending on the level of security needed.

In asymmetric encryption, there must be a mathematical relationship between the public and private keys. Since malicious actors can potentially exploit this pattern to crack the encryption, asymmetric keys need to be longer to offer the same level of security. The difference in the length of the keys is so pronounced that a 2048-bit asymmetric key and a 128-bit symmetric key provide about an equivalent level of security.

Asymmetric encryption is notably slower than symmetric encryption, which has a faster execution speed.

## How does asymmetric cryptography work?

The main difference between asymmetric versus symmetric cryptography is that asymmetric encryption algorithms make use of two different but related keys. One key encrypts data and another key decrypts it. Symmetric encryption uses the same key to perform both encryption and decryption functions.

![image](https://github.com/aomnutza58/aomnutza58.github.io/assets/86311377/46d99015-6327-4670-b000-9711a30a72a8)

Asymmetric encryption uses a mathematically related pair of keys for encryption and decryption: a public key and a private key. If the public key is used for encryption, then the related private key is used for decryption. If the private key is used for encryption, then the related public key is used for decryption.

The two participants in the asymmetric encryption workflow are the sender and the receiver. Each has its own pair of public and private keys. First, the sender obtains the receiver's public key. Next, the plaintext message is encrypted by the sender using the receiver's public key. This creates ciphertext. The ciphertext is sent to the receiver, who decrypts it with their private key, returning it to legible plaintext.

Because of the one-way nature of the encryption function, one sender is unable to read the messages of another sender, even though each has the public key of the receiver.

## How are asymmetric encryption and symmetric encryption used for TLS/SSL?

TLS, historically known as SSL, is a protocol for encrypting communications over a network. TLS uses both asymmetric encryption and symmetric encryption. During a TLS handshake, the client and server agree upon new keys to use for symmetric encryption, called "session keys." Each new communication session will start with a new TLS handshake and use new session keys.

The TLS handshake itself makes use of asymmetric cryptography for security while the two sides generate the session keys, and in order to authenticate the identity of the website's origin server.

## Uses of asymmetric cryptography

Asymmetric cryptography is typically used to authenticate data using digital signatures. A digital signature is a mathematical technique used to validate the authenticity and integrity of a message, software or digital document. It is the digital equivalent of a handwritten signature or stamped seal.

Based on asymmetric cryptography, digital signatures can provide assurances of evidence to the origin, identity and status of an electronic document, transaction or message, as well as acknowledge informed consent by the signer.

Asymmetric cryptography can also be applied to systems in which many users may need to encrypt and decrypt messages, including:

+ Encrypted email. A public key can be used to encrypt a message and a private key can be used to decrypt it.
+ SSL/TLS. Establishing encrypted links between websites and browsers also makes use of asymmetric encryption.
+ Cryptocurrencies. Bitcoin and other cryptocurrencies rely on asymmetric cryptography. Users have public keys that everyone can see and private keys that are kept secret. Bitcoin uses a cryptographic algorithm to ensure only legitimate owners can spend the funds.

In the case of the Bitcoin ledger, each unspent transaction output (UTXO) is typically associated with a public key. For example, if user X, who has an UTXO associated with his public key, wants to send the money to user Y, user X uses his private key to sign a transaction that spends the UTXO and creates a new UTXO that's associated with user Y's public key.

## What are the benefits and disadvantages of asymmetric cryptography?

The benefits of asymmetric cryptography include:

+ The key distribution problem is eliminated because there's no need for exchanging keys.
+ Security is increased since the private keys don't ever have to be transmitted or revealed to anyone.
+ The use of digital signatures is enabled so that a recipient can verify that a message comes from a particular sender.
+ It allows for nonrepudiation so the sender can't deny sending a message.

Disadvantages of asymmetric cryptography include:

+ It's a slow process compared to symmetric cryptography. Therefore, it's not appropriate for decrypting bulk messages.
+ If an individual loses his private key, he can't decrypt the messages he receives.
+ Because public keys aren't authenticated, no one can ensure a public key belongs to the person specified. Consequently, users must verify that their public keys belong to them.
+ If a malicious actor identifies a person's private key, the attacker can read that individual's messages.

## What are examples of asymmetric cryptography?

The RSA algorithm -- the most widely used asymmetric algorithm -- is embedded in the SSL/TLS, which is used to provide secure communications over a computer network. RSA derives its security from the computational difficulty of factoring large integers that are the product of two large prime numbers.

Multiplying two large primes is easy, but the difficulty of determining the original numbers from the product -- factoring -- forms the basis of public-key cryptography security. The time it takes to factor the product of two sufficiently large primes is beyond the capabilities of most attackers.

RSA keys are typically 1024 or 2048 bits long, but experts believe 1024-bit keys will be broken soon, which is why government and industry are moving to a minimum key length of 2048-bits.

Elliptic Curve Cryptography (ECC) is gaining favor with many security experts as an alternative to RSA. ECC is a public-key encryption technique based on elliptic curve theory. It can create faster, smaller and more efficient cryptographic keys through the properties of the elliptic curve equation.

To break ECC, an attacker must compute an elliptic curve discrete logarithm, which is significantly more difficult problem than factoring. As a result, ECC key sizes can be significantly smaller than those required by RSA while still delivering equivalent security with lower computing power and battery resource usage.

Source : <a href="https://www.techtarget.com/searchsecurity/definition/asymmetric-cryptography">techtarget</a>, <a href="https://www.cloudflare.com/learning/ssl/what-is-asymmetric-encryption/">cloudflare</a>
