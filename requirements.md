# Requirements

- Write a contract that accepts as input a list of desired bonds for example
  bonds number 1110 and 1111 when the current number of bonds is 1031
- The contract must be able to bond chicken ([ChickenBondManager.sol#createBond](https://github.com/liquity/ChickenBond/blob/main/LUSDChickenBonds/src/ChickenBondManager.sol)) in the following way:
  - It has had bonded until 1011
  - It must at least bond 100USD
  - Things to be checked
    - There is a minimum amount of provided ETH for which I can bond
    - Makes sure that when the transaction is executed the chicken 1011 is
      obtained

# Links

- [Chicken bond documentation](https://docs.chickenbonds.org/documentation/technical-resources)
- [BOND_NFT_ADDRESS: 0xa8384862219188a8f03c144953Cf21fc124029Ee](https://etherscan.io/address/0xa8384862219188a8f03c144953Cf21fc124029Ee)
- [CHICKEN_BOND_MANAGER_ADDRESS: 0x57619FE9C539f890b19c61812226F9703ce37137](https://etherscan.io/address/0x57619FE9C539f890b19c61812226F9703ce37137)
- [Github](https://github.com/liquity/ChickenBond)
