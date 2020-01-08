# `NodesFunctionality`



--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [createNode(from, value, data)](#createNode)
- [removeNode(from, nodeIndex)](#removeNode)
- [removeNodeByRoot(nodeIndex)](#removeNodeByRoot)
- [initWithdrawDeposit(from, nodeIndex)](#initWithdrawDeposit)
- [completeWithdrawDeposit(from, nodeIndex)](#completeWithdrawDeposit)
- [setNodeType(nodesDataAddress, constantsAddress, nodeIndex)](#setNodeType)

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

##### `createNode`

<div class="funcnamecreateNode contract-function">
<h4 id="createNode">
<code>createNode(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
value
, <span class="var-type">bytes</span>
data
)<span class="var-type"> → uint256 nodeIndex</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeNode`

<div class="funcnameremoveNode contract-function">
<h4 id="removeNode">
<code>removeNode(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeNodeByRoot`

<div class="funcnameremoveNodeByRoot contract-function">
<h4 id="removeNodeByRoot">
<code>removeNodeByRoot(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `initWithdrawDeposit`

<div class="funcnameinitWithdrawDeposit contract-function">
<h4 id="initWithdrawDeposit">
<code>initWithdrawDeposit(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `completeWithdrawDeposit`

<div class="funcnamecompleteWithdrawDeposit contract-function">
<h4 id="completeWithdrawDeposit">
<code>completeWithdrawDeposit(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setNodeType`

<div class="funcnamesetNodeType contract-function">
<h4 id="setNodeType">
<code>setNodeType(<span class="var-type">address</span>
nodesDataAddress
, <span class="var-type">address</span>
constantsAddress
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
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