# ITokenSaleManager.sol

View Source: [contracts/interfaces/tokenSale/ITokenSaleManager.sol](../contracts/interfaces/tokenSale/ITokenSaleManager.sol)

**↘ Derived Contracts: [TokenSaleManager](TokenSaleManager.md)**

**ITokenSaleManager**

Token Sale Manager will initially hold all tokens for the sale and allow users to retrieve them

## Functions

- [approve(address[] walletAddress, uint256[] value)](#approve)
- [retrieve()](#retrieve)
- [registerSeller(address seller)](#registerseller)

### approve

⤿ Overridden Implementation(s): [TokenSaleManager.approve](TokenSaleManager.md#approve)

Allocates values for `walletAddresses` <br>
At the end of the sale token approval function will be called (can be called multiple times)

```js
function approve(address[] walletAddress, uint256[] value) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| walletAddress | address[] | array of addresses that the tokens will be sent | 
| value | uint256[] | array of the values of the tokens that will be sent to each address | 

### retrieve

⤿ Overridden Implementation(s): [TokenSaleManager.retrieve](TokenSaleManager.md#retrieve)

Transfers the entire value to sender address. Tokens are locked. <br>
Each sale participant calls retrieve() - the entire value is transferred to walletAddress<br>
After the transfer, the token in walletAddress will be locked through DelegationService contract<br>
User will be able to see the token in the wallet.

```js
function retrieve() external nonpayable
```

### registerSeller

⤿ Overridden Implementation(s): [TokenSaleManager.registerSeller](TokenSaleManager.md#registerseller)

Allows seller address to approve tokens transfers

```js
function registerSeller(address seller) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| seller | address | seller address of the wallet | 

