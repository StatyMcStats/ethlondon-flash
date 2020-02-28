# ETHLondon Aave Flash Loans workshop

## Setup
- ```docker-compose up``` will start the docker container development environment and the ganache container.
- In a different console, ```docker-compose exec contracts-env bash``` to connect to the running container.
- Inside the container, all the interaction with the smart contracts should be done through the following npm scripts, wrapping truffle framework's features.

## Available npm scripts
The smart contracts' related npm scripts on package.json are prefixed with a network id: **dev:** for Ganache network and **ropsten:** for Ropsten network.

The main available scripts (using the **dev:** prefix as example) are:
- ```npm run compile```: Compiles the Solidity contracts.
- ```npm run dev:migrate```: Executes the migrations for the corresponding network. 
- ```npm run dev:cleanDeploy```: removes the build/ folder of the compiled contracts, compiles them again and executes npm run dev:migrate

## Addresses

### FlashExchange (Ropsten)
0xA211b59A3dbD38614D1700C66E179621eef8319F

### DAI (Ropsten)
0xf80a32a835f79d7787e8a8ee5721d0feafd78108

### ETH Address (Ropsten, Mainnet)
0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE

### FlashExchange (Mainnet)
0xF1d29e94754C897D4e51c13DEA9B27a35C7DD653

## Credits

Thanks to David for the flashloan.sol template 
https://github.com/mrdavey/ez-flashloan