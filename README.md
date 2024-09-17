# ULTRA
Military-grade security for your onchain transactions.

## FROM A SECURE COMPUTER (e.g. air-gapped computer):
Step 1. git clone https://github.com/soliditybank/ultra.git

Step 2. Open the 'index.html' file on a browser offline. Choose an action:

'keygen.html' generates a - truly random - private key and its address.

'new-wallet.html' creates a new wallet and stores it locally in your browser.file and paste the private key or choose another option to create your new wallet. This wallet is stored locally in your browser and will be used any time you sign a transaction.

'sign.html' creates and sign a transaction. A QR of the signature is generated.

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
