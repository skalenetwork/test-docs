# `SchainsFunctionalityInternal`



--- 


## Functions

- [constructor(newExecutorName, newDataName, newContractsAddress)](#constructor)
- [createGroupForSchain(schainName, schainId, numberOfNodes, partOfNode)](#createGroupForSchain)
- [getNodesDataFromTypeOfSchain(typeOfSchain)](#getNodesDataFromTypeOfSchain)
- [replaceNode(nodeIndex, groupHash)](#replaceNode)
- [findSchainAtSchainsForNode(nodeIndex, schainId)](#findSchainAtSchainsForNode)
- [removeNodeFromSchain(nodeIndex, groupHash)](#removeNodeFromSchain)
- [selectNodeToGroup(groupIndex)](#selectNodeToGroup)
- [generateGroup(groupIndex)](#generateGroup)
- [removeSpace(nodeIndex, space)](#removeSpace)
- [setNumberOfNodesInGroup(groupIndex, partOfNode, dataAddress)](#setNumberOfNodesInGroup)

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

##### `createGroupForSchain`

<div class="funcnamecreateGroupForSchain contract-function">
<h4 id="createGroupForSchain">
<code>createGroupForSchain(<span class="var-type">string</span>
schainName
, <span class="var-type">bytes32</span>
schainId
, <span class="var-type">uint256</span>
numberOfNodes
, <span class="var-type">uint256</span>
partOfNode
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodesDataFromTypeOfSchain`

<div class="funcnamegetNodesDataFromTypeOfSchain contract-function">
<h4 id="getNodesDataFromTypeOfSchain">
<code>getNodesDataFromTypeOfSchain(<span class="var-type">uint256</span>
typeOfSchain
)<span class="var-type"> → uint256 numberOfNodes, uint256 partOfNode</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `replaceNode`

<div class="funcnamereplaceNode contract-function">
<h4 id="replaceNode">
<code>replaceNode(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes32</span>
groupHash
)<span class="var-type"> → bytes32 schainId, uint256 newNodeIndex</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `findSchainAtSchainsForNode`

<div class="funcnamefindSchainAtSchainsForNode contract-function">
<h4 id="findSchainAtSchainsForNode">
<code>findSchainAtSchainsForNode(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes32</span>
schainId
)<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `removeNodeFromSchain`

<div class="funcnameremoveNodeFromSchain contract-function">
<h4 id="removeNodeFromSchain">
<code>removeNodeFromSchain(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes32</span>
groupHash
)<span class="var-type"></span></code>
<span class="item">public</span>
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

##### `generateGroup`

<div class="funcnamegenerateGroup contract-function">
<h4 id="generateGroup">
<code>generateGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256[] nodesInGroup</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `removeSpace`

<div class="funcnameremoveSpace contract-function">
<h4 id="removeSpace">
<code>removeSpace(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">uint256</span>
space
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `setNumberOfNodesInGroup`

<div class="funcnamesetNumberOfNodesInGroup contract-function">
<h4 id="setNumberOfNodesInGroup">
<code>setNumberOfNodesInGroup(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
partOfNode
, <span class="var-type">address</span>
dataAddress
)<span class="var-type"> → uint256 numberOfNodes, uint256 space</span></code>
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