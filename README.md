# Encryption-and-Decryption-in-node-using-Crypto
The Node.js crypto module provides cryptographic operations to help you secure your Node.js application. It supports hashes, HMAC for authentication, ciphers, deciphers, and more.

Q. How is cryptography used in node.js?
 -The answer is simple. To encrypt and decrypt important data so the malicious attackers don't get access to it.

Q. How to actually implement crypto in node?
 -There is an in-built crypto module which allows us to encrypt data in node

Q. How to encrypt data in Node.js
 -you will import the crypto module
 While encrypting data, it’s vital to use an algorithm. In this project, we use aes-256-cbc.

 The crypto.randomBytes() method is used to generate cryptographically built random data generated in the written code.

 The initVector (initialization vector) is used here to hold 16 bytes of random data from the randomBytes() method, and Securitykey contains 32 bytes of random data.

 To encrypt the data, the cipher function is used. Our project’s cipher function is made using createCipheriv(), the initialization vector from the crypto module.

 Pass the first argument as the algorithm we are using, the second argument as the Securitykey, and initVector as the third argument.

 To encrypt the message, use the update() method on the cipher. Pass the first argument as the message, the second argument as utf-8 (input encoding), and hex (output encoding) as the third argument.

 The code tells cipher to stop the encryption using the final() method. When the final() method is called, the cipher can’t be used once more to encrypt data.

 Decrypting data follows a similar format to that of encrypting data. In our Node.js project, we will use the decipher function to decrypt data. Thus, our project encrypts and decrypts data.
