# `ValidatorsData`



--- 


## Functions

- [constructor(newExecutorName, newContractsAddress)](#constructor)
- [addValidatedNode(validatorIndex, data)](#addValidatedNode)
- [addVerdict(validatorIndex, downtime, latency)](#addVerdict)
- [removeValidatedNode(validatorIndex, indexOfValidatedNode)](#removeValidatedNode)
- [removeAllValidatedNodes(validatorIndex)](#removeAllValidatedNodes)
- [removeAllVerdicts(validatorIndex)](#removeAllVerdicts)
- [getValidatedArray(validatorIndex)](#getValidatedArray)
- [getLengthOfMetrics(validatorIndex)](#getLengthOfMetrics)

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

##### `addValidatedNode`

<div class="funcnameaddValidatedNode contract-function">
<h4 id="addValidatedNode">
<code>addValidatedNode(<span class="var-type">bytes32</span>
validatorIndex
, <span class="var-type">bytes32</span>
data
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Add validated node or update existing one if it is already exits </p>
</div>
</div>

##### `addVerdict`

<div class="funcnameaddVerdict contract-function">
<h4 id="addVerdict">
<code>addVerdict(<span class="var-type">bytes32</span>
validatorIndex
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

##### `removeValidatedNode`

<div class="funcnameremoveValidatedNode contract-function">
<h4 id="removeValidatedNode">
<code>removeValidatedNode(<span class="var-type">bytes32</span>
validatorIndex
, <span class="var-type">uint256</span>
indexOfValidatedNode
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeAllValidatedNodes`

<div class="funcnameremoveAllValidatedNodes contract-function">
<h4 id="removeAllValidatedNodes">
<code>removeAllValidatedNodes(<span class="var-type">bytes32</span>
validatorIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `removeAllVerdicts`

<div class="funcnameremoveAllVerdicts contract-function">
<h4 id="removeAllVerdicts">
<code>removeAllVerdicts(<span class="var-type">bytes32</span>
validatorIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getValidatedArray`

<div class="funcnamegetValidatedArray contract-function">
<h4 id="getValidatedArray">
<code>getValidatedArray(<span class="var-type">bytes32</span>
validatorIndex
)<span class="var-type"> → bytes32[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `getLengthOfMetrics`

<div class="funcnamegetLengthOfMetrics contract-function">
<h4 id="getLengthOfMetrics">
<code>getLengthOfMetrics(<span class="var-type">bytes32</span>
validatorIndex
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