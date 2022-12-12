# Build a Whitelist Dapp for your upcoming NFT Collection

This repo contains coursework project from [LearnWeb3](https://learnweb3.io/) completed by [0xsenzel](https://github.com/0xSenzel/) for [LearnWeb3DAO-Sophomore](https://learnweb3.io/courses/c1d7081b-63a9-4c6e-b35c-9fcbbad418b2) lesson.

## Project Info

Whitelist Dapp give the first 10 users the ability to access exclusive feature to mint NFT on our NFT minting Dapp : [NFT Collection](https://github.com/0xSenzel/nft-collection).

## Project Demo

<figure>
<img src="./my-app/public/demo1.PNG" alt="demo1" style="width:100%">
<p align="center">Fig.1 - Home Page of Whitelist Dapp</p>
</figure>

<br/>

<figure>
<img src="./my-app/public/demo2.PNG" alt="demo1" style="width:100%">
<p align="center">Fig.2 - After User Been Whitelisted</p>
</figure>

## Project Setup

### Hardhat

Head to [hardhat-tutorial](./hardhat-tutorial/) folder:

Install dependencies

```
npm install
```

Compile smart contract

```
npx hardhat compile
```

To deploy smart contracts: <br/>
Head to [hardhat.config.js](./hardhat-tutorial/hardhat.config.js) file, changed the value of `ALCHEMY_HTTP_URL` with your own Ethereum Network API & `PRIVATE_KEY` with Ethereum wallet's private key. Then run the following command.

```
npx hardhat run scripts/deploy.js --network goerli
```

### React & Next Js

Head to [my-app](./my-app/) folder:

```
npm install
```

Replace the variable inside with your respective deployed contract address and contract's compiled abi inside [this folder](./my-app/constants/index.js).

To run the app locally:

```
npm run dev
```
