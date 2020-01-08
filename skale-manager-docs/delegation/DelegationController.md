# `DelegationController`

 Delegation Controller for executing delegation events

--- 

## Modifiers
- [checkDelegationExists(delegationId)](#checkDelegationExists)

--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [lock(holder, amount)](#lock)
- [unlock(holder, amount)](#unlock)
- [getLocked(holder)](#getLocked)
- [delegate(delegationId)](#delegate)
- [addDelegation(holder, validatorId, amount, delegationPeriod, created, info)](#addDelegation)
- [unDelegate(validatorId)](#unDelegate)
- [getDelegationsByHolder(holder)](#getDelegationsByHolder)
- [getDelegation(delegationId)](#getDelegation)

--- 



##### `checkDelegationExists`

<div class="funcnamecheckDelegationExists contract-function">
<h4 id="checkDelegationExists"><a class="anchor" href="#checkDelegationExists"></a>
<code>checkDelegationExists(<span class="var-type">uint256</span>
delegationId
) <span class="var-type"></span></code>
<span class="item"></span>
</h4>
<div class="description">


</div>
</div>

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

 <p> DelegationController constructor
 </p>
</div>
</div>

##### `lock`

<div class="funcnamelock contract-function">
<h4 id="lock">
<code>lock(<span class="var-type">address</span>
holder
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
holder
, <span class="var-type">uint256</span>
amount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getLocked`

<div class="funcnamegetLocked contract-function">
<h4 id="getLocked">
<code>getLocked(<span class="var-type">address</span>
holder
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `delegate`

<div class="funcnamedelegate contract-function">
<h4 id="delegate">
<code>delegate(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> with this function validator finalizes the approval of a delegation request
 </p>
</div>
</div>

##### `addDelegation`

<div class="funcnameaddDelegation contract-function">
<h4 id="addDelegation">
<code>addDelegation(<span class="var-type">address</span>
holder
, <span class="var-type">uint256</span>
validatorId
, <span class="var-type">uint256</span>
amount
, <span class="var-type">uint256</span>
delegationPeriod
, <span class="var-type">uint256</span>
created
, <span class="var-type">string</span>
info
)<span class="var-type"> → uint256 delegationId</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `unDelegate`

<div class="funcnameunDelegate contract-function">
<h4 id="unDelegate">
<code>unDelegate(<span class="var-type">uint256</span>
validatorId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> undelegates a delegation from validator
 </p>
</div>
</div>

##### `getDelegationsByHolder`

<div class="funcnamegetDelegationsByHolder contract-function">
<h4 id="getDelegationsByHolder">
<code>getDelegationsByHolder(<span class="var-type">address</span>
holder
)<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getDelegation`

<div class="funcnamegetDelegation contract-function">
<h4 id="getDelegation">
<code>getDelegation(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"> → struct DelegationController.Delegation</span></code>
<span class="item">public</span>
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