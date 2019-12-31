# Permissions - connected module for Upgradeable approach, knows ContractManager (Permissions.sol)

View Source: [contracts/Permissions.sol](../contracts/Permissions.sol)

**↗ Extends: [Ownable](Ownable.md)**
**↘ Derived Contracts: [ConstantsHolder](ConstantsHolder.md), [DelegationController](DelegationController.md), [DelegationPeriodManager](DelegationPeriodManager.md), [DelegationRequestManager](DelegationRequestManager.md), [DelegationService](DelegationService.md), [GroupsData](GroupsData.md), [GroupsFunctionality](GroupsFunctionality.md), [IDecryption](IDecryption.md), [IECDH](IECDH.md), [ISchainsFunctionalityInternal](ISchainsFunctionalityInternal.md), [ISkaleDKG](ISkaleDKG.md), [ISkaleVerifier](ISkaleVerifier.md), [ManagerData](ManagerData.md), [NodesData](NodesData.md), [NodesFunctionality](NodesFunctionality.md), [Pricing](Pricing.md), [SchainsFunctionality](SchainsFunctionality.md), [SkaleBalances](SkaleBalances.md), [SkaleDKG](SkaleDKG.md), [SkaleManager](SkaleManager.md), [SkaleToken](SkaleToken.md), [SkaleVerifier](SkaleVerifier.md), [TokenSaleManager](TokenSaleManager.md), [TokenState](TokenState.md), [ValidatorService](ValidatorService.md)**

**Permissions**

## Contract Members
**Constants & Variables**

```js
contract ContractManager internal contractManager;

```

## Modifiers

- [allow](#allow)
- [allowMultiple](#allowmultiple)

### allow

allow - throws if called by any account and contract other than the owner
or `contractName` contract

```js
modifier allow(string contractName) internal
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| contractName | string | - human readable name of contract | 

### allowMultiple

```js
modifier allowMultiple(string contractNameFirst, string contractNameSecond) internal
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| contractNameFirst | string |  | 
| contractNameSecond | string |  | 

## Functions

- [(address newContractsAddress)](#)

### 

constructor - sets current address of ContractManager

```js
function (address newContractsAddress) public nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| newContractsAddress | address | - current address of ContractManager | 

