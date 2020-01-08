# `IValidatorsFunctionality`



--- 


## Functions

- [addValidator(nodeIndex)](#addValidator)
- [upgradeValidator(nodeIndex)](#upgradeValidator)
- [sendVerdict(fromValidatorIndex, toNodeIndex, downtime, latency)](#sendVerdict)
- [calculateMetrics(nodeIndex)](#calculateMetrics)
- [deleteValidatorByRoot(nodeIndex)](#deleteValidatorByRoot)

--- 




##### `addValidator`

<div class="funcnameaddValidator contract-function">
<h4 id="addValidator">
<code>addValidator(<span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


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
)<span class="var-type"> → uint32, uint32</span></code>
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