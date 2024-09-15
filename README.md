MiniShell

MiniShell is a versatile tool designed for encrypting raw payloads using RC4 or AES algorithms. Developed by Pentesterclub, this utility provides functionalities for encrypting files and generating corresponding decryption functions.


Features

Encryption Options: Supports RC4 and AES encryption algorithms.

Decryption Function Output: Generates the decryption function for the selected encryption type.

Encrypted File Output: Outputs encrypted bytes as a binary file.

Random Key Generation: Automatically generates random keys for the selected encryption algorithms.

Usage

To use MiniShell, you can execute the following command structure:

MiniShell.exe <Input Payload FileName> <Enc *Option*> <Output FileName>

Encryption Options

aes: Encrypts the file using AES-256 with a randomly generated key and initialization vector (IV).

rc4: Encrypts the file using RC4 with a randomly generated key.

Examples

Encrypt a file using RC4 and output the encrypted bytes to a binary file, along with the decryption function to the console:

.\MiniShell.exe .\calc.bin rc4 encpayload.bin

Encrypt a file using RC4, write the encrypted bytes to a binary file, and output the decryption function to a C source file:

.\MiniShell.exe .\calc.bin rc4 encpayload.bin > rc4.c


Encrypt a file using AES, write the encrypted bytes to a binary file, and output the decryption function to the console:

.\MiniShell.exe .\calc.bin aes calcenc.bin


Encrypt a file using AES, write the encrypted bytes to a binary file, and output the decryption function to a C source file:

.\MiniShell.exe .\calc.bin aes calcenc.bin > aes.c

Requirements
Ensure you have the necessary permissions to execute the program.
The input file must be a valid binary file.

Contact
For any inquiries or feedback, please reach out to the project maintainers:

Pentesterclub: @Pentesterclubpvtltd | @alex14324
