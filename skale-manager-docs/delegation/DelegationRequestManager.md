# `DelegationRequestManager`

 Handles Delegation Requests <br>
Requests are created/canceled by the delegator <br>
Requests are accepted by the validator

--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [createRequest(holder, validatorId, amount, delegationPeriod, info)](#createRequest)
- [cancelRequest(delegationId)](#cancelRequest)
- [acceptRequest(delegationId)](#acceptRequest)

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


</div>
</div>

##### `createRequest`

<div class="funcnamecreateRequest contract-function">
<h4 id="createRequest">
<code>createRequest(<span class="var-type">address</span>
holder
, <span class="var-type">uint256</span>
validatorId
, <span class="var-type">uint256</span>
amount
, <span class="var-type">uint256</span>
delegationPeriod
, <span class="var-type">string</span>
info
)<span class="var-type"> → uint256 delegationId</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> creates a Delegation Request
 </p>
</div>
</div>

##### `cancelRequest`

<div class="funcnamecancelRequest contract-function">
<h4 id="cancelRequest">
<code>cancelRequest(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> cancels a Delegation Request
 </p>
</div>
</div>

##### `acceptRequest`

<div class="funcnameacceptRequest contract-function">
<h4 id="acceptRequest">
<code>acceptRequest(<span class="var-type">uint256</span>
delegationId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> validator calls this function to accept a Delegation Request
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