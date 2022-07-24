


What is an Ethereum address?

An Ethereum address is your identity on the blockchain, and it looks like this “0x6E0d01A76C3Cf4288372a29124A26D4353EE51BE”. Having a valid Ethereum address is required for:

Receiving/Sending Ethereum currency
Signing/Sending transactions
Connecting to decentralized applications

Consider an Ethereum address as your username and a corresponding private key as the password. While your Ethereum address is public and can be shared, the private key must always be kept secret.

How an Ethereum address is generated:

A random private key of 64 (hex) characters (256 bits / 32 bytes) is generated first.

The Keccak-256 hash function is then applied to (128 characters / 64 bytes) the public key to obtain a 64 character (32 bytes) hash string. The last 40 characters / 20 bytes of this string prefixed with 0x become the final Ethereum address. 

What is ethers.js?

Ethers.js is considered by some to be more stable and less buggy than other libraries and has extensive documentation. This library is also very friendly to beginners. Ethers.js is very well maintained and is preferred over Web3.js by many new developers.

If node.js is properly installed on your computer, let’s add the ethers.js library using npm (Node Package Manager, a part of node.js).

=== npm install ethers ====

f ethers.js is successfully installed, let’s proceed with creating an Ethereum address.

Create a file named address.js or name it any file name of your choice, which will be a short script to create a random private key and an Ethereum address from that key. check out the code in this project.

Explanation of the code above

Line 1-2: Importing ethers library and crypto module that comes with node.js

Line 4: Generating a random 32 bytes hexadecimal string using the crypto object and storing it in the id variable.

Line 4: Adding ‘0x’ prefix to the string in id and storing the new string in a variable called privateKey.

Line 6: Printing our private key with a warning.

Line 8: Creating a new wallet using the privateKey and storing it in the wallet variable.

Line 9: Printing the address of the newly created wallet with a message “Address:”

Go to your terminal on your VS Code or computer and type this command line "node address or the name of the file your name your code implementation" and then you will see your Ethereum address.

