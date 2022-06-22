# Matic Polygon Pizza

### Install dependencies with

```
npm install
```

### Compile

bor-chain-id for Mainnet = 137
bor-chain-id for TestnetV4 (Mumbai) = 80001

```
npm run template:process -- --bor-chain-id <bor-chain-id>
npm run truffle:compile
```

### Start main chain and side chain

- Start Main chain

```
npm run testrpc
```

- Start Matic side chain. Requires docker.

```
npm run bor:simulate
```

- If you ran a bor instance before, a dead docker container might still be lying around, clean it with

```
npm run bor:clean
```

- Run a bor (our matic chain node) instance.

### Deploy Contracts

- For local development

```
npm run truffle:migrate
```

### Run tests

```
npm test
```
