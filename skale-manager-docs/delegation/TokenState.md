# `TokenState`

 Store and manage tokens states

--- 


## Functions

- [constructor(_contractManager)](#constructor)
- [getLockedCount(holder)](#getLockedCount)
- [getDelegatedCount(holder)](#getDelegatedCount)
- [sold(holder, amount)](#sold)
- [accept(delegationId)](#accept)
- [requestUndelegation(delegationId)](#requestUndelegation)
- [cancel(delegationId)](#cancel)
- [getState(delegationId)](#getState)
- [getPurchasedAmount(holder)](#getPurchasedAmount)
- [setState(delegationId, newState)](#setState)
- [initProposed(delegationId)](#initProposed)
- [isLocked(state)](#isLocked)
- [isDelegated(state)](#isDelegated)
- [proposedToUnlocked(delegationId)](#proposedToUnlocked)
- [acceptedToDelegated(delegationId)](#acceptedToDelegated)
- [purchasedProposedToPurchased(delegationId, delegation)](#purchasedProposedToPurchased)
- [endingDelegatedToUnlocked(delegationId, delegation)](#endingDelegatedToUnlocked)
- [purchasedToUnlocked(holder)](#purchasedToUnlocked)
- [_cancel(delegationId, delegation)](#_cancel)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">address</span>
_contractManager
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `getLockedCount`

<div class="funcnamegetLockedCount contract-function">
<h4 id="getLockedCount">
<code>getLockedCount(<span class="var-type">address</span>
holder
)<span class="var-type"> → uint256 amount</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> get the total locked amount
 </p>
</div>
</div>

##### `getDelegatedCount`

<div class="funcnamegetDelegatedCount contract-function">
<h4 id="getDelegatedCount">
<code>getDelegatedCount(<span class="var-type">address</span>
holder
)<span class="var-type"> → uint256 amount</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> get the total delegated amount
 </p>
</div>
</div>

##### `sold`

<div class="funcnamesold contract-function">
<h4 id="sold">
<code>sold(<span class="var-type">address</span>
holder
, <span class="var-type">uint256</span>
amount
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

##### `cancel`

<div class="funcnamecancel contract-function">
<h4 id="cancel">
<code>cancel(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getState`

<div class="funcnamegetState contract-function">
<h4 id="getState">
<code>getState(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">public</span>
</h4>
<div class="description">

 <p> get the final state of the delegation request
 </p>
</div>
</div>

##### `getPurchasedAmount`

<div class="funcnamegetPurchasedAmount contract-function">
<h4 id="getPurchasedAmount">
<code>getPurchasedAmount(<span class="var-type">address</span>
holder
)<span class="var-type"> → uint256 amount</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `setState`

<div class="funcnamesetState contract-function">
<h4 id="setState">
<code>setState(<span class="var-type">uint256</span>
delegationId
, <span class="var-type">enum TokenState.State</span>
newState
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">

 <p> modifies the token state
 </p>
</div>
</div>

##### `initProposed`

<div class="funcnameinitProposed contract-function">
<h4 id="initProposed">
<code>initProposed(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isLocked`

<div class="funcnameisLocked contract-function">
<h4 id="isLocked">
<code>isLocked(<span class="var-type">enum TokenState.State</span>
state
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isDelegated`

<div class="funcnameisDelegated contract-function">
<h4 id="isDelegated">
<code>isDelegated(<span class="var-type">enum TokenState.State</span>
state
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `proposedToUnlocked`

<div class="funcnameproposedToUnlocked contract-function">
<h4 id="proposedToUnlocked">
<code>proposedToUnlocked(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `acceptedToDelegated`

<div class="funcnameacceptedToDelegated contract-function">
<h4 id="acceptedToDelegated">
<code>acceptedToDelegated(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `purchasedProposedToPurchased`

<div class="funcnamepurchasedProposedToPurchased contract-function">
<h4 id="purchasedProposedToPurchased">
<code>purchasedProposedToPurchased(<span class="var-type">uint256</span>
delegationId
, <span class="var-type">struct DelegationController.Delegation</span>
delegation
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `endingDelegatedToUnlocked`

<div class="funcnameendingDelegatedToUnlocked contract-function">
<h4 id="endingDelegatedToUnlocked">
<code>endingDelegatedToUnlocked(<span class="var-type">uint256</span>
delegationId
, <span class="var-type">struct DelegationController.Delegation</span>
delegation
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `purchasedToUnlocked`

<div class="funcnamepurchasedToUnlocked contract-function">
<h4 id="purchasedToUnlocked">
<code>purchasedToUnlocked(<span class="var-type">address</span>
holder
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `_cancel`

<div class="funcname_cancel contract-function">
<h4 id="_cancel">
<code>_cancel(<span class="var-type">uint256</span>
delegationId
, <span class="var-type">struct DelegationController.Delegation</span>
delegation
)<span class="var-type"> → enum TokenState.State state</span></code>
<span class="item">internal</span>
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