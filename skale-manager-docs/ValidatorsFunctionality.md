# `ValidatorsFunctionality`



--- 


## Functions

- [constructor(newExecutorName, newDataName, newContractsAddress)](#constructor)
- [addValidator(nodeIndex)](#addValidator)
- [upgradeValidator(nodeIndex)](#upgradeValidator)
- [deleteValidatorByRoot(nodeIndex)](#deleteValidatorByRoot)
- [sendVerdict(fromValidatorIndex, toNodeIndex, downtime, latency)](#sendVerdict)
- [calculateMetrics(nodeIndex)](#calculateMetrics)
- [rotateNode(schainId)](#rotateNode)
- [selectNodeToGroup(groupIndex)](#selectNodeToGroup)
- [generateGroup(groupIndex)](#generateGroup)
- [median(values)](#median)
- [setNumberOfNodesInGroup(groupIndex, groupData)](#setNumberOfNodesInGroup)
- [comparator(groupIndex, indexOfNode)](#comparator)
- [setValidators(groupIndex, nodeIndex)](#setValidators)
- [find(validatorIndex, nodeIndex)](#find)
- [quickSort(array, left, right)](#quickSort)
- [getDataFromBytes(data)](#getDataFromBytes)
- [getDataToBytes(nodeIndex)](#getDataToBytes)

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

##### `addValidator`

<div class="funcnameaddValidator contract-function">
<h4 id="addValidator">
<code>addValidator(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> addValidator - setup validators of node </p>
</div>
</div>

##### `upgradeValidator`

<div class="funcnameupgradeValidator contract-function">
<h4 id="upgradeValidator">
<code>upgradeValidator(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteValidatorByRoot`

<div class="funcnamedeleteValidatorByRoot contract-function">
<h4 id="deleteValidatorByRoot">
<code>deleteValidatorByRoot(<span class="var-type">uint256</span>
nodeIndex
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

##### `calculateMetrics`

<div class="funcnamecalculateMetrics contract-function">
<h4 id="calculateMetrics">
<code>calculateMetrics(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint32 averageDowntime, uint32 averageLatency</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `rotateNode`

<div class="funcnamerotateNode contract-function">
<h4 id="rotateNode">
<code>rotateNode(<span class="var-type">bytes32</span>
schainId
)<span class="var-type"></span></code>
<span class="item">external</span>
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
)<span class="var-type"> → uint256[]</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `median`

<div class="funcnamemedian contract-function">
<h4 id="median">
<code>median(<span class="var-type">uint32[]</span>
values
)<span class="var-type"> → uint32</span></code>
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
, <span class="var-type">bytes32</span>
groupData
)<span class="var-type"> → uint256 numberOfNodes, uint256 finish</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `comparator`

<div class="funcnamecomparator contract-function">
<h4 id="comparator">
<code>comparator(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
indexOfNode
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `setValidators`

<div class="funcnamesetValidators contract-function">
<h4 id="setValidators">
<code>setValidators(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `find`

<div class="funcnamefind contract-function">
<h4 id="find">
<code>find(<span class="var-type">bytes32</span>
validatorIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256 index, uint32 time</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `quickSort`

<div class="funcnamequickSort contract-function">
<h4 id="quickSort">
<code>quickSort(<span class="var-type">uint32[]</span>
array
, <span class="var-type">uint256</span>
left
, <span class="var-type">uint256</span>
right
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `getDataFromBytes`

<div class="funcnamegetDataFromBytes contract-function">
<h4 id="getDataFromBytes">
<code>getDataFromBytes(<span class="var-type">bytes32</span>
data
)<span class="var-type"> → uint256 index, uint32 time</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `getDataToBytes`

<div class="funcnamegetDataToBytes contract-function">
<h4 id="getDataToBytes">
<code>getDataToBytes(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bytes32 bytesParameters</span></code>
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