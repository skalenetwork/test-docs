# Delegation Service Contract (DelegationService.sol)

View Source: [contracts/delegation/DelegationService.sol](../contracts/delegation/DelegationService.sol)

**↗ Extends: [Permissions](Permissions.md), [IHolderDelegation](IHolderDelegation.md), [IValidatorDelegation](IValidatorDelegation.md)**

**DelegationService**

Implements IHolderDelegation and IValidatorDelegation interfaces

**Events**

```js
event DelegationRequestIsSent(uint256  delegationId);
event ValidatorRegistered(uint256  validatorId);
```

## Functions

- [(address newContractsAddress)](#)
- [requestUndelegation(uint256 delegationId)](#requestundelegation)
- [accept(uint256 delegationId)](#accept)
- [createNode(uint16 port, uint16 nonce, bytes4 ip, bytes4 publicIp)](#createnode)
- [setMinimumDelegationAmount(uint256 amount)](#setminimumdelegationamount)
- [returnTokens(uint256 amount)](#returntokens)
- [listDelegationRequests()](#listdelegationrequests)
- [slash(address validator, uint256 amount)](#slash)
- [pay(address validator, uint256 amount)](#pay)
- [getDelegatedAmount(address validator)](#getdelegatedamount)
- [setMinimumStakingRequirement(uint256 amount)](#setminimumstakingrequirement)
- [delegate(uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info)](#delegate)
- [cancelPendingDelegation(uint256 delegationId)](#cancelpendingdelegation)
- [getAllDelegationRequests()](#getalldelegationrequests)
- [getDelegationRequestsForValidator(uint256 validatorId)](#getdelegationrequestsforvalidator)
- [registerValidator(string name, string description, uint256 feeRate, uint256 minimumDelegationAmount)](#registervalidator)
- [unregisterValidator(uint256 validatorId)](#unregistervalidator)
- [getBondAmount(uint256 validatorId)](#getbondamount)
- [setValidatorName(string newName)](#setvalidatorname)
- [setValidatorDescription(string description)](#setvalidatordescription)
- [setValidatorAddress(address newAddress)](#setvalidatoraddress)
- [getValidatorInfo(uint256 validatorId)](#getvalidatorinfo)
- [getValidators()](#getvalidators)
- [withdrawBounty(address bountyCollectionAddress, uint256 amount)](#withdrawbounty)
- [getEarnedBountyAmount()](#getearnedbountyamount)
- [deleteNode(uint256 nodeIndex)](#deletenode)
- [lock(address wallet, uint256 amount)](#lock)
- [unlock(address target)](#unlock)
- [getLockedOf(address wallet)](#getlockedof)
- [getDelegatedOf(address wallet)](#getdelegatedof)

### 

constructor of DelegationService

```js
function (address newContractsAddress) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address | to register for Permissions | 

### requestUndelegation

⤾ overrides [IHolderDelegation.requestUndelegation](IHolderDelegation.md#requestundelegation)

```js
function requestUndelegation(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### accept

⤾ overrides [IValidatorDelegation.accept](IValidatorDelegation.md#accept)

See {IValidatorDelegation.accept}
calls DelegationRequestManager.acceptRequest

```js
function accept(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### createNode

⤾ overrides [IValidatorDelegation.createNode](IValidatorDelegation.md#createnode)

See {IValidatorDelegation-createNode}. Not Implemented!

```js
function createNode(uint16 port, uint16 nonce, bytes4 ip, bytes4 publicIp) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| port | uint16 |  | 
| nonce | uint16 |  | 
| ip | bytes4 |  | 
| publicIp | bytes4 |  | 

### setMinimumDelegationAmount

⤾ overrides [IValidatorDelegation.setMinimumDelegationAmount](IValidatorDelegation.md#setminimumdelegationamount)

See {IValidatorDelegation-minimumDelegationAmount}. Not Implemented!

```js
function setMinimumDelegationAmount(uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| amount | uint256 |  | 

### returnTokens

Requests return of tokens that are locked in SkaleManager

```js
function returnTokens(uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| amount | uint256 |  | 

### listDelegationRequests

Returns array of delegation requests id

```js
function listDelegationRequests() external nonpayable
returns(uint256[])
```

### slash

Allows service to slash `validator` by `amount` of tokens

```js
function slash(address validator, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validator | address |  | 
| amount | uint256 |  | 

### pay

Allows service to pay `amount` of tokens to `validator`

```js
function pay(address validator, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validator | address |  | 
| amount | uint256 |  | 

### getDelegatedAmount

Returns amount of delegated token of the validator

```js
function getDelegatedAmount(address validator) external nonpayable
returns(uint256)
```

**Returns**

amount of Delegated Tokens

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validator | address | address of the validator | 

### setMinimumStakingRequirement

Minimum Staking Requirement, set by the validator

```js
function setMinimumStakingRequirement(uint256 amount) external nonpayable
```

**Returns**

Amount of Delegated Tokens

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| amount | uint256 | minimum staking amount | 

### delegate

⤾ overrides [IHolderDelegation.delegate](IHolderDelegation.md#delegate)

See {IHolderDelegation.delegate}

```js
function delegate(uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 |  | 
| amount | uint256 |  | 
| delegationPeriod | uint256 |  | 
| info | string |  | 

### cancelPendingDelegation

⤾ overrides [IHolderDelegation.cancelPendingDelegation](IHolderDelegation.md#cancelpendingdelegation)

See {IHolderDelegation.cancelPendingDelegation}

```js
function cancelPendingDelegation(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 |  | 

### getAllDelegationRequests

See {IHolderDelegation.getAllDelegationRequests}. "Not implemented"

```js
function getAllDelegationRequests() external nonpayable
returns(uint256[])
```

### getDelegationRequestsForValidator

⤾ overrides [IHolderDelegation.getDelegationRequestsForValidator](IHolderDelegation.md#getdelegationrequestsforvalidator)

See {IHolderDelegation.getDelegationRequestsForValidator}. "Not implemented"

```js
function getDelegationRequestsForValidator(uint256 validatorId) external nonpayable
returns(uint256[])
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 |  | 

### registerValidator

⤾ overrides [IValidatorDelegation.registerValidator](IValidatorDelegation.md#registervalidator)

See {IValidatorDelegation.registerValidator}.

```js
function registerValidator(string name, string description, uint256 feeRate, uint256 minimumDelegationAmount) external nonpayable
returns(validatorId uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| name | string |  | 
| description | string |  | 
| feeRate | uint256 |  | 
| minimumDelegationAmount | uint256 |  | 

### unregisterValidator

⤾ overrides [IValidatorDelegation.unregisterValidator](IValidatorDelegation.md#unregistervalidator)

See {IValidatorDelegation.unregisterValidator}. "Not implemented"

```js
function unregisterValidator(uint256 validatorId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 |  | 

### getBondAmount

⤾ overrides [IValidatorDelegation.getBondAmount](IValidatorDelegation.md#getbondamount)

See {IValidatorDelegation.getBondAmount}. "Not implemented"

```js
function getBondAmount(uint256 validatorId) external nonpayable
returns(amount uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 |  | 

### setValidatorName

⤾ overrides [IValidatorDelegation.setValidatorName](IValidatorDelegation.md#setvalidatorname)

See {IValidatorDelegation.setValidatorName}. "Not implemented"

```js
function setValidatorName(string newName) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newName | string |  | 

### setValidatorDescription

⤾ overrides [IValidatorDelegation.setValidatorDescription](IValidatorDelegation.md#setvalidatordescription)

See {IValidatorDelegation.setValidatorDescription}. "Not implemented"

```js
function setValidatorDescription(string description) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| description | string |  | 

### setValidatorAddress

⤾ overrides [IValidatorDelegation.setValidatorAddress](IValidatorDelegation.md#setvalidatoraddress)

See {IValidatorDelegation.setValidatorAddress}. "Not implemented"

```js
function setValidatorAddress(address newAddress) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newAddress | address |  | 

### getValidatorInfo

⤾ overrides [IValidatorDelegation.getValidatorInfo](IValidatorDelegation.md#getvalidatorinfo)

See {IValidatorDelegation.getValidatorInfo}. "Not implemented"

```js
function getValidatorInfo(uint256 validatorId) external nonpayable
returns(validator struct IValidatorDelegation.Validator)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 |  | 

### getValidators

⤾ overrides [IHolderDelegation.getValidators](IHolderDelegation.md#getvalidators)

See {IHolderDelegation.getValidators}. "Not implemented"

```js
function getValidators() external nonpayable
returns(validatorIds uint256[])
```

### withdrawBounty

⤾ overrides [IHolderDelegation.withdrawBounty](IHolderDelegation.md#withdrawbounty)

See {IHolderDelegation.withdrawBounty}. "Not implemented"

```js
function withdrawBounty(address bountyCollectionAddress, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| bountyCollectionAddress | address |  | 
| amount | uint256 |  | 

### getEarnedBountyAmount

⤾ overrides [IHolderDelegation.getEarnedBountyAmount](IHolderDelegation.md#getearnedbountyamount)

See {IHolderDelegation.getEarnedBountyAmount}. "Not implemented"

```js
function getEarnedBountyAmount() external nonpayable
returns(uint256)
```

### deleteNode

⤾ overrides [IValidatorDelegation.deleteNode](IValidatorDelegation.md#deletenode)

See {IValidatorDelegation.deleteNode}. "Not implemented"

```js
function deleteNode(uint256 nodeIndex) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| nodeIndex | uint256 |  | 

### lock

```js
function lock(address wallet, uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address |  | 
| amount | uint256 |  | 

### unlock

```js
function unlock(address target) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| target | address |  | 

### getLockedOf

```js
function getLockedOf(address wallet) external nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address |  | 

### getDelegatedOf

```js
function getDelegatedOf(address wallet) external nonpayable
returns(bool)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| wallet | address |  | 

