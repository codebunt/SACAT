# Testnet \(Ropsten\) Instructions

These are instructions for interacting with the Beta version of CarboDebt hosted on the Ropsten using Remix and MetaMask

* Download and install [MetaMask](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=en) plugin form Chrome
* Select the Ropsten Test Network within MetaMask \(top menu\)
* Send some Ether to your wallet generated by MetaMask using a [Rposten faucet](https://faucet.ropsten.be/)
* Open [Remix](https://remix.ethereum.org/)
* Use the file explorer to upload flatContract.sol and compile
* From the Deploy and Run Transactions tab set Environment to Injected Web3
* Account in Remix should match wallet address generated by MetaMask with ether from Ropsten faucet \(wait for faucet confirmation\)
* load the following contract using the At Address button

  CarboTag Contract Address

  ```text
    0x198c3aD892b6ee476d3CcA06762cEaa152fcCea8
  ```

* From CarboDebt contract signup using your wallet addresss
* Add debt, createEscrow, createTransaction, etc
* CreateEscrow requires a \_receiver address. Here is an account registered to the network with name "seller"

  ```text
    0xfb645a584cb19d7d3f1dbe77feade85c76388bc3
  ```

* once escrow is created use findEscrowAddr view function to get the new MultiSigWallet address. Inputs are your address and the \_receiver address
* Select the MultiSigWallet contract from the drop down list and using the At Address button to load the external escrow contract
* This contract is use to confirm transactions.
* getTransactionIds function returns the list of pending escrow transactions for a given escrowAddr
* transactionData funciton returns the external transaction id parameter \(within the MultiSigContract\) that must be sent when confirming a transaction
* TODO work on registering the list of escrows linked to each CarboTag waller. see the escrowList address\[\] array within the wallet Attributes. Not showing in Remix.
* TODO build application

