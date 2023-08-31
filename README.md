# XYZ PUB Crypto Scanner

XYZ PUB Crypto Scanner is a PyQt5-based tool for scanning Bitcoin wallets and deriving wallet information. It supports both online and offline modes of operation.

Python script for generating and checking Bitcoin addresses derived from a mnemonic (BIP39) using the hdwallet library. It includes various functions for formatting and displaying text in different colors.


## QTxpub.py

![image](https://github.com/Mizogg/XYZ-pub-Scanner/assets/88630056/d03b68b3-0cfc-4d41-84c1-535c40451e0f)


## xpubscan.py

![image](https://github.com/Mizogg/XYZ-pub-Scanner/assets/88630056/70aaa45b-9aff-49ff-af28-674500e40112)

The script prompts the user to either enter a mnemonic manually or generate one randomly.

If the user chooses to enter a mnemonic, it validates the input and proceeds with the main logic. 

If the user chooses to generate a random mnemonic, the script allows the user to select the number of words (12, 15, 18, 21, or 24) and the language (English, French, Italian, Spanish, Chinese Simplified, Chinese Traditional, Japanese, or Korean).

After obtaining the mnemonic, the script performs the following steps:

Checks the initial account extended public key for balances and other information using an API.

Displays the account extended private key, account extended public key, and initial balance information.

If any balance or important value is found in the initial account extended public key, it proceeds to derive child keys from different derivation paths and checks their balances and other information.

For each derived key, it displays the derivation path, compressed and uncompressed addresses, balances, total received, total sent, number of transactions, mnemonic words, private key, root public key, extended private key, root extended private key, compressed public key, uncompressed public key, WIF private key, and WIF compressed private key.

If any balance or important value is found in any of the derived keys, it logs the information to a file.


![image](https://github.com/Mizogg/XYZ-pub-Scanner/assets/88630056/b3443666-b0e5-4c89-9740-78c238654380)

Screenshot 1 Description: The application's main interface, English version Scanning Online Random Mnemonic.

![image](https://github.com/Mizogg/XYZ-pub-Scanner/assets/88630056/282b0a98-1380-4e4d-8601-027822830054)

Screenshot 2 Description: Russian version scanning in sequence looking for missing Mnemonic Words.

## Installation

1. Clone the repository:

   ```
   $ git clone https://github.com/Mizogg/XYZ-pub-Scanner.git
   $ cd XYZ-pub-Scanner
2. Install the required dependencies:

  ```
$ pip install -r requirements.txt
```
3. Run the application:

```
$ python QTXpub.py

or

$ python xpubscan.py
```
## Features
Supports both online and offline mode
Scans Bitcoin wallets and derives wallet information
Displays address balances, total received, total sent, and transaction history
Provides mnemonic words, private keys, root public keys, extended private keys, and more
## Usage
Enter the mnemonic phrase in the provided field.
Select the mode (online or offline) for scanning.
Click on the "Start Scan" button to begin the scanning process.
The tool will derive wallet information and display it in the output area.
For online mode, the tool will also check the account extended public key for balance and other important values.
If balance or important values are found, the tool will save the information in the "WINNER_found.txt" file.
The tool supports sequential and random modes for key derivation.
## Contributing
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

## Fork the repository.
Create a new branch for your feature or bug fix.
Make your changes and commit them.
Push your changes to your forked repository.
Open a pull request, describing your changes in detail.
## License
This project is licensed under the MIT License. See the LICENSE file for more information.
