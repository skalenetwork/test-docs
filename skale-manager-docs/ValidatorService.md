# `ValidatorService`



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








### `constructor`

<div class="funcnameconstructor contract-item">
<h4 id="hfuncnameconstructor"><a class="anchor" href="#funcnameconstructor"></a>
<code>constructor(address newContractsAddress) <span class="var-type"></span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">

 <p> Constructor of a validator service registers newContract Address
 </p>
</div>

</div>

### `registerValidator`

<div class="funcnameregisterValidator contract-item">
<h4 id="hfuncnameregisterValidator"><a class="anchor" href="#funcnameregisterValidator"></a>
<code>registerValidator(string name, string description, uint256 feeRate, uint256 minimumDelegationAmount) <span class="var-type"> → uint256 validatorId</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">

 <p> Executed by a DelegationService.registerValidator : and registers a validator info sets validatorAddress to to the address of the caller
 </p>
</div>

</div>

### `setNewValidatorAddress`

<div class="funcnamesetNewValidatorAddress contract-item">
<h4 id="hfuncnamesetNewValidatorAddress"><a class="anchor" href="#funcnamesetNewValidatorAddress"></a>
<code>setNewValidatorAddress(address newValidatorAddress, uint256 validatorId) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">

 <p> sets new address to validator
 </p>
</div>

</div>

### `checkValidatorExists`

<div class="funcnamecheckValidatorExists contract-item">
<h4 id="hfuncnamecheckValidatorExists"><a class="anchor" href="#funcnamecheckValidatorExists"></a>
<code>checkValidatorExists(uint256 validatorId) <span class="var-type"> → bool</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


</div>

</div>

### `checkMinimumDelegation`

<div class="funcnamecheckMinimumDelegation contract-item">
<h4 id="hfuncnamecheckMinimumDelegation"><a class="anchor" href="#funcnamecheckMinimumDelegation"></a>
<code>checkMinimumDelegation(uint256 validatorId, uint256 amount) <span class="var-type"> → bool</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


</div>

</div>

### `checkValidatorAddressToId`

<div class="funcnamecheckValidatorAddressToId contract-item">
<h4 id="hfuncnamecheckValidatorAddressToId"><a class="anchor" href="#funcnamecheckValidatorAddressToId"></a>
<code>checkValidatorAddressToId(address validatorAddress, uint256 validatorId) <span class="var-type"> → bool</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">

 <p> this function is used by DelegationRequestManager.checkValidatorAccess to check if a validatorId is matching the validatorAddress
 </p>
</div>

</div>

### `createNode`

<div class="funcnamecreateNode contract-item">
<h4 id="hfuncnamecreateNode"><a class="anchor" href="#funcnamecreateNode"></a>
<code>createNode() <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


</div>

</div>

<style>
    .contract-item {
        border-radius: var(--border-radius);
        border: solid 1px #ddd;
        max-width: 90vw;
        padding: 0;
        margin-top: 1em;
        margin-bottom: 1em;
        word-wrap: break-word;
    }

    .contract-item h4 {
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

    .contract-item h4::before {
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
    .contract-item h4 code {
        color: inherit;
        background-color: transparent;
        padding: 5px
    }

    .contract-item h4 .item-kind {
        font-weight: 300;
        opacity: .8;
    }

    .contract-item .description{
        padding: 5px
    }

    .contract-item .box {
        margin: 20px 10px;
        padding: 10px 30px;
        background-color: #EEE;
        border: 1px solid #CCC;
    }
</style>


