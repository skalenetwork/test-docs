# IValidatorDelegation.sol

View Source: [contracts/interfaces/delegation/IValidatorDelegation.sol](../contracts/interfaces/delegation/IValidatorDelegation.sol)

**↘ Derived Contracts: [DelegationService](DelegationService.md)**

**IValidatorDelegation**

## Structs
### Validator

```js
struct Validator {
 string name,
 address validatorAddress,
 string description,
 uint256 feeRate,
 uint256 registrationTime,
 uint256 minimumDelegationAmount
}
```

## Functions

- [accept(uint256 delegationId)](#accept)
- [createNode(uint16 port, uint16 nonce, bytes4 ip, bytes4 publicIp)](#createnode)
- [deleteNode(uint256 nodeIndex)](#deletenode)
- [registerValidator(string name, string description, uint256 feeRatePromille, uint256 minimumDelegationAmount)](#registervalidator)
- [unregisterValidator(uint256 validatorId)](#unregistervalidator)
- [getBondAmount(uint256 validatorId)](#getbondamount)
- [setValidatorName(string newName)](#setvalidatorname)
- [setValidatorDescription(string description)](#setvalidatordescription)
- [setValidatorAddress(address newAddress)](#setvalidatoraddress)
- [setMinimumDelegationAmount(uint256 amount)](#setminimumdelegationamount)
- [getValidatorInfo(uint256 validatorId)](#getvalidatorinfo)

### accept

⤿ Overridden Implementation(s): [DelegationService.accept](DelegationService.md#accept)

Allows validator to accept tokens delegated at `delegationId`

```js
function accept(uint256 delegationId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| delegationId | uint256 | returns request | 

### createNode

⤿ Overridden Implementation(s): [DelegationService.createNode](DelegationService.md#createnode)

Adds node to SKALE network

```js
function createNode(uint16 port, uint16 nonce, bytes4 ip, bytes4 publicIp) external nonpayable
```

**Returns**

Returns registered validatorId

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| port | uint16 | Port Validator Node | 
| nonce | uint16 | Node | 
| ip | bytes4 | IP Address of the Validator node | 
| publicIp | bytes4 | Public IP Address of the Validator node | 

### deleteNode

⤿ Overridden Implementation(s): [DelegationService.deleteNode](DelegationService.md#deletenode)

removes node from system

```js
function deleteNode(uint256 nodeIndex) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| nodeIndex | uint256 | index of Node | 

### registerValidator

⤿ Overridden Implementation(s): [DelegationService.registerValidator](DelegationService.md#registervalidator)

Executed by a validator : Registers a new validator <br>
sets validatorAddress to to the address of the caller

```js
function registerValidator(string name, string description, uint256 feeRatePromille, uint256 minimumDelegationAmount) external nonpayable
returns(validatorId uint256)
```

**Returns**

Returns registered validatorId

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| name | string | name of the validator | 
| description | string | Validator Description | 
| feeRatePromille | uint256 | Validator Commission Rate | 
| minimumDelegationAmount | uint256 |  | 

### unregisterValidator

⤿ Overridden Implementation(s): [DelegationService.unregisterValidator](DelegationService.md#unregistervalidator)

Executed by a validator : Unregisters validator. <br>
Returns false if the validator did not exist. Requires zero delegation and bond

```js
function unregisterValidator(uint256 validatorId) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | Id of the registered Validator | 

### getBondAmount

⤿ Overridden Implementation(s): [DelegationService.getBondAmount](DelegationService.md#getbondamount)

return how many of validator funds are locked in SKALEManager

```js
function getBondAmount(uint256 validatorId) external nonpayable
returns(amount uint256)
```

**Returns**

bond amount deposited by this validator

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | Id of the registered Validator | 

### setValidatorName

⤿ Overridden Implementation(s): [DelegationService.setValidatorName](DelegationService.md#setvalidatorname)

sets validator name

```js
function setValidatorName(string newName) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newName | string | new Validator Name | 

### setValidatorDescription

⤿ Overridden Implementation(s): [DelegationService.setValidatorDescription](DelegationService.md#setvalidatordescription)

sets validator address

```js
function setValidatorDescription(string description) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| description | string | Validator Description | 

### setValidatorAddress

⤿ Overridden Implementation(s): [DelegationService.setValidatorAddress](DelegationService.md#setvalidatoraddress)

sets validator address

```js
function setValidatorAddress(address newAddress) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newAddress | address | validator address | 

### setMinimumDelegationAmount

⤿ Overridden Implementation(s): [DelegationService.setMinimumDelegationAmount](DelegationService.md#setminimumdelegationamount)

sets minimum delegation amount

```js
function setMinimumDelegationAmount(uint256 amount) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| amount | uint256 | minimum delegation amount | 

### getValidatorInfo

⤿ Overridden Implementation(s): [DelegationService.getValidatorInfo](DelegationService.md#getvalidatorinfo)

returns the validator info as struct

```js
function getValidatorInfo(uint256 validatorId) external nonpayable
returns(validator struct IValidatorDelegation.Validator)
```

**Returns**

the validator info as struct

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| validatorId | uint256 | Id of the registered Validator | 

