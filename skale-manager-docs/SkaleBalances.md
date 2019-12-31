# SkaleBalances.sol

View Source: [contracts/SkaleBalances.sol](../contracts/SkaleBalances.sol)

**↗ Extends: [Permissions](Permissions.md)**

**SkaleBalances**

## Contract Members
**Constants & Variables**

```js
mapping(address => uint256) internal bountyBalances;

```

## Functions

- [(address newContractsAddress)](#)
- [withdrawBalance(uint256 amountOfTokens)](#withdrawbalance)
- [stashBalance(address recipient, uint256 bountyForMiner)](#stashbalance)

### 

```js
function (address newContractsAddress) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address |  | 

### withdrawBalance

```js
function withdrawBalance(uint256 amountOfTokens) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| amountOfTokens | uint256 |  | 

### stashBalance

```js
function stashBalance(address recipient, uint256 bountyForMiner) external nonpayable allow 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| recipient | address |  | 
| bountyForMiner | uint256 |  | 

