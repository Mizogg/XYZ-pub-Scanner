# XYZ PUB Crypto Scanner

XYZ PUB Crypto Scanner is a PyQt5-based tool for scanning Bitcoin wallets and deriving wallet information. It supports both online and offline modes of operation.

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
