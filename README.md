# Crowd funding

https://user-images.githubusercontent.com/55044734/164529677-27af29f2-96d6-4ce6-bb61-c1f0c63a3beb.mp4

### Project features :bulb:

- [x] User can start a fundraising.
- [x] Anyone can contribute.
- [x] End the project if the targeted contribution amount is reached.
- [x] Expire project if the targeted amount is not fulfilled by the deadline.
- [x] Contributors can withdraw the contributed amount if the project expires.
- [x] The Owner needs to request contributors for withdrawal amount.
- [x] The Owner can withdraw the amount if 50% of contributors agree.
- [x] Connect with the wallet.


### Tech stack & packages used 📦

| package                                                             | explain                                                               |
| ------------------------------------------------------------------- | --------------------------------------------------------------------- |
| [solidity](https://docs.soliditylang.org/en/v0.8.13/)               | For writting smart contracts                                          |
| [tailwind css](https://tailwindcss.com/docs/installation)           | For building design                                                   |       
| [ether.js](https://docs.ethers.io/v5/)                              | Web3 client (contract testing ).                                      |
| [web3.js](https://www.npmjs.com/package/web3)                       | Web3 client (Frontend Next.js).                                       |
| [hardhat](https://www.npmjs.com/package/hardhat)                    | Ethereum development environment.                                     | 


----------------

### How to run :runner: :

- Run hardhat node
    ```
    npx hardhat node
    ```
- Run test cases
    ```
    npx hardhat test
    ```
- Connect HardHat Account to Metamask

https://github.com/Thiru-Malai/Crowdfunding-DAPP/assets/73980589/f694a9ef-a035-4f2a-9763-98c90839e2b9

- Deploy contract in local hardhat node
    ```
    npx hardhat run scripts/deploy.js --network localhost
    ```
- Run Next.js frontend
    ```
    cd client
    npm run dev
    ```
- Connect account to  website


### Web3.js 
------------
- [Load web3](https://web3js.readthedocs.io/en/v1.2.11/web3-eth.html#web3-eth)
- [Connect with contract](https://web3js.readthedocs.io/en/v1.2.11/web3-eth-contract.html#web3-eth-contract)
    ```
    new web3.eth.Contract(jsonInterface[, address][, options])
    ```
- [Callback promises events](https://web3js.readthedocs.io/en/v1.2.11/callbacks-promises-events.html#callbacks-promises-events)
    ```
    .on('transactionHash', function(hash){ ... })
    .on('error', function(error){ ... })
    ```
- [Subscribe to event](https://web3js.readthedocs.io/en/v1.2.11/web3-eth-contract.html#contract-events)
    ```
    contractName.events.EventName([options][, callback])
    ```
- [Fetch all data from contract event](https://web3js.readthedocs.io/en/v1.2.11/web3-eth-contract.html#getpastevents)
    - <small> An array with the past event Objects, matching the given event name and filter.</small>

    ```
    contractName.getPastEvents(EventName[, options][, callback])
    ```

### Hardhat commands
```shell
npx hardhat accounts
npx hardhat compile
npx hardhat clean
npx hardhat test
npx hardhat node
node scripts/deploy.js
npx hardhat help
npx hardhat run scripts/deploy.js --network <network name>
```
