# `NodesData`



--- 


## Functions

- [constructor(newLeavingPeriod, newContractsAddress)](#constructor)
- [getNodesWithFreeSpace(partOfNode, freeSpace)](#getNodesWithFreeSpace)
- [addNode(from, name, ip, publicIP, port, publicKey)](#addNode)
- [addFractionalNode(nodeIndex)](#addFractionalNode)
- [addFullNode(nodeIndex)](#addFullNode)
- [setNodeLeaving(nodeIndex)](#setNodeLeaving)
- [setNodeLeft(nodeIndex)](#setNodeLeft)
- [removeFractionalNode(subarrayIndex)](#removeFractionalNode)
- [removeFullNode(subarrayIndex)](#removeFullNode)
- [removeSpaceFromFractionalNode(subarrayLink, space)](#removeSpaceFromFractionalNode)
- [removeSpaceFromFullNode(subarrayLink, space)](#removeSpaceFromFullNode)
- [addSpaceToFractionalNode(subarrayLink, space)](#addSpaceToFractionalNode)
- [addSpaceToFullNode(subarrayLink, space)](#addSpaceToFullNode)
- [changeNodeLastRewardDate(nodeIndex)](#changeNodeLastRewardDate)
- [isNodeExist(from, nodeIndex)](#isNodeExist)
- [isLeavingPeriodExpired(nodeIndex)](#isLeavingPeriodExpired)
- [isTimeForReward(nodeIndex)](#isTimeForReward)
- [getNodeIP(nodeIndex)](#getNodeIP)
- [getNodePort(nodeIndex)](#getNodePort)
- [getNodePublicKey(nodeIndex)](#getNodePublicKey)
- [isNodeLeaving(nodeIndex)](#isNodeLeaving)
- [isNodeLeft(nodeIndex)](#isNodeLeft)
- [getNodeLastRewardDate(nodeIndex)](#getNodeLastRewardDate)
- [getNodeNextRewardDate(nodeIndex)](#getNodeNextRewardDate)
- [getNumberOfNodes()](#getNumberOfNodes)
- [getNumberOfFractionalNodes()](#getNumberOfFractionalNodes)
- [getNumberOfFullNodes()](#getNumberOfFullNodes)
- [getNumberOnlineNodes()](#getNumberOnlineNodes)
- [getNumberOfFreeFractionalNodes(space, needNodes)](#getNumberOfFreeFractionalNodes)
- [getNumberOfFreeFullNodes(needNodes)](#getNumberOfFreeFullNodes)
- [getActiveNodeIPs()](#getActiveNodeIPs)
- [getActiveNodesByAddress()](#getActiveNodesByAddress)
- [isNodeActive(nodeIndex)](#isNodeActive)
- [getActiveNodeIds()](#getActiveNodeIds)
- [getNodesWithFreeSpace(nodesFillings, freeSpace)](#getNodesWithFreeSpace)
- [countNodesWithFreeSpace(nodesFillings, freeSpace)](#countNodesWithFreeSpace)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">uint256</span>
newLeavingPeriod
, <span class="var-type">address</span>
newContractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodesWithFreeSpace`

<div class="funcnamegetNodesWithFreeSpace contract-function">
<h4 id="getNodesWithFreeSpace">
<code>getNodesWithFreeSpace(<span class="var-type">uint256</span>
partOfNode
, <span class="var-type">uint256</span>
freeSpace
)<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addNode`

<div class="funcnameaddNode contract-function">
<h4 id="addNode">
<code>addNode(<span class="var-type">address</span>
from
, <span class="var-type">string</span>
name
, <span class="var-type">bytes4</span>
ip
, <span class="var-type">bytes4</span>
publicIP
, <span class="var-type">uint16</span>
port
, <span class="var-type">bytes</span>
publicKey
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addFractionalNode`

<div class="funcnameaddFractionalNode contract-function">
<h4 id="addFractionalNode">
<code>addFractionalNode(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addFullNode`

<div class="funcnameaddFullNode contract-function">
<h4 id="addFullNode">
<code>addFullNode(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setNodeLeaving`

<div class="funcnamesetNodeLeaving contract-function">
<h4 id="setNodeLeaving">
<code>setNodeLeaving(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `setNodeLeft`

<div class="funcnamesetNodeLeft contract-function">
<h4 id="setNodeLeft">
<code>setNodeLeft(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeFractionalNode`

<div class="funcnameremoveFractionalNode contract-function">
<h4 id="removeFractionalNode">
<code>removeFractionalNode(<span class="var-type">uint256</span>
subarrayIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeFullNode`

<div class="funcnameremoveFullNode contract-function">
<h4 id="removeFullNode">
<code>removeFullNode(<span class="var-type">uint256</span>
subarrayIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeSpaceFromFractionalNode`

<div class="funcnameremoveSpaceFromFractionalNode contract-function">
<h4 id="removeSpaceFromFractionalNode">
<code>removeSpaceFromFractionalNode(<span class="var-type">uint256</span>
subarrayLink
, <span class="var-type">uint256</span>
space
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeSpaceFromFullNode`

<div class="funcnameremoveSpaceFromFullNode contract-function">
<h4 id="removeSpaceFromFullNode">
<code>removeSpaceFromFullNode(<span class="var-type">uint256</span>
subarrayLink
, <span class="var-type">uint256</span>
space
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addSpaceToFractionalNode`

<div class="funcnameaddSpaceToFractionalNode contract-function">
<h4 id="addSpaceToFractionalNode">
<code>addSpaceToFractionalNode(<span class="var-type">uint256</span>
subarrayLink
, <span class="var-type">uint256</span>
space
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `addSpaceToFullNode`

<div class="funcnameaddSpaceToFullNode contract-function">
<h4 id="addSpaceToFullNode">
<code>addSpaceToFullNode(<span class="var-type">uint256</span>
subarrayLink
, <span class="var-type">uint256</span>
space
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `changeNodeLastRewardDate`

<div class="funcnamechangeNodeLastRewardDate contract-function">
<h4 id="changeNodeLastRewardDate">
<code>changeNodeLastRewardDate(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isNodeExist`

<div class="funcnameisNodeExist contract-function">
<h4 id="isNodeExist">
<code>isNodeExist(<span class="var-type">address</span>
from
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isLeavingPeriodExpired`

<div class="funcnameisLeavingPeriodExpired contract-function">
<h4 id="isLeavingPeriodExpired">
<code>isLeavingPeriodExpired(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isTimeForReward`

<div class="funcnameisTimeForReward contract-function">
<h4 id="isTimeForReward">
<code>isTimeForReward(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodeIP`

<div class="funcnamegetNodeIP contract-function">
<h4 id="getNodeIP">
<code>getNodeIP(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bytes4</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodePort`

<div class="funcnamegetNodePort contract-function">
<h4 id="getNodePort">
<code>getNodePort(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint16</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodePublicKey`

<div class="funcnamegetNodePublicKey contract-function">
<h4 id="getNodePublicKey">
<code>getNodePublicKey(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bytes</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isNodeLeaving`

<div class="funcnameisNodeLeaving contract-function">
<h4 id="isNodeLeaving">
<code>isNodeLeaving(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isNodeLeft`

<div class="funcnameisNodeLeft contract-function">
<h4 id="isNodeLeft">
<code>isNodeLeft(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodeLastRewardDate`

<div class="funcnamegetNodeLastRewardDate contract-function">
<h4 id="getNodeLastRewardDate">
<code>getNodeLastRewardDate(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint32</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodeNextRewardDate`

<div class="funcnamegetNodeNextRewardDate contract-function">
<h4 id="getNodeNextRewardDate">
<code>getNodeNextRewardDate(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint32</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfNodes`

<div class="funcnamegetNumberOfNodes contract-function">
<h4 id="getNumberOfNodes">
<code>getNumberOfNodes()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfFractionalNodes`

<div class="funcnamegetNumberOfFractionalNodes contract-function">
<h4 id="getNumberOfFractionalNodes">
<code>getNumberOfFractionalNodes()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfFullNodes`

<div class="funcnamegetNumberOfFullNodes contract-function">
<h4 id="getNumberOfFullNodes">
<code>getNumberOfFullNodes()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOnlineNodes`

<div class="funcnamegetNumberOnlineNodes contract-function">
<h4 id="getNumberOnlineNodes">
<code>getNumberOnlineNodes()<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfFreeFractionalNodes`

<div class="funcnamegetNumberOfFreeFractionalNodes contract-function">
<h4 id="getNumberOfFreeFractionalNodes">
<code>getNumberOfFreeFractionalNodes(<span class="var-type">uint256</span>
space
, <span class="var-type">uint256</span>
needNodes
)<span class="var-type"> → bool nodesAreEnough</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getNumberOfFreeFullNodes`

<div class="funcnamegetNumberOfFreeFullNodes contract-function">
<h4 id="getNumberOfFreeFullNodes">
<code>getNumberOfFreeFullNodes(<span class="var-type">uint256</span>
needNodes
)<span class="var-type"> → bool nodesAreEnough</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getActiveNodeIPs`

<div class="funcnamegetActiveNodeIPs contract-function">
<h4 id="getActiveNodeIPs">
<code>getActiveNodeIPs()<span class="var-type"> → bytes4[] activeNodeIPs</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getActiveNodesByAddress`

<div class="funcnamegetActiveNodesByAddress contract-function">
<h4 id="getActiveNodesByAddress">
<code>getActiveNodesByAddress()<span class="var-type"> → uint256[] activeNodesByAddress</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isNodeActive`

<div class="funcnameisNodeActive contract-function">
<h4 id="isNodeActive">
<code>isNodeActive(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `getActiveNodeIds`

<div class="funcnamegetActiveNodeIds contract-function">
<h4 id="getActiveNodeIds">
<code>getActiveNodeIds()<span class="var-type"> → uint256[] activeNodeIds</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `getNodesWithFreeSpace`

<div class="funcnamegetNodesWithFreeSpace contract-function">
<h4 id="getNodesWithFreeSpace">
<code>getNodesWithFreeSpace(<span class="var-type">struct NodesData.NodeFilling[]</span>
nodesFillings
, <span class="var-type">uint256</span>
freeSpace
)<span class="var-type"> → uint256[]</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `countNodesWithFreeSpace`

<div class="funcnamecountNodesWithFreeSpace contract-function">
<h4 id="countNodesWithFreeSpace">
<code>countNodesWithFreeSpace(<span class="var-type">struct NodesData.NodeFilling[]</span>
nodesFillings
, <span class="var-type">uint256</span>
freeSpace
)<span class="var-type"> → uint256 count</span></code>
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