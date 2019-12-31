# ISkaleToken.sol

View Source: [contracts/interfaces/ISkaleToken.sol](../contracts/interfaces/ISkaleToken.sol)

**ISkaleToken**

interface of SKALE Token

## Functions

- [transfer(address to, uint256 value)](#transfer)
- [mint(address operator, address account, uint256 amount, bytes userData, bytes operatorData)](#mint)
- [CAP()](#cap)

### transfer

Moves `value` tokens from the caller's account to `address`.
    *

```js
function transfer(address to, uint256 value) external nonpayable
returns(success bool)
```

**Returns**

a boolean value indicating whether the operation succeeded.

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| to | address | Address to transfer SKALE tokens | 
| value | uint256 | Transferred token Value | 

### mint

mint - create some amount of token and transfer it to specify address

```js
function mint(address operator, address account, uint256 amount, bytes userData, bytes operatorData) external nonpayable
returns(bool)
```

**Returns**

success of function call.

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| operator | address | address operator requesting the transfer | 
| account | address | - address where some amount of token would be created | 
| amount | uint256 | - amount of tokens to mine | 
| userData | bytes | bytes extra information provided by the token holder (if any) | 
| operatorData | bytes | bytes extra information provided by the operator (if any) | 

### CAP

```js
function CAP() external view
returns(uint256)
```

