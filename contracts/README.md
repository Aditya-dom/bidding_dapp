## Deployments

- Auctioneer: [0x6b08b0b3f272108620d9b01242c927e112a99e51](https://sepolia.basescan.org/address/0x6b08b0b3f272108620d9b01242c927e112a99e51)

## Contracts

- Auctioneer.sol: Factory contract for creating and managing Dutch auctions
- DutchAuction.sol: A Dutch auction contract for token ICOs (similar to Liquidity Bootstrapping Pools)
- Token.sol: An ERC20 token contract for the auction

## Tests

- DutchAuctionTest.t.sol
- ReentrancyAttackTest.t.sol

## Commands

### Deploy Auctioneer

```bash
forge script script/deployAuctioneer.sol:DeployAuctioneer --rpc-url $RPC_URL --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY
```

### Test Dutch Auction

```bash
forge test --match-contract DutchAuctionTest -vvvvv
```

### Test Reentrancy Attack

```bash
forge test --match-contract ReentrancyAttackTest -vvvvv
```


