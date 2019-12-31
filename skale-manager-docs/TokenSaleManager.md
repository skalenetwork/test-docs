# TokenSaleManager.sol

View Source: [contracts/delegation/TokenSaleManager.sol](../contracts/delegation/TokenSaleManager.sol)

**↗ Extends: [ITokenSaleManager](ITokenSaleManager.md), [Permissions](Permissions.md), [IERC777Recipient](IERC777Recipient.md)**

**TokenSaleManager**

: Implements ITokenSaleManager interface <br>
Token Sale Manager will initially hold all tokens for the sale and allow users to retrieve them.
Implements the function from IERC777Recipient.tokensReceived <br>

## Contract Members
**Constants & Variables**

```js
//private members
contract IERC1820Registry private _erc1820;

//internal members
address internal seller;
mapping(address => uint256) internal approved;
uint256 internal totalApproved;

```

## Functions

- [(address _contractManager)](#)
- [approve(address[] walletAddress, uint256[] value)](#approve)
- [retrieve()](#retrieve)
- [registerSeller(address _seller)](#registerseller)
- [tokensReceived(address operator, address from, address to, uint256 amount, bytes userData, bytes operatorData)](#tokensreceived)
- [getBalance()](#getbalance)

### 

Token Sale Manager Constructor

```js
function (address _contractManager) public nonpayable Permissions 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| _contractManager | address | Contract Manager address | 

### approve

⤾ overrides [ITokenSaleManager.approve](ITokenSaleManager.md#approve)

Implementation of the ITokenSaleManager.approve function <br>
Allocates values for `walletAddresses` <br>
At the end of the sale token approval function will be called (can be called multiple times) <br>

```js
function approve(address[] walletAddress, uint256[] value) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| walletAddress | address[] | array of addresses that the tokens will be sent | 
| value | uint256[] | array of the values of the tokens that will be sent to each address
Requirement
-
Seller should be authorized to distribute tokens to addresses
WalletAddress length should be equal to value
Balance of the seller should be more than the total approved amount | 

### retrieve

⤾ overrides [ITokenSaleManager.retrieve](ITokenSaleManager.md#retrieve)

Implementation of the ITokenSaleManager.retrieve function <br>
Transfers the entire value to sender address. Tokens are locked. <br>
Each sale participant calls retrieve() - the entire value is transferred to walletAddress<br>
After the transfer, the token in walletAddress will be locked through DelegationService contract<br>
User will be able to see the token in the wallet.

```js
function retrieve() external nonpayable
```

### registerSeller

⤾ overrides [ITokenSaleManager.registerSeller](ITokenSaleManager.md#registerseller)

Implementation of the ITokenSaleManager.registerSeller function <br>
Allows seller address to approve tokens transfers

```js
function registerSeller(address _seller) external nonpayable onlyOwner 
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| _seller | address | seller address of the wallet | 

### tokensReceived

⤾ overrides [IERC777Recipient.tokensReceived](IERC777Recipient.md#tokensreceived)

Not implemented!
Called by an {IERC777} token contract whenever tokens are being
moved or created into a registered account (`to`). The type of operation
is conveyed by `from` being the zero address or not.
     * This call occurs _after_ the token contract's state is updated, so
{IERC777-balanceOf}, etc., can be used to query the post-operation state.
     * This function may revert to prevent the operation from being executed.

```js
function tokensReceived(address operator, address from, address to, uint256 amount, bytes userData, bytes operatorData) external nonpayable
```

**Arguments**

| Name        | Type           | Description  |
| ------------- |------------- | -----|
| operator | address |  | 
| from | address |  | 
| to | address |  | 
| amount | uint256 |  | 
| userData | bytes |  | 
| operatorData | bytes |  | 

### getBalance

internal function to get balance from ERC-20 contract through contract manager <br>
This will be used to check if an address have enough balance

```js
function getBalance() internal nonpayable
returns(balance uint256)
```

**Returns**

the balance of the current address

