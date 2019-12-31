# DelegationRequestManager.sol

View Source: [contracts/delegation/DelegationRequestManager.sol](../contracts/delegation/DelegationRequestManager.sol)

**↗ Extends: [Permissions](Permissions.md)**

**DelegationRequestManager**

Handles Delegation Requests <br>
Requests are created/canceled by the delegator <br>
Requests are accepted by the validator

## Functions

- [(address newContractsAddress)](#)
- [createRequest(address holder, uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info)](#createrequest)
- [cancelRequest(uint256 delegationId)](#cancelrequest)
- [acceptRequest(uint256 delegationId)](#acceptrequest)

### 

```js
function (address newContractsAddress) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address |  | 

### createRequest

creates a Delegation Request

```js
function createRequest(address holder, uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info) external nonpayable
returns(delegationId uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| holder | address |  | 
| validatorId | uint256 | Id of the validator | 
| amount | uint256 | amount of tokens to be used for delegation | 
| delegationPeriod | uint256 | delegation period (3,6,12) | 
| info | string | information about the delegation request
Requirement
-
Delegation period should be allowed
Validator should be registered
Delegator should have enough tokens to delegate, checks the account holder balance through SKALEToken contract | 

### cancelRequest

cancels a Delegation Request

```js
function cancelRequest(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation Request
Requirement
-
Only token holder can cancel request
After cancellation token should be COMPLETED | 

### acceptRequest

validator calls this function to accept a Delegation Request

```js
function acceptRequest(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation Request
Requirement
-
Only token holder can cancel request | 

