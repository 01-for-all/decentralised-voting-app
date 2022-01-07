# Decentralised Election App: 


# Election DAPP-V1.0:

Made a decentralised election app which can be used to conduct elections through mobile or web app. This is just a basic version 1.0.

## Dependencies

- NPM:

```
  
  > nvm use 16.13.0
  > npm install
  > npm run dev
```

- Truffle:

```
  > npm install --g truffle@5.1.39
  > truffle init
  > truffle compile
  > truffle migrate
```

- Ganache: Local Blockchain Network
- Metamask

## Step 1. Install dependencies:

```
> cd election-v1.0
> npm install
```

## Step 2. Start Ganache

Open the `Ganache GUI client` that you downloaded and installed Or use `ganache-cli` .This will start your local blockchain instance.

## Step 3. Compile & Deploy Election Smart Contract:

`> truffle compile`
You must compile election smart contract before migrating it.
`> truffle migrate --reset`
You must migrate the election smart contract each time your restart ganache.

To see the logs: [test/truffle-logs.txt]

## Step 4. Configure Metamask:

- Unlock Metamask
- Connect metamask to your local Etherum blockchain provided by Ganache.
- Import an account provided by ganache.

## Step 5. Run the Front End Application:

`$ npm run dev`
Visit this URL in your browser: http://localhost:3000

### Basic overview of the project structure of Dapp:

- [/election/contracts/migration.sol] : this will handle all of our migration whenever we deploy our smart contracts to the blockchain.
- [/election/migrations] : this is were all the migration files live whenever we deploy our smart contracts to the blockchain. In this, we are changing its state.This same as changing the state of the database.
- [/election/node_modules] : This is were all our node dependecies live.
- [/election/src] : source directory. This is were we develop our client-side app.
- [/election/test] : test files are kept here.
- [/election/package.json] : This is were we specify our depedencies.
- [/election/truffle-config.js] : main conf file for our project.
