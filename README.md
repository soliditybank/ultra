# ULTRA
Military-grade security for your onchain transactions.

## FROM A SECURE COMPUTER (e.g. air-gapped computer):
Step 1. A local web server is needed to run the web application.
  - git clone https://github.com/soliditybank/ultra.git
  - move files to the web server folder.
  - run the server and open localhost:port in the browser

Step 2. Open the 'index.html' file on a browser offline. Choose an action:
  - 'keygen.html' generates a - truly random - private key and its address.
  - 'wallet.html' offers various ways to create a new wallet. This wallet is stored locally in your browser and will be used any time you sign a transaction.
  - 'sign.html' creates and signs a transaction with your stored wallet. A QR of the signature is generated.

### How to start a server
  $ mkdir soliditybank
  
  $ cd soliditybank
  
  $ git clone https://github.com/soliditybank/ultra.git

**NODEJS**
  $ npx http-server /path/to/soliditybank/ultra -o -p 9999

**PYTHON**
  $ cd /path/to/soliditybank/ultra
  
  $ python3 -m http.server 9999
  
  // On Windows, try "python -m http.server" or "py -3 -m http.server"

  **PHP**
  $ cd /path/to/soliditybank/ultra
  
  $ php -S localhost:9999

## IMPORTANT
Your address must be funded with enough Ether to cover the transaction fee.

## FROM ANY DEVICE (e.g. your phone):
Step 3. Go to https://soliditybank.com/ultra and scan the QR. Or copy/paste the signature.

Step 4. Execute the transaction and wait for confirmation.

## Possible Issues
Insufficient ether in your address to pay the network fee.

Transaction nonce is already used. Check the current nonce of your address before signing the transaction.

## ethers.js library
'/lib/ethers.min.js' is a copy of the code on https://cdnjs.cloudflare.com/ajax/libs/ethers/6.7.0/ethers.min.js
