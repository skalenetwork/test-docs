# IHolderDelegation.sol

View Source: [contracts/interfaces/delegation/IHolderDelegation.sol](../contracts/interfaces/delegation/IHolderDelegation.sol)

**↘ Derived Contracts: [DelegationService](DelegationService.md)**

**IHolderDelegation**

Delegation Request Calls

**Events**

```js
event DelegationRequestIsSent(uint256  id);
```

## Functions

- [delegate(uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info)](#delegate)
- [requestUndelegation(uint256 delegationId)](#requestundelegation)
- [cancelPendingDelegation(uint256 delegationId)](#cancelpendingdelegation)
- [getDelegationRequestsForValidator(uint256 validatorId)](#getdelegationrequestsforvalidator)
- [getValidators()](#getvalidators)
- [withdrawBounty(address bountyCollectionAddress, uint256 amount)](#withdrawbounty)
- [getEarnedBountyAmount()](#getearnedbountyamount)

### delegate

⤿ Overridden Implementation(s): [DelegationService.delegate](DelegationService.md#delegate)

Creates request to delegate `amount` of tokens to `validatorId` from the beginning of the next month <br>
Executed by delegator wallet, emits request ID sent event. <br>
Delegation requests expire after one week

```js
function delegate(uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | unique Id of the validator | 
| amount | uint256 | amount of delegation delegator sets up, Value needs to be less than total of the undelegated token value. | 
| delegationPeriod | uint256 | Currently: 3, 6, 12 months | 
| info | string | description | 

### requestUndelegation

⤿ Overridden Implementation(s): [DelegationService.requestUndelegation](DelegationService.md#requestundelegation)

Undelegates a particular delegation, executed by token owner <br>
Allows tokens holder to request return of it's token from validator <br>
This will succeed only if delegation period passed

```js
function requestUndelegation(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation request | 

### cancelPendingDelegation

⤿ Overridden Implementation(s): [DelegationService.cancelPendingDelegation](DelegationService.md#cancelpendingdelegation)

Removes delegation request for this delegator wallet

```js
function cancelPendingDelegation(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | Id of the delegation Request | 

### getDelegationRequestsForValidator

⤿ Overridden Implementation(s): [DelegationService.getDelegationRequestsForValidator](DelegationService.md#getdelegationrequestsforvalidator)

Returns an array of pending delegation request IDs for this validator <br>
Returns 0 if no request exists

```js
function getDelegationRequestsForValidator(uint256 validatorId) external nonpayable
returns(uint256[])
```

**Returns**

an array of pending delegation request IDs for this validator

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | Id of the validator | 

### getValidators

⤿ Overridden Implementation(s): [DelegationService.getValidators](DelegationService.md#getvalidators)

get the list of registered validators

```js
function getValidators() external nonpayable
returns(validatorIds uint256[])
```

**Returns**

list of registered validator Ids

### withdrawBounty

⤿ Overridden Implementation(s): [DelegationService.withdrawBounty](DelegationService.md#withdrawbounty)

Withdraws bounty for particular delegation. Bounties will be locked for 3 months

```js
function withdrawBounty(address bountyCollectionAddress, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| bountyCollectionAddress | address | delegationID | 
| amount | uint256 | amount of bounty request to withdraw | 

### getEarnedBountyAmount

⤿ Overridden Implementation(s): [DelegationService.getEarnedBountyAmount](DelegationService.md#getearnedbountyamount)

Get earned bounty for delegator

```js
function getEarnedBountyAmount() external nonpayable
returns(uint256)
```

**Returns**

Amount of earned bounties

