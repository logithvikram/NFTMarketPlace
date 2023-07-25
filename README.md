# NFT Marketplace Smart Contract

## Description

This is a decentralized Non-Fungible Token (NFT) marketplace smart contract built on the Ethereum blockchain. It allows users to mint new NFT tokens, list them for sale, and purchase NFTs from other users using cryptocurrency.


## Contract Details

The smart contract is implemented in Solidity and is based on the ERC-721 and ERC-721URIStorage standards. It uses the OpenZeppelin library for safe and standard token implementations.

### Main Features

- **Create NFT Token**: Allows users to create new NFT tokens by specifying the token URI and the initial price.

- **List NFT for Sale**: Users can list their NFTs for sale by providing the NFT token ID and the desired sale price.

- **Resell NFT**: Owners of NFTs can choose to resell their tokens by updating the sale price.

- **Purchase NFT**: Users can purchase NFTs listed for sale by paying the specified price in cryptocurrency.

### Ownership and Listing Price

The smart contract has an owner who has special privileges, such as updating the listing price for creating and reselling NFTs.

### Modifiers

- `onlyOwner`: Ensures that only the owner of the marketplace can change the listing price.

## Usage

### Update Listing Price

The owner of the marketplace can update the listing price for creating and reselling NFTs. Use the following function:

### List NFT for Sale

Owners can list their NFTs for sale using the `createMarketItem` function, providing the NFT token ID and the desired sale price:


### Resell NFT

Owners can update the sale price and resell their NFTs using the `resellToken` function:


### Purchase NFT

To purchase an NFT listed for sale, send the required amount of cryptocurrency to the contract using the `createmarketsale` function:


### Fetch NFTs

Various functions are available to fetch NFT data:

- `fetchMarketItem`: Get unsold NFTs listed on the marketplace.

- `fetchMyNFT`: Get NFTs owned by the caller.

- `fetchItemsListed`: Get NFTs listed for sale by the caller.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.







