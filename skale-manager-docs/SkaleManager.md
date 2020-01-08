# `SkaleManager`



--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [tokensReceived(operator, from, to, value, userData, operatorData)](#tokensReceived)
- [initWithdrawDeposit(nodeIndex)](#initWithdrawDeposit)
- [completeWithdrawdeposit(nodeIndex)](#completeWithdrawdeposit)
- [deleteNode(nodeIndex)](#deleteNode)
- [deleteNodeByRoot(nodeIndex)](#deleteNodeByRoot)
- [deleteSchain(name)](#deleteSchain)
- [deleteSchainByRoot(name)](#deleteSchainByRoot)
- [sendVerdict(fromValidatorIndex, toNodeIndex, downtime, latency)](#sendVerdict)
- [sendVerdicts(fromValidatorIndex, toNodeIndexes, downtimes, latencies)](#sendVerdicts)
- [getBounty(nodeIndex)](#getBounty)
- [manageBounty(from, nodeIndex, downtime, latency, nodesDataAddress)](#manageBounty)
- [fallbackOperationTypeConvert(data)](#fallbackOperationTypeConvert)

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

##### `tokensReceived`

<div class="funcnametokensReceived contract-function">
<h4 id="tokensReceived">
<code>tokensReceived(<span class="var-type">address</span>
operator
, <span class="var-type">address</span>
from
, <span class="var-type">address</span>
to
, <span class="var-type">uint256</span>
value
, <span class="var-type">bytes</span>
userData
, <span class="var-type">bytes</span>
operatorData
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `initWithdrawDeposit`

<div class="funcnameinitWithdrawDeposit contract-function">
<h4 id="initWithdrawDeposit">
<code>initWithdrawDeposit(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `completeWithdrawdeposit`

<div class="funcnamecompleteWithdrawdeposit contract-function">
<h4 id="completeWithdrawdeposit">
<code>completeWithdrawdeposit(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
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

##### `deleteNodeByRoot`

<div class="funcnamedeleteNodeByRoot contract-function">
<h4 id="deleteNodeByRoot">
<code>deleteNodeByRoot(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteSchain`

<div class="funcnamedeleteSchain contract-function">
<h4 id="deleteSchain">
<code>deleteSchain(<span class="var-type">string</span>
name
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteSchainByRoot`

<div class="funcnamedeleteSchainByRoot contract-function">
<h4 id="deleteSchainByRoot">
<code>deleteSchainByRoot(<span class="var-type">string</span>
name
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `sendVerdict`

<div class="funcnamesendVerdict contract-function">
<h4 id="sendVerdict">
<code>sendVerdict(<span class="var-type">uint256</span>
fromValidatorIndex
, <span class="var-type">uint256</span>
toNodeIndex
, <span class="var-type">uint32</span>
downtime
, <span class="var-type">uint32</span>
latency
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `sendVerdicts`

<div class="funcnamesendVerdicts contract-function">
<h4 id="sendVerdicts">
<code>sendVerdicts(<span class="var-type">uint256</span>
fromValidatorIndex
, <span class="var-type">uint256[]</span>
toNodeIndexes
, <span class="var-type">uint32[]</span>
downtimes
, <span class="var-type">uint32[]</span>
latencies
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getBounty`

<div class="funcnamegetBounty contract-function">
<h4 id="getBounty">
<code>getBounty(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `manageBounty`

<div class="funcnamemanageBounty contract-function">
<h4 id="manageBounty">
<code>manageBounty(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">uint32</span>
downtime
, <span class="var-type">uint32</span>
latency
, <span class="var-type">address</span>
nodesDataAddress
)<span class="var-type"> → uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `fallbackOperationTypeConvert`

<div class="funcnamefallbackOperationTypeConvert contract-function">
<h4 id="fallbackOperationTypeConvert">
<code>fallbackOperationTypeConvert(<span class="var-type">bytes</span>
data
)<span class="var-type"> → enum SkaleManager.TransactionOperation</span></code>
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