# Audio Cryptogrpahy Using LA concepts
This project aims to develop a robust technique for encoding and decoding audio signals in a manner that securely conceals sensitive information within the audio using linear algebraic concepts such as orthogonal projection, rotation, inversion, and QR decomposition. Additionally, this project incorporates strong encryption techniques, including wrap key encryption.

Utilizing Python libraries such as NumPy, we have successfully implemented the necessary matrix operations and calculations required to generate an encryption key, create an orthogonal matrix, and generate a wrap key. By combining these techniques, we have created a solution that is both secure and effective.

**Project Workflow**

The project is structured into four main sections: encryption key generation, wrap key generation, encryption, and decryption.

Encryption Key Generation: To illustrate the concepts of linear algebra, we have utilized an encryption key represented as a random n × n orthogonal matrix. This matrix is obtained by performing QR decomposition on the inverse of a randomly generated n × n matrix.

Wrap Key Generation: The concept of using a wrap key is to introduce elements of steganography, thereby increasing the difficulty of identifying the original encryption key. The wrap key is generated by rotating the encryption key by 90 degrees and performing a projection about the origin. By applying a 90-degree rotation to the encryption key and projecting it about the origin, we achieve an additional layer of complexity that enhances the security of the overall encryption process.

Encryption: The original encryption key is multiplied with each block of size nx1 of the input audio signal. 

Decryption: The encrypted signal is broken into nx1 blocks and multiplied with the transpose of the original encryption key.

**How to use**

Download the male.wav file, make note of the location of this file. Download the .py file and open with any python supported application. In the "#open audio file", replace the given file with the location of the male.wav file. Upon running the respected output signal as well as the graphs should be displayed. 
Please note any other .wav file can also be used. For better encryption changes to the encryption can be made with accordance to the type of .wav file used.
