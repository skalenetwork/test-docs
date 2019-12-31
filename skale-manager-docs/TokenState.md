# TokenState.sol

View Source: [contracts/delegation/TokenState.sol](../contracts/delegation/TokenState.sol)

**↗ Extends: [Permissions](Permissions.md)**

**TokenState**

Store and manage tokens states

**Enums**
### State

```js
enum State {
 PROPOSED,
 ACCEPTED,
 DELEGATED,
 ENDING_DELEGATED,
 COMPLETED
}
```

## Contract Members
**Constants & Variables**

```js
mapping(uint256 => enum TokenState.State) private _state;
mapping(uint256 => uint256) private _timelimit;
mapping(address => uint256) private _purchased;
mapping(address => uint256) private _totalDelegated;
mapping(uint256 => bool) private _isPurchased;
mapping(address => uint256[]) private _endingDelegations;

```

## Functions

- [(address _contractManager)](#)
- [getLockedCount(address holder)](#getlockedcount)
- [getDelegatedCount(address holder)](#getdelegatedcount)
- [sold(address holder, uint256 amount)](#sold)
- [accept(uint256 delegationId)](#accept)
- [requestUndelegation(uint256 delegationId)](#requestundelegation)
- [cancel(uint256 delegationId)](#cancel)
- [getState(uint256 delegationId)](#getstate)
- [getPurchasedAmount(address holder)](#getpurchasedamount)
- [setState(uint256 delegationId, enum TokenState.State newState)](#setstate)
- [initProposed(uint256 delegationId)](#initproposed)
- [isLocked(enum TokenState.State state)](#islocked)
- [isDelegated(enum TokenState.State state)](#isdelegated)
- [proposedToUnlocked(uint256 delegationId)](#proposedtounlocked)
- [acceptedToDelegated(uint256 delegationId)](#acceptedtodelegated)
- [purchasedProposedToPurchased(uint256 delegationId, struct DelegationController.Delegation delegation)](#purchasedproposedtopurchased)
- [endingDelegatedToUnlocked(uint256 delegationId, struct DelegationController.Delegation delegation)](#endingdelegatedtounlocked)
- [purchasedToUnlocked(address holder)](#purchasedtounlocked)
- [_cancel(uint256 delegationId, struct DelegationController.Delegation delegation)](#_cancel)

### 

```js
function (address _contractManager) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| _contractManager | address |  | 

### getLockedCount

get the total locked amount

```js
function getLockedCount(address holder) external nonpayable
returns(amount uint256)
```

**Returns**

total locked amount

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address | address of the token holder | 

### getDelegatedCount

get the total delegated amount

```js
function getDelegatedCount(address holder) external nonpayable
returns(amount uint256)
```

**Returns**

total delegated amount

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address | address of the token holder | 

### sold

```js
function sold(address holder, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 
| amount | uint256 |  | 

### accept

```js
function accept(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### requestUndelegation

```js
function requestUndelegation(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### cancel

```js
function cancel(uint256 delegationId) external nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### getState

get the final state of the delegation request

```js
function getState(uint256 delegationId) public nonpayable
returns(state enum TokenState.State)
```

**Returns**

state final state of the token

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation | 

### getPurchasedAmount

```js
function getPurchasedAmount(address holder) public nonpayable
returns(amount uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 

### setState

modifies the token state

```js
function setState(uint256 delegationId, enum TokenState.State newState) internal nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegator | 
| newState | enum TokenState.State | state of the delegatedToken | 

### initProposed

```js
function initProposed(uint256 delegationId) internal nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### isLocked

```js
function isLocked(enum TokenState.State state) internal nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| state | enum TokenState.State |  | 

### isDelegated

```js
function isDelegated(enum TokenState.State state) internal nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| state | enum TokenState.State |  | 

### proposedToUnlocked

```js
function proposedToUnlocked(uint256 delegationId) internal nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### acceptedToDelegated

```js
function acceptedToDelegated(uint256 delegationId) internal nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### purchasedProposedToPurchased

```js
function purchasedProposedToPurchased(uint256 delegationId, struct DelegationController.Delegation delegation) internal nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 
| delegation | struct DelegationController.Delegation |  | 

### endingDelegatedToUnlocked

```js
function endingDelegatedToUnlocked(uint256 delegationId, struct DelegationController.Delegation delegation) internal nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 
| delegation | struct DelegationController.Delegation |  | 

### purchasedToUnlocked

```js
function purchasedToUnlocked(address holder) internal nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 

### _cancel

```js
function _cancel(uint256 delegationId, struct DelegationController.Delegation delegation) internal nonpayable
returns(state enum TokenState.State)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 
| delegation | struct DelegationController.Delegation |  | 

