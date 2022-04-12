# lq-test
## Install
#### Installation
```
npm install
```

## Test
```
npx hardhat test
````

#### Test Result
```
  SplitPayment
    ✓ only owner should update accounts 
    ✓ should withdraw correct amount of eth to accounts
    ✓ should withdraw correct amount of token to accounts
```

#### Gas Report
```
·-----------------------------------|----------------------------|-------------|-----------------------------·
|        Solc version: 0.8.4        ·  Optimizer enabled: false  ·  Runs: 200  ·  Block limit: 30000000 gas  │
····································|····························|·············|······························
|  Methods                                                                                                   │
·················|··················|··············|·············|·············|···············|··············
|  Contract      ·  Method          ·  Min         ·  Max        ·  Avg        ·  # calls      ·  usd (avg)  │
·················|··················|··············|·············|·············|···············|··············
|  MockERC20     ·  approve         ·           -  ·          -  ·      46894  ·            1  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  MockERC20     ·  transfer        ·           -  ·          -  ·      52417  ·            3  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  SplitPayment  ·  deposit         ·           -  ·          -  ·      67725  ·            1  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  SplitPayment  ·  depositToken    ·           -  ·          -  ·     108184  ·            1  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  SplitPayment  ·  updateAccounts  ·           -  ·          -  ·      65520  ·            1  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  SplitPayment  ·  withdraw        ·           -  ·          -  ·      35270  ·            4  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  SplitPayment  ·  withdrawToken   ·       60093  ·      64893  ·      62493  ·            2  ·          -  │
·················|··················|··············|·············|·············|···············|··············
|  Deployments                      ·                                          ·  % of limit   ·             │
····································|··············|·············|·············|···············|··············
|  MockERC20                        ·           -  ·          -  ·    1229303  ·        4.1 %  ·          -  │
····································|··············|·············|·············|···············|··············
|  SplitPayment                     ·           -  ·          -  ·    1715481  ·        5.7 %  ·          -  │
·-----------------------------------|--------------|-------------|-------------|---------------|-------------·

```