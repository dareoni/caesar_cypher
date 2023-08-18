# caesar_cypher

This code is an implementation of a simple text encryption technique known as the Caesar cipher. It takes an input message, a shift key, and an output file name from the user, and then encrypts the message using the Caesar cipher with the specified shift key. The encrypted message is then written to the specified output file.

Let's break down the code step by step:

User Input:

message: The plaintext message that the user wants to encrypt.
key: An integer representing the shift key. This key determines how much each letter in the plaintext message is shifted to create the encrypted message.
outputFileName: The name of the output file where the encrypted message will be written.
Alphabet and Shifted Alphabet:

The alphabet variable contains the set of characters that can be encrypted (uppercase and lowercase letters along with a space character).
The shiftedAlphabetStart and shiftedAlphabetEnd variables represent the parts of the alphabet after and before the shift, respectively. This is used to create the shifted alphabet for encryption.
Encryption Process:

The encryptedMessage variable is initially an empty string that will store the encrypted version of the input message.
The code iterates through each character in the message.
For each character, it finds the index of that character in the alphabet using the alphabet.find(character) method.
It then retrieves the corresponding character from the shiftedAlphabet and appends it to the encryptedMessage.
Writing Encrypted Message to File:

The encrypted message is printed to the console using the print() function.
The code opens the specified outputFileName in write mode using open(outputFileName, "w").
It prints the encrypted message to the output file using print(encryptedMessage, file=outputFile).
Finally, it closes the output file using outputFile.close().
Output:

After encryption, the encrypted message is printed to the console.
The encrypted message is also written to the specified output file.
Note:

There's a minor typo in the code. In the last print statement, it should be outputFileName instead of outputFilename.
Overall, this code demonstrates a basic example of text encryption using the Caesar cipher technique. It's a straightforward illustration of how a simple encryption algorithm can be implemented in Python to transform a given message using a shift key and write the result to a file.





