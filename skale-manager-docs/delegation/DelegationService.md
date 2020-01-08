# `DelegationService`

 Implements IHolderDelegation and IValidatorDelegation interfaces

--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [requestUndelegation(delegationId)](#requestUndelegation)
- [accept(delegationId)](#accept)
- [createNode(port, nonce, ip, publicIp)](#createNode)
- [setMinimumDelegationAmount(amount)](#setMinimumDelegationAmount)
- [returnTokens(amount)](#returnTokens)
- [listDelegationRequests()](#listDelegationRequests)
- [slash(validator, amount)](#slash)
- [pay(validator, amount)](#pay)
- [getDelegatedAmount(validator)](#getDelegatedAmount)
- [setMinimumStakingRequirement(amount)](#setMinimumStakingRequirement)
- [delegate(validatorId, amount, delegationPeriod, info)](#delegate)
- [cancelPendingDelegation(delegationId)](#cancelPendingDelegation)
- [getAllDelegationRequests()](#getAllDelegationRequests)
- [getDelegationRequestsForValidator(validatorId)](#getDelegationRequestsForValidator)
- [registerValidator(name, description, feeRate, minimumDelegationAmount)](#registerValidator)
- [unregisterValidator(validatorId)](#unregisterValidator)
- [getBondAmount(validatorId)](#getBondAmount)
- [setValidatorName(newName)](#setValidatorName)
- [setValidatorDescription(description)](#setValidatorDescription)
- [setValidatorAddress(newAddress)](#setValidatorAddress)
- [getValidatorInfo(validatorId)](#getValidatorInfo)
- [getValidators()](#getValidators)
- [withdrawBounty(bountyCollectionAddress, amount)](#withdrawBounty)
- [getEarnedBountyAmount()](#getEarnedBountyAmount)
- [deleteNode(nodeIndex)](#deleteNode)
- [lock(wallet, amount)](#lock)
- [unlock(target)](#unlock)
- [getLockedOf(wallet)](#getLockedOf)
- [getDelegatedOf(wallet)](#getDelegatedOf)

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

 <p> constructor of DelegationService
 </p>
</div>
</div>

##### `requestUndelegation`

<div class="funcnamerequestUndelegation contract-function">
<h4 id="requestUndelegation">
<code>requestUndelegation(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `accept`

<div class="funcnameaccept contract-function">
<h4 id="accept">
<code>accept(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


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


</div>
</div>

##### `returnTokens`

<div class="funcnamereturnTokens contract-function">
<h4 id="returnTokens">
<code>returnTokens(<span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Requests return of tokens that are locked in SkaleManager </p>
</div>
</div>

##### `listDelegationRequests`

<div class="funcnamelistDelegationRequests contract-function">
<h4 id="listDelegationRequests">
<code>listDelegationRequests()<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Returns array of delegation requests id </p>
</div>
</div>

##### `slash`

<div class="funcnameslash contract-function">
<h4 id="slash">
<code>slash(<span class="var-type">address</span>
validator
, <span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Allows service to slash `validator` by `amount` of tokens </p>
</div>
</div>

##### `pay`

<div class="funcnamepay contract-function">
<h4 id="pay">
<code>pay(<span class="var-type">address</span>
validator
, <span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Allows service to pay `amount` of tokens to `validator` </p>
</div>
</div>

##### `getDelegatedAmount`

<div class="funcnamegetDelegatedAmount contract-function">
<h4 id="getDelegatedAmount">
<code>getDelegatedAmount(<span class="var-type">address</span>
validator
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Returns amount of delegated token of the validator
 </p>
</div>
</div>

##### `setMinimumStakingRequirement`

<div class="funcnamesetMinimumStakingRequirement contract-function">
<h4 id="setMinimumStakingRequirement">
<code>setMinimumStakingRequirement(<span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Minimum Staking Requirement, set by the validator
 </p>
</div>
</div>

##### `delegate`

<div class="funcnamedelegate contract-function">
<h4 id="delegate">
<code>delegate(<span class="var-type">uint256</span>
validatorId
, <span class="var-type">uint256</span>
amount
, <span class="var-type">uint256</span>
delegationPeriod
, <span class="var-type">string</span>
info
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `cancelPendingDelegation`

<div class="funcnamecancelPendingDelegation contract-function">
<h4 id="cancelPendingDelegation">
<code>cancelPendingDelegation(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getAllDelegationRequests`

<div class="funcnamegetAllDelegationRequests contract-function">
<h4 id="getAllDelegationRequests">
<code>getAllDelegationRequests()<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getDelegationRequestsForValidator`

<div class="funcnamegetDelegationRequestsForValidator contract-function">
<h4 id="getDelegationRequestsForValidator">
<code>getDelegationRequestsForValidator(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


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


</div>
</div>

##### `getValidators`

<div class="funcnamegetValidators contract-function">
<h4 id="getValidators">
<code>getValidators()<span class="var-type"> → uint256[] validatorIds</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `withdrawBounty`

<div class="funcnamewithdrawBounty contract-function">
<h4 id="withdrawBounty">
<code>withdrawBounty(<span class="var-type">address</span>
bountyCollectionAddress
, <span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getEarnedBountyAmount`

<div class="funcnamegetEarnedBountyAmount contract-function">
<h4 id="getEarnedBountyAmount">
<code>getEarnedBountyAmount()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


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


</div>
</div>

##### `lock`

<div class="funcnamelock contract-function">
<h4 id="lock">
<code>lock(<span class="var-type">address</span>
wallet
, <span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `unlock`

<div class="funcnameunlock contract-function">
<h4 id="unlock">
<code>unlock(<span class="var-type">address</span>
target
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getLockedOf`

<div class="funcnamegetLockedOf contract-function">
<h4 id="getLockedOf">
<code>getLockedOf(<span class="var-type">address</span>
wallet
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getDelegatedOf`

<div class="funcnamegetDelegatedOf contract-function">
<h4 id="getDelegatedOf">
<code>getDelegatedOf(<span class="var-type">address</span>
wallet
)<span class="var-type"> → bool</span></code>
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