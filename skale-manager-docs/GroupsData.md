# `GroupsData`



--- 


## Functions

- [constructor(newExecutorName, newContractsAddress)](#constructor)
- [addGroup(groupIndex, amountOfNodes, data)](#addGroup)
- [setException(groupIndex, nodeIndex)](#setException)
- [setPublicKey(groupIndex, publicKeyx1, publicKeyy1, publicKeyx2, publicKeyy2)](#setPublicKey)
- [setNodeInGroup(groupIndex, nodeIndex)](#setNodeInGroup)
- [removeNodeFromGroup(indexOfNode, groupIndex)](#removeNodeFromGroup)
- [removeAllNodesInGroup(groupIndex)](#removeAllNodesInGroup)
- [setNodesInGroup(groupIndex, nodesInGroup)](#setNodesInGroup)
- [setGroupFailedDKG(groupIndex)](#setGroupFailedDKG)
- [removeGroup(groupIndex)](#removeGroup)
- [removeExceptionNode(groupIndex, nodeIndex)](#removeExceptionNode)
- [isGroupActive(groupIndex)](#isGroupActive)
- [isExceptionNode(groupIndex, nodeIndex)](#isExceptionNode)
- [getGroupsPublicKey(groupIndex)](#getGroupsPublicKey)
- [getNodesInGroup(groupIndex)](#getNodesInGroup)
- [getGroupData(groupIndex)](#getGroupData)
- [getRecommendedNumberOfNodes(groupIndex)](#getRecommendedNumberOfNodes)
- [getNumberOfNodesInGroup(groupIndex)](#getNumberOfNodesInGroup)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">string</span>
newExecutorName
, <span class="var-type">address</span>
newContractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
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
amountOfNodes
, <span class="var-type">bytes32</span>
data
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setException`

<div class="funcnamesetException contract-function">
<h4 id="setException">
<code>setException(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setPublicKey`

<div class="funcnamesetPublicKey contract-function">
<h4 id="setPublicKey">
<code>setPublicKey(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
publicKeyx1
, <span class="var-type">uint256</span>
publicKeyy1
, <span class="var-type">uint256</span>
publicKeyx2
, <span class="var-type">uint256</span>
publicKeyy2
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setNodeInGroup`

<div class="funcnamesetNodeInGroup contract-function">
<h4 id="setNodeInGroup">
<code>setNodeInGroup(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeNodeFromGroup`

<div class="funcnameremoveNodeFromGroup contract-function">
<h4 id="removeNodeFromGroup">
<code>removeNodeFromGroup(<span class="var-type">uint256</span>
indexOfNode
, <span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeAllNodesInGroup`

<div class="funcnameremoveAllNodesInGroup contract-function">
<h4 id="removeAllNodesInGroup">
<code>removeAllNodesInGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setNodesInGroup`

<div class="funcnamesetNodesInGroup contract-function">
<h4 id="setNodesInGroup">
<code>setNodesInGroup(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256[]</span>
nodesInGroup
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setGroupFailedDKG`

<div class="funcnamesetGroupFailedDKG contract-function">
<h4 id="setGroupFailedDKG">
<code>setGroupFailedDKG(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeGroup`

<div class="funcnameremoveGroup contract-function">
<h4 id="removeGroup">
<code>removeGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeExceptionNode`

<div class="funcnameremoveExceptionNode contract-function">
<h4 id="removeExceptionNode">
<code>removeExceptionNode(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isGroupActive`

<div class="funcnameisGroupActive contract-function">
<h4 id="isGroupActive">
<code>isGroupActive(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isExceptionNode`

<div class="funcnameisExceptionNode contract-function">
<h4 id="isExceptionNode">
<code>isExceptionNode(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getGroupsPublicKey`

<div class="funcnamegetGroupsPublicKey contract-function">
<h4 id="getGroupsPublicKey">
<code>getGroupsPublicKey(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256, uint256, uint256, uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodesInGroup`

<div class="funcnamegetNodesInGroup contract-function">
<h4 id="getNodesInGroup">
<code>getNodesInGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getGroupData`

<div class="funcnamegetGroupData contract-function">
<h4 id="getGroupData">
<code>getGroupData(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → bytes32</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getRecommendedNumberOfNodes`

<div class="funcnamegetRecommendedNumberOfNodes contract-function">
<h4 id="getRecommendedNumberOfNodes">
<code>getRecommendedNumberOfNodes(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfNodesInGroup`

<div class="funcnamegetNumberOfNodesInGroup contract-function">
<h4 id="getNumberOfNodesInGroup">
<code>getNumberOfNodesInGroup(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"> → uint256</span></code>
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