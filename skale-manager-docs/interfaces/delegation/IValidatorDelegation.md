# `IValidatorDelegation`



--- 


## Functions

- [accept(delegationId)](#accept)
- [createNode(port, nonce, ip, publicIp)](#createNode)
- [deleteNode(nodeIndex)](#deleteNode)
- [registerValidator(name, description, feeRatePromille, minimumDelegationAmount)](#registerValidator)
- [unregisterValidator(validatorId)](#unregisterValidator)
- [getBondAmount(validatorId)](#getBondAmount)
- [setValidatorName(newName)](#setValidatorName)
- [setValidatorDescription(description)](#setValidatorDescription)
- [setValidatorAddress(newAddress)](#setValidatorAddress)
- [setMinimumDelegationAmount(amount)](#setMinimumDelegationAmount)
- [getValidatorInfo(validatorId)](#getValidatorInfo)

--- 




##### `accept`

<div class="funcnameaccept contract-function">
<h4 id="accept">
<code>accept(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Allows validator to accept tokens delegated at `delegationId`
 </p>
</div>
</div>

##### `createNode`

<div class="funcnamecreateNode contract-function">
<h4 id="createNode">
<code>createNode(<span class="var-type">uint16</span>
port
, <span class="var-type">uint16</span>
nonce
, <span class="var-type">bytes4</span>
ip
, <span class="var-type">bytes4</span>
publicIp
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Adds node to SKALE network
 </p>
</div>
</div>

##### `deleteNode`

<div class="funcnamedeleteNode contract-function">
<h4 id="deleteNode">
<code>deleteNode(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> removes node from system
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
feeRatePromille
, <span class="var-type">uint256</span>
minimumDelegationAmount
)<span class="var-type"> → uint256 validatorId</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Executed by a validator : Registers a new validator 
sets validatorAddress to to the address of the caller
 </p>
</div>
</div>

##### `unregisterValidator`

<div class="funcnameunregisterValidator contract-function">
<h4 id="unregisterValidator">
<code>unregisterValidator(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p>  Executed by a validator : Unregisters validator. 
Returns false if the validator did not exist. Requires zero delegation and bond
 </p>
</div>
</div>

##### `getBondAmount`

<div class="funcnamegetBondAmount contract-function">
<h4 id="getBondAmount">
<code>getBondAmount(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"> → uint256 amount</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> return how many of validator funds are locked in SKALEManager
 </p>
</div>
</div>

##### `setValidatorName`

<div class="funcnamesetValidatorName contract-function">
<h4 id="setValidatorName">
<code>setValidatorName(<span class="var-type">string</span>
newName
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> sets validator name
 </p>
</div>
</div>

##### `setValidatorDescription`

<div class="funcnamesetValidatorDescription contract-function">
<h4 id="setValidatorDescription">
<code>setValidatorDescription(<span class="var-type">string</span>
description
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> sets validator address
 </p>
</div>
</div>

##### `setValidatorAddress`

<div class="funcnamesetValidatorAddress contract-function">
<h4 id="setValidatorAddress">
<code>setValidatorAddress(<span class="var-type">address</span>
newAddress
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> sets validator address
 </p>
</div>
</div>

##### `setMinimumDelegationAmount`

<div class="funcnamesetMinimumDelegationAmount contract-function">
<h4 id="setMinimumDelegationAmount">
<code>setMinimumDelegationAmount(<span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> sets minimum delegation amount
 </p>
</div>
</div>

##### `getValidatorInfo`

<div class="funcnamegetValidatorInfo contract-function">
<h4 id="getValidatorInfo">
<code>getValidatorInfo(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"> → struct IValidatorDelegation.Validator validator</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> returns the validator info as struct
 </p>
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