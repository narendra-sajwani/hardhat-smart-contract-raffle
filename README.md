# Decentralized Raffle Application

## About

This Project is back-end part (smart contracts deployed over goerli testnet) of fullstack project of Decentralised Raffle Application.

This is an end to end Project which includes Development, Testing and Deployment of smart contracts written in solidity.

In This Project I used multiple <a href="https://chain.link/">Chainlink</a> oracles for Automatically selecting a Random winner from a list of participents in given Interval.

## Functionalities:

-   Constants Variables of the Frontend Project are automatically updated with addresses and ABIs of the contracts after deploying the contracts.
-   Verifies the contracts on etherscan automatically if Contracts are deployed on testnet.
-   Automatically selects Random winner from a List of participents and rewards them with the amount collected by lottery/ raffle contract.
-   Uses <a href="https://docs.chain.link/docs/chainlink-automation/introduction/">Chainlink keepers</a> for Automation.
-   Uses <a href="https://docs.chain.link/docs/vrf/v2/introduction/"> Chainlink VRF</a> for randomly selecting a winner.

<br>

> ### <a href="https://cool-dawn-6357.on.fleek.co/"> Link to my Raffle Application</a>

## Requirements

-   [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
    -   You'll know you did it right if you can run `git --version` and you see a response like `git version x.x.x`
-   [Nodejs](https://nodejs.org/en/)
    -   You'll know you've installed nodejs right if you can run:
        -   `node --version` and get an ouput like: `vx.x.x`
-   [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/) instead of `npm`
    -   You'll know you've installed yarn right if you can run:
        -   `yarn --version` and get an output like: `x.x.x`
        -   You might need to install it with `npm`

## Quickstart

```
git clone https://github.com/narendra-sajwani/hardhat-smart-contract-raffle.git
cd hardhat-smart-contract-raffle
yarn
```

# Usage

Deploy:

```
yarn hardhat deploy
```

## Testing

```
yarn hardhat test
```

# Deployment to a testnet or mainnet

1. Setup environment variabltes

You'll want to set your `GOERLI_RPC_URL` and `PRIVATE_KEY` as environment variables. You can add them to a `.env` file, similar to what you see in `.env.example`.

-   `PRIVATE_KEY`: The private key of your account (like from [metamask](https://metamask.io/)). **NOTE:** FOR DEVELOPMENT, PLEASE USE A KEY THAT DOESN'T HAVE ANY REAL FUNDS ASSOCIATED WITH IT.
    -   You can [learn how to export it here](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key).
-   `GOERLI_RPC_URL`: This is url of the goerli testnet node you're working with. You can get setup with one for free from [Alchemy](https://alchemy.com/?a=673c802981)

2. Get testnet ETH

Head over to [faucets.chain.link](https://faucets.chain.link/) and get some tesnet ETH. You should see the ETH show up in your metamask.

3. Deploy

```
yarn hardhat deploy --network goerli
```

### Checkout My Repo for Frontend of this Project built using Next.js

<a href="https://github.com/narendra-sajwani/nextjs-smartcontract-lottery-fcc.git">Raffle Frontend</a>

# Thank you!
