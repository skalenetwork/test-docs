# `SchainsFunctionality`



--- 


## Functions

- [constructor(newExecutorName, newDataName, newContractsAddress)](#constructor)
- [addSchain(from, deposit, data)](#addSchain)
- [deleteSchain(from, name)](#deleteSchain)
- [deleteSchainByRoot(name)](#deleteSchainByRoot)
- [rotateNode(nodeIndex, schainId)](#rotateNode)
- [getSchainPrice(typeOfSchain, lifetime)](#getSchainPrice)
- [initializeSchainInSchainsData(name, from, deposit, lifetime)](#initializeSchainInSchainsData)
- [fallbackSchainParametersDataConverter(data)](#fallbackSchainParametersDataConverter)
- [addSpace(nodeIndex, partOfNode)](#addSpace)

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

##### `addSchain`

<div class="funcnameaddSchain contract-function">
<h4 id="addSchain">
<code>addSchain(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
deposit
, <span class="var-type">bytes</span>
data
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteSchain`

<div class="funcnamedeleteSchain contract-function">
<h4 id="deleteSchain">
<code>deleteSchain(<span class="var-type">address</span>
from
, <span class="var-type">string</span>
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

##### `rotateNode`

<div class="funcnamerotateNode contract-function">
<h4 id="rotateNode">
<code>rotateNode(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes32</span>
schainId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getSchainPrice`

<div class="funcnamegetSchainPrice contract-function">
<h4 id="getSchainPrice">
<code>getSchainPrice(<span class="var-type">uint256</span>
typeOfSchain
, <span class="var-type">uint256</span>
lifetime
)<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `initializeSchainInSchainsData`

<div class="funcnameinitializeSchainInSchainsData contract-function">
<h4 id="initializeSchainInSchainsData">
<code>initializeSchainInSchainsData(<span class="var-type">string</span>
name
, <span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
deposit
, <span class="var-type">uint256</span>
lifetime
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `fallbackSchainParametersDataConverter`

<div class="funcnamefallbackSchainParametersDataConverter contract-function">
<h4 id="fallbackSchainParametersDataConverter">
<code>fallbackSchainParametersDataConverter(<span class="var-type">bytes</span>
data
)<span class="var-type"> → struct SchainsFunctionality.SchainParameters schainParameters</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `addSpace`

<div class="funcnameaddSpace contract-function">
<h4 id="addSpace">
<code>addSpace(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">uint256</span>
partOfNode
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