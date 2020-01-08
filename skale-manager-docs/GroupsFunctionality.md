# `GroupsFunctionality`



--- 


## Functions

- [constructor(newExecutorName, newDataName, newContractsAddress)](#constructor)
- [verifySignature(groupIndex, signatureX, signatureY, hashX, hashY)](#verifySignature)
- [addGroup(groupIndex, newRecommendedNumberOfNodes, data)](#addGroup)
- [deleteGroup(groupIndex)](#deleteGroup)
- [upgradeGroup(groupIndex, newRecommendedNumberOfNodes, data)](#upgradeGroup)
- [findNode(groupIndex, nodeIndex)](#findNode)
- [generateGroup(groupIndex)](#generateGroup)
- [selectNodeToGroup(groupIndex)](#selectNodeToGroup)
- [swap(array, index1, index2)](#swap)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">string</span>
newExecutorName
, <span class="var-type">string</span>
newDataName
, <span class="var-type">address</span>
newContractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `verifySignature`

<div class="funcnameverifySignature contract-function">
<h4 id="verifySignature">
<code>verifySignature(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
signatureX
, <span class="var-type">uint256</span>
signatureY
, <span class="var-type">uint256</span>
hashX
, <span class="var-type">uint256</span>
hashY
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addGroup`

<div class="funcnameaddGroup contract-function">
<h4 id="addGroup">
<code>addGroup(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
newRecommendedNumberOfNodes
, <span class="var-type">bytes32</span>
data
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteGroup`

<div class="funcnamedeleteGroup contract-function">
<h4 id="deleteGroup">
<code>deleteGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `upgradeGroup`

<div class="funcnameupgradeGroup contract-function">
<h4 id="upgradeGroup">
<code>upgradeGroup(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
newRecommendedNumberOfNodes
, <span class="var-type">bytes32</span>
data
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `findNode`

<div class="funcnamefindNode contract-function">
<h4 id="findNode">
<code>findNode(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256 index</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `generateGroup`

<div class="funcnamegenerateGroup contract-function">
<h4 id="generateGroup">
<code>generateGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256[]</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `selectNodeToGroup`

<div class="funcnameselectNodeToGroup contract-function">
<h4 id="selectNodeToGroup">
<code>selectNodeToGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → bytes32, uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `swap`

<div class="funcnameswap contract-function">
<h4 id="swap">
<code>swap(<span class="var-type">uint256[]</span>
array
, <span class="var-type">uint256</span>
index1
, <span class="var-type">uint256</span>
index2
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