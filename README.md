# cryptoMagic
This is an encrypting / decrypting utility for Linux.

1.This utility will take any ASCII file and encrypt it in such a way that its contents are not readable – until they are decrypted by the utility.

    a. The utility has 2 command-line switches – they are –encrypt and –decrypt
    b. If none of these switches is specified, then –encrypt is assumed
    c. The utility also takes the name of an ASCII input file to encrypt/decrypt as an argument.
    d. For example:
        cryptoMagic –encrypt myFile.txt  will encrypt the contents of the myFile.txt file
        cryptoMagic myFile.txt  will encrypt the contents of the myFile.txt file
        cryptoMagic –decrypt myFile.crp  will decrypt the contents of the myFile.crp file
2. When the utility is asked to –encrypt an ASCII file, it will take the input filename and produce the encrypted file with the same base filename and an .crp file extension.

    a. For example:
        cryptoMagic –encrypt myFile.txt  will produce an encrypted file called myFile.crp
3. When the utility is asked to –decrypt an encrypted file, it will take the input filename and produce the decrypted file with the same base filename and an .txt file extension

    a. For example:
        cryptoMagic –decrypt myFile.crp  will produce a decrypted file called myFile.txt
