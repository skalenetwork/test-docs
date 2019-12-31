# SkaleToken is ERC777 Token implementation, also this contract in skale
manager system (SkaleToken.sol)

View Source: [contracts/SkaleToken.sol](../contracts/SkaleToken.sol)

**↗ Extends: [LockableERC777](LockableERC777.md), [Permissions](Permissions.md), [IDelegatableToken](IDelegatableToken.md)**

**SkaleToken**

## Contract Members
**Constants & Variables**

```js
string public constant NAME;
string public constant SYMBOL;
uint256 public constant DECIMALS;
uint256 public constant CAP;

```

## Functions

- [(address contractsAddress, address[] defOps)](#)
- [mint(address operator, address account, uint256 amount, bytes userData, bytes operatorData)](#mint)
- [slash(address target, uint256 amount)](#slash)
- [getLockedOf(address wallet)](#getlockedof)
- [getDelegatedOf(address wallet)](#getdelegatedof)

### 

```js
function (address contractsAddress, address[] defOps) public nonpayable Permissions LockableERC777 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| contractsAddress | address |  | 
| defOps | address[] |  | 

### mint

mint - create some amount of token and transfer it to specify address

```js
function mint(address operator, address account, uint256 amount, bytes userData, bytes operatorData) external nonpayable allow 
returns(bool)
```

**Returns**

returns success of function call.

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| operator | address | address operator requesting the transfer | 
| account | address | - address where some amount of token would be created | 
| amount | uint256 | - amount of tokens to mine | 
| userData | bytes | bytes extra information provided by the token holder (if any) | 
| operatorData | bytes | bytes extra information provided by the operator (if any) | 

### slash

move `amount` of tokens to SkaleManager

```js
function slash(address target, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| target | address |  | 
| amount | uint256 |  | 

### getLockedOf

⤾ overrides [IDelegatableToken.getLockedOf](IDelegatableToken.md#getlockedof)

See {IDelegatableToken-getLockedOf}.

```js
function getLockedOf(address wallet) external nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address |  | 

### getDelegatedOf

⤾ overrides [IDelegatableToken.getDelegatedOf](IDelegatableToken.md#getdelegatedof)

See {IDelegatableToken-getDelegatedOf}.

```js
function getDelegatedOf(address wallet) external nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address |  | 

