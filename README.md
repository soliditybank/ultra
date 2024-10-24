# ULTRA (work in progress)
Military-grade security for your onchain operations.

## FROM A SECURE COMPUTER (e.g. air-gapped computer):
In the terminal:
  - $ mkdir soliditybank && cd soliditybank
  - $ git clone https://github.com/soliditybank/ultra.git
  - $ npx http-server ./ultra -o -p 9999
  - It will prompt you to install the 'http-server' package if it isn't already installed.

In the browser:
  - 'keygen.html' generates a - truly random - private key and its address.
  - 'wallet.html' creates a new wallet or recover an old one from the private key, the passphrase or the seed. This wallet is stored locally in your browser and will be used any time you sign a transaction.
  - 'sign.html' creates and signs a transaction with your stored wallet. A QR of the signature is generated.

### Other server options (not tested)

**PYTHON**

  $ cd ./ultra
  
  $ python3 -m http.server 9999
  
  // On Windows, try "python -m http.server" or "py -3 -m http.server"

  **PHP**
  
  $ cd ./ultra
  
  $ php -S localhost:9999

## IMPORTANT
Your address must be funded with enough ether to cover the network fee.

## FROM ANY DEVICE (e.g. your phone):
Step 3. Go to https://soliditybank.com/ultra and scan the QR. Or copy/paste the signature.

Step 4. Execute the transaction and wait for confirmation.

## Possible Issues
Insufficient ether in your address to pay the network fee.

Transaction nonce is already used. Check the current nonce of your address before signing the transaction.

## ethers.js library
'/lib/ethers.min.js' is a copy of https://cdnjs.cloudflare.com/ajax/libs/ethers/6.7.0/ethers.min.js
