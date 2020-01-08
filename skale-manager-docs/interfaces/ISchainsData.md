# `ISchainsData`



--- 


## Functions

- [schainsAtSystem(index)](#schainsAtSystem)
- [numberOfSchains()](#numberOfSchains)
- [sumOfSchainsResources()](#sumOfSchainsResources)
- [addSchainForNode(nodeIndex, schainId)](#addSchainForNode)
- [setSchainPartOfNode(schainId, partOfNode)](#setSchainPartOfNode)
- [getLengthOfSchainsForNode(nodeIndex)](#getLengthOfSchainsForNode)
- [schainsForNodes(nodeIndex, indexOfSchain)](#schainsForNodes)
- [getSchainOwner(schainId)](#getSchainOwner)
- [initializeSchain(name, from, lifetime, deposit)](#initializeSchain)
- [setSchainIndex(schainId, from)](#setSchainIndex)
- [removeSchain(schainId, from)](#removeSchain)
- [removeSchainForNode(nodeIndex, schainIndex)](#removeSchainForNode)
- [isTimeExpired(schainId)](#isTimeExpired)
- [isOwnerAddress(from, schainId)](#isOwnerAddress)
- [isSchainNameAvailable(name)](#isSchainNameAvailable)
- [getSchainsPartOfNode(schainId)](#getSchainsPartOfNode)
- [getSchainIdsForNode(nodeIndex)](#getSchainIdsForNode)

--- 




##### `schainsAtSystem`

<div class="funcnameschainsAtSystem contract-function">
<h4 id="schainsAtSystem">
<code>schainsAtSystem(<span class="var-type">uint256</span>
index
)<span class="var-type"> → bytes32</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `numberOfSchains`

<div class="funcnamenumberOfSchains contract-function">
<h4 id="numberOfSchains">
<code>numberOfSchains()<span class="var-type"> → uint64</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `sumOfSchainsResources`

<div class="funcnamesumOfSchainsResources contract-function">
<h4 id="sumOfSchainsResources">
<code>sumOfSchainsResources()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addSchainForNode`

<div class="funcnameaddSchainForNode contract-function">
<h4 id="addSchainForNode">
<code>addSchainForNode(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes32</span>
schainId
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setSchainPartOfNode`

<div class="funcnamesetSchainPartOfNode contract-function">
<h4 id="setSchainPartOfNode">
<code>setSchainPartOfNode(<span class="var-type">bytes32</span>
schainId
, <span class="var-type">uint256</span>
partOfNode
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getLengthOfSchainsForNode`

<div class="funcnamegetLengthOfSchainsForNode contract-function">
<h4 id="getLengthOfSchainsForNode">
<code>getLengthOfSchainsForNode(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `schainsForNodes`

<div class="funcnameschainsForNodes contract-function">
<h4 id="schainsForNodes">
<code>schainsForNodes(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">uint256</span>
indexOfSchain
)<span class="var-type"> → bytes32</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getSchainOwner`

<div class="funcnamegetSchainOwner contract-function">
<h4 id="getSchainOwner">
<code>getSchainOwner(<span class="var-type">bytes32</span>
schainId
)<span class="var-type"> → address</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `initializeSchain`

<div class="funcnameinitializeSchain contract-function">
<h4 id="initializeSchain">
<code>initializeSchain(<span class="var-type">string</span>
name
, <span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
lifetime
, <span class="var-type">uint256</span>
deposit
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setSchainIndex`

<div class="funcnamesetSchainIndex contract-function">
<h4 id="setSchainIndex">
<code>setSchainIndex(<span class="var-type">bytes32</span>
schainId
, <span class="var-type">address</span>
from
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeSchain`

<div class="funcnameremoveSchain contract-function">
<h4 id="removeSchain">
<code>removeSchain(<span class="var-type">bytes32</span>
schainId
, <span class="var-type">address</span>
from
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeSchainForNode`

<div class="funcnameremoveSchainForNode contract-function">
<h4 id="removeSchainForNode">
<code>removeSchainForNode(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">uint256</span>
schainIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isTimeExpired`

<div class="funcnameisTimeExpired contract-function">
<h4 id="isTimeExpired">
<code>isTimeExpired(<span class="var-type">bytes32</span>
schainId
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isOwnerAddress`

<div class="funcnameisOwnerAddress contract-function">
<h4 id="isOwnerAddress">
<code>isOwnerAddress(<span class="var-type">address</span>
from
, <span class="var-type">bytes32</span>
schainId
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isSchainNameAvailable`

<div class="funcnameisSchainNameAvailable contract-function">
<h4 id="isSchainNameAvailable">
<code>isSchainNameAvailable(<span class="var-type">string</span>
name
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getSchainsPartOfNode`

<div class="funcnamegetSchainsPartOfNode contract-function">
<h4 id="getSchainsPartOfNode">
<code>getSchainsPartOfNode(<span class="var-type">bytes32</span>
schainId
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getSchainIdsForNode`

<div class="funcnamegetSchainIdsForNode contract-function">
<h4 id="getSchainIdsForNode">
<code>getSchainIdsForNode(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bytes32[]</span></code>
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