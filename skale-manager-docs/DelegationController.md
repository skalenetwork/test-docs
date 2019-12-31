# DelegationController.sol

View Source: [contracts/delegation/DelegationController.sol](../contracts/delegation/DelegationController.sol)

**↗ Extends: [Permissions](Permissions.md)**

**DelegationController**

Delegation Controller for executing delegation events

## Structs
### Delegation

```js
struct Delegation {
 address holder,
 uint256 validatorId,
 uint256 amount,
 uint256 delegationPeriod,
 uint256 created,
 string info
}
```

## Contract Members
**Constants & Variables**

```js
//public members
struct DelegationController.Delegation[] public delegations;
mapping(uint256 => uint256) public effectiveDelegationsTotal;
mapping(uint256 => uint256) public delegationsTotal;

//private members
mapping(address => uint256) private _locks;
mapping(address => uint256[]) private _delegationsByHolder;

```

## Modifiers

- [checkDelegationExists](#checkdelegationexists)

### checkDelegationExists

```js
modifier checkDelegationExists(uint256 delegationId) internal
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

## Functions

- [(address newContractsAddress)](#)
- [lock(address holder, uint256 amount)](#lock)
- [unlock(address holder, uint256 amount)](#unlock)
- [getLocked(address holder)](#getlocked)
- [delegate(uint256 delegationId)](#delegate)
- [addDelegation(address holder, uint256 validatorId, uint256 amount, uint256 delegationPeriod, uint256 created, string info)](#adddelegation)
- [unDelegate(uint256 validatorId)](#undelegate)
- [getDelegationsByHolder(address holder)](#getdelegationsbyholder)
- [getDelegation(uint256 delegationId)](#getdelegation)

### 

DelegationController constructor

```js
function (address newContractsAddress) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address | registers for Permissions | 

### lock

```js
function lock(address holder, uint256 amount) external nonpayable allow 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 
| amount | uint256 |  | 

### unlock

```js
function unlock(address holder, uint256 amount) external nonpayable allow 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 
| amount | uint256 |  | 

### getLocked

```js
function getLocked(address holder) external nonpayable
returns(uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 

### delegate

with this function validator finalizes the approval of a delegation request

```js
function delegate(uint256 delegationId) external nonpayable allow 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation requests | 

### addDelegation

```js
function addDelegation(address holder, uint256 validatorId, uint256 amount, uint256 delegationPeriod, uint256 created, string info) external nonpayable allow 
returns(delegationId uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 
| validatorId | uint256 |  | 
| amount | uint256 |  | 
| delegationPeriod | uint256 |  | 
| created | uint256 |  | 
| info | string |  | 

### unDelegate

undelegates a delegation from validator

```js
function unDelegate(uint256 validatorId) external view
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | Id of the validator | 

### getDelegationsByHolder

```js
function getDelegationsByHolder(address holder) external view
returns(uint256[])
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 

### getDelegation

```js
function getDelegation(uint256 delegationId) public view checkDelegationExists 
returns(struct DelegationController.Delegation)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

