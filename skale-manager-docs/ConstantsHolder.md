# `ConstantsHolder`



--- 


## Functions

- [constructor(contractsAddress)](#constructor)
- [setPeriods(newRewardPeriod, newDeltaPeriod)](#setPeriods)
- [setCheckTime(newCheckTime)](#setCheckTime)
- [setLastTimeUnderloaded()](#setLastTimeUnderloaded)
- [setLastTimeOverloaded()](#setLastTimeOverloaded)
- [setLatency(newAllowableLatency)](#setLatency)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">address</span>
contractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `setPeriods`

<div class="funcnamesetPeriods contract-function">
<h4 id="setPeriods">
<code>setPeriods(<span class="var-type">uint32</span>
newRewardPeriod
, <span class="var-type">uint32</span>
newDeltaPeriod
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Set reward and delta periods to new one, run only by owner. This function
only for tests.
 </p>
</div>
</div>

##### `setCheckTime`

<div class="funcnamesetCheckTime contract-function">
<h4 id="setCheckTime">
<code>setCheckTime(<span class="var-type">uint8</span>
newCheckTime
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Set new check time. This function only for tests.
 </p>
</div>
</div>

##### `setLastTimeUnderloaded`

<div class="funcnamesetLastTimeUnderloaded contract-function">
<h4 id="setLastTimeUnderloaded">
<code>setLastTimeUnderloaded()<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Set time if system underloaded, run only by NodesFunctionality contract </p>
</div>
</div>

##### `setLastTimeOverloaded`

<div class="funcnamesetLastTimeOverloaded contract-function">
<h4 id="setLastTimeOverloaded">
<code>setLastTimeOverloaded()<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Set time if system iverloaded, run only by SchainsFunctionality contract </p>
</div>
</div>

##### `setLatency`

<div class="funcnamesetLatency contract-function">
<h4 id="setLatency">
<code>setLatency(<span class="var-type">uint32</span>
newAllowableLatency
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Set latency new one in ms, run only by owner. This function
only for tests.
 </p>
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