# DelegationPeriodManager.sol

View Source: [contracts/delegation/DelegationPeriodManager.sol](../contracts/delegation/DelegationPeriodManager.sol)

**↗ Extends: [Permissions](Permissions.md)**

**DelegationPeriodManager**

Manager handles the values for the stake multiplier <br>
or delegation periods that are supported by the network

## Contract Members
**Constants & Variables**

```js
mapping(uint256 => uint256) public stakeMultipliers;

```

## Functions

- [(address newContractsAddress)](#)
- [getStakeMultiplier(uint256 monthsCount)](#getstakemultiplier)
- [getDelegationPeriods()](#getdelegationperiods)
- [setDelegationPeriod(uint256 monthsCount, uint256 stakeMultiplier)](#setdelegationperiod)
- [removeDelegationPeriod(uint256 monthsCount)](#removedelegationperiod)
- [isDelegationPeriodAllowed(uint256 monthsCount)](#isdelegationperiodallowed)

### 

constructor which registers newContractsAddress

```js
function (address newContractsAddress) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address | new contract address to register for permissions | 

### getStakeMultiplier

Returns the stake multiplier for this delegation period  <br>
A multiplier to calculate the various yields per delegation period. e.g. 3m = 1, 6m = 1.5, 12m = 2

```js
function getStakeMultiplier(uint256 monthsCount) external view
returns(uint256)
```

**Returns**

the stake multiplier for this delegation period

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| monthsCount | uint256 |  | 

### getDelegationPeriods

Returns the set of allowed delegation period

```js
function getDelegationPeriods() external nonpayable
returns(uint256[])
```

**Returns**

All allowed delegation periods

### setDelegationPeriod

checks whether the delegation period is allowed in the system

```js
function setDelegationPeriod(uint256 monthsCount, uint256 stakeMultiplier) external nonpayable onlyOwner 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| monthsCount | uint256 | delegation period | 
| stakeMultiplier | uint256 |  | 

### removeDelegationPeriod

removes a delegation period from the stake multiplier. </br>

```js
function removeDelegationPeriod(uint256 monthsCount) external nonpayable onlyOwner 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| monthsCount | uint256 | delegation period | 

### isDelegationPeriodAllowed

checks whether the delegation period is allowed in the system

```js
function isDelegationPeriodAllowed(uint256 monthsCount) public view
returns(bool)
```

**Returns**

true if delegation period is allowed

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| monthsCount | uint256 | delegation period | 

