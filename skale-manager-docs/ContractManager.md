# Main contract in upgradeable approach. This contract contain actual
contracts for this moment in skale manager system by human name. (ContractManager.sol)

View Source: [contracts/ContractManager.sol](../contracts/ContractManager.sol)

**↗ Extends: [Ownable](Ownable.md)**

**ContractManager**

## Contract Members
**Constants & Variables**

```js
mapping(bytes32 => address) public contracts;

```

**Events**

```js
event ContractUpgraded(string  contractsName, address  contractsAddress);
```

## Functions

- [setContractsAddress(string contractsName, address newContractsAddress)](#setcontractsaddress)
- [getContract(string name)](#getcontract)

### setContractsAddress

```js
function setContractsAddress(string contractsName, address newContractsAddress) external nonpayable onlyOwner 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| contractsName | string | - contracts name in skale manager system | 
| newContractsAddress | address | - contracts address in skale manager system | 

### getContract

```js
function getContract(string name) external view
returns(contractAddress address)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| name | string |  | 

