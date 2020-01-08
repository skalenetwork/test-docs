# `IHolderDelegation`

 Delegation Request Calls


--- 


## Functions

- [delegate(validatorId, amount, delegationPeriod, info)](#delegate)
- [requestUndelegation(delegationId)](#requestUndelegation)
- [cancelPendingDelegation(delegationId)](#cancelPendingDelegation)
- [getDelegationRequestsForValidator(validatorId)](#getDelegationRequestsForValidator)
- [getValidators()](#getValidators)
- [withdrawBounty(bountyCollectionAddress, amount)](#withdrawBounty)
- [getEarnedBountyAmount()](#getEarnedBountyAmount)

--- 




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

 <p> Creates request to delegate `amount` of tokens to `validatorId` from the beginning of the next month 
Executed by delegator wallet, emits request ID sent event. 
Delegation requests expire after one week
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

 <p> Undelegates a particular delegation, executed by token owner 
Allows tokens holder to request return of it's token from validator 
This will succeed only if delegation period passed
 </p>
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

 <p> Removes delegation request for this delegator wallet
 </p>
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

 <p> Returns an array of pending delegation request IDs for this validator 
Returns 0 if no request exists
 </p>
</div>
</div>

##### `getValidators`

<div class="funcnamegetValidators contract-function">
<h4 id="getValidators">
<code>getValidators()<span class="var-type"> → uint256[] validatorIds</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> get the list of registered validators
 </p>
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

 <p> Withdraws bounty for particular delegation. Bounties will be locked for 3 months
 </p>
</div>
</div>

##### `getEarnedBountyAmount`

<div class="funcnamegetEarnedBountyAmount contract-function">
<h4 id="getEarnedBountyAmount">
<code>getEarnedBountyAmount()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Get earned bounty for delegator
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