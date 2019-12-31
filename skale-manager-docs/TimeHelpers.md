# TimeHelpers.sol

View Source: [contracts/delegation/TimeHelpers.sol](../contracts/delegation/TimeHelpers.sol)

**TimeHelpers**

## Functions

- [getNextMonthStart()](#getnextmonthstart)
- [calculateDelegationEndTime(uint256 requestTime, uint256 delegationPeriod, uint256 redelegationPeriod)](#calculatedelegationendtime)
- [getNextMonthStartFromDate(uint256 dateTimestamp)](#getnextmonthstartfromdate)

### getNextMonthStart

```js
function getNextMonthStart() external view
returns(timestamp uint256)
```

### calculateDelegationEndTime

```js
function calculateDelegationEndTime(uint256 requestTime, uint256 delegationPeriod, uint256 redelegationPeriod) external view
returns(timestamp uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| requestTime | uint256 |  | 
| delegationPeriod | uint256 |  | 
| redelegationPeriod | uint256 |  | 

### getNextMonthStartFromDate

```js
function getNextMonthStartFromDate(uint256 dateTimestamp) public pure
returns(timestamp uint256)
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| dateTimestamp | uint256 |  | 

