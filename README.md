# Chicken Bonds
## Deploy locally(anvil):

1. run anvil
2. rename **example.env** to **.env**
3. copy one of private keys in the .env file without double-quote and 0x. If
   deploying to testnet use RPC provided by Alchemy or Infura.

### Deploy to local testnet(anvil)

```bash
forge script script/Contract.s.sol:ContractScript --fork-url http://localhost:8545 --private-key $PRIVATE_KEY  --broadcast
```

### Deploy to goerli testnet

```bash
forge script script/HelloWorld.s.sol:ContractScript --rpc-url ${GOERLI_RPC_URL}  --private-key ${PRIVATE_KEY}
 --broadcast --verify --etherscan-api-key ${ETHERSCAN_API_KEY}  -vvvv
```

Then replace **CONTRACT_ADDRESS** in .env with the contract address provided in
the deploy output log

```bash
✅ Hash: 0xd8ade633b4007d2ca33b0668d5d04d6587b36fd433d7541d8d85b89c5dfcccbc
Contract Address: 0x412077fc61144c436a49025d352ddcc0ee41fe22
Block: 7980326
Paid: 0.00092922428100375 ETH (309735 gas * 3.00006225 gwei)
```

## References
- [Foundry](https://book.getfoundry.sh)
- [Chicken Bonds](https://docs.chickenbonds.org)

