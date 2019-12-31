# IDelegatableToken.sol

View Source: [contracts/interfaces/delegation/IDelegatableToken.sol](../contracts/interfaces/delegation/IDelegatableToken.sol)

**↘ Derived Contracts: [SkaleToken](SkaleToken.md)**

**IDelegatableToken**

Token that can be used for delegation, unlocked

## Functions

- [getLockedOf(address wallet)](#getlockedof)
- [getDelegatedOf(address wallet)](#getdelegatedof)

### getLockedOf

⤿ Overridden Implementation(s): [SkaleToken.getLockedOf](SkaleToken.md#getlockedof)

returns if the token is locked

```js
function getLockedOf(address wallet) external nonpayable
returns(bool)
```

**Returns**

true if token is locked

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address | of the wallet | 

### getDelegatedOf

⤿ Overridden Implementation(s): [SkaleToken.getDelegatedOf](SkaleToken.md#getdelegatedof)

returns if the token is delegated

```js
function getDelegatedOf(address wallet) external nonpayable
returns(bool)
```

**Returns**

true if the token is delegated

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address | address of the wallet | 

