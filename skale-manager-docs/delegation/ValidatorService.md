# `ValidatorService`

 Validator Service handles all validator related information and registration

--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [registerValidator(name, description, feeRate, minimumDelegationAmount)](#registerValidator)
- [setNewValidatorAddress(newValidatorAddress, validatorId)](#setNewValidatorAddress)
- [checkValidatorExists(validatorId)](#checkValidatorExists)
- [checkMinimumDelegation(validatorId, amount)](#checkMinimumDelegation)
- [checkValidatorAddressToId(validatorAddress, validatorId)](#checkValidatorAddressToId)
- [createNode()](#createNode)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">address</span>
newContractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">

 <p> Constructor of a validator service registers newContract Address
 </p>
</div>
</div>

##### `registerValidator`

<div class="funcnameregisterValidator contract-function">
<h4 id="registerValidator">
<code>registerValidator(<span class="var-type">string</span>
name
, <span class="var-type">string</span>
description
, <span class="var-type">uint256</span>
feeRate
, <span class="var-type">uint256</span>
minimumDelegationAmount
)<span class="var-type"> → uint256 validatorId</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Executed by a DelegationService.registerValidator : and registers a validator info 
sets validatorAddress to to the address of the caller
 </p>
</div>
</div>

##### `setNewValidatorAddress`

<div class="funcnamesetNewValidatorAddress contract-function">
<h4 id="setNewValidatorAddress">
<code>setNewValidatorAddress(<span class="var-type">address</span>
newValidatorAddress
, <span class="var-type">uint256</span>
validatorId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> sets new address to validator
 </p>
</div>
</div>

##### `checkValidatorExists`

<div class="funcnamecheckValidatorExists contract-function">
<h4 id="checkValidatorExists">
<code>checkValidatorExists(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `checkMinimumDelegation`

<div class="funcnamecheckMinimumDelegation contract-function">
<h4 id="checkMinimumDelegation">
<code>checkMinimumDelegation(<span class="var-type">uint256</span>
validatorId
, <span class="var-type">uint256</span>
amount
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `checkValidatorAddressToId`

<div class="funcnamecheckValidatorAddressToId contract-function">
<h4 id="checkValidatorAddressToId">
<code>checkValidatorAddressToId(<span class="var-type">address</span>
validatorAddress
, <span class="var-type">uint256</span>
validatorId
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> this function is used by DelegationRequestManager.checkValidatorAccess 
to check if a validatorId is matching the validatorAddress
 </p>
</div>
</div>

##### `createNode`

<div class="funcnamecreateNode contract-function">
<h4 id="createNode">
<code>createNode()<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

--- 


<style>
    .contract-function {
        border-radius: var(--border-radius);
        border: solid 1px #ddd;
        max-width: 90vw;
        padding: 0;
        margin-top: 1em;
        margin-bottom: 1em;
        word-wrap: break-word;
    }

    .contract-function h4 {
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-orient: horizontal;
        -webkit-box-direction: normal;
        -ms-flex-direction: row;
        flex-direction: row;
        -webkit-box-pack: justify;
        -ms-flex-pack: justify;
        justify-content: space-between;
        -ms-flex-line-pack: start;
        align-content: flex-start;
        padding: 0;
        margin: 1em;
        margin-bottom: 2em;
        position: relative;
        font-size: inherit;
    }

    .contract-function h4::before {
        content: "";
        display: block;
        position: absolute;
        height: 100%;
        width: 100%;
        -webkit-box-sizing: content-box;
        box-sizing: content-box;
        padding: 1em;
        margin: -1em;
        z-index: -10;
        background-color: #f9f9fa;
        border-bottom: solid 1px #ddd;
    }
    .anchor {
        display: inline-block;
        height: 1em;
        margin-left: -25px;
        opacity: 0;
        position: absolute;
        transition: opacity var(--transition-speed-sm) var(--transition-timing);
    }

    .contract-function h4 code {
        color: inherit;
        background-color: transparent;
        padding: 5px
    }

    .contract-function h4 .item {
        font-weight: 300;
        opacity: .8;
    }

    .contract-function .description{
        margin-left: 20px;
        padding: 5px
    }

    .contract-function .var-type {
         font-weight: 300;
    }
</style>