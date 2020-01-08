# `DelegationPeriodManager`

 Manager handles the values for the stake multiplier <br>
or delegation periods that are supported by the network

--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [getStakeMultiplier(monthsCount)](#getStakeMultiplier)
- [getDelegationPeriods()](#getDelegationPeriods)
- [setDelegationPeriod(monthsCount, stakeMultiplier)](#setDelegationPeriod)
- [removeDelegationPeriod(monthsCount)](#removeDelegationPeriod)
- [isDelegationPeriodAllowed(monthsCount)](#isDelegationPeriodAllowed)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">address</span>
newContractsAddress
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">

 <p> constructor which registers newContractsAddress
 </p>
</div>
</div>

##### `getStakeMultiplier`

<div class="funcnamegetStakeMultiplier contract-function">
<h4 id="getStakeMultiplier">
<code>getStakeMultiplier(<span class="var-type">uint256</span>
monthsCount
)<span class="var-type"> → uint256</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Returns the stake multiplier for this delegation period  <br>
A multiplier to calculate the various yields per delegation period. e.g. 3m = 1, 6m = 1.5, 12m = 2
 </p>
</div>
</div>

##### `getDelegationPeriods`

<div class="funcnamegetDelegationPeriods contract-function">
<h4 id="getDelegationPeriods">
<code>getDelegationPeriods()<span class="var-type"> → uint256[]</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Returns the set of allowed delegation period
 </p>
</div>
</div>

##### `setDelegationPeriod`

<div class="funcnamesetDelegationPeriod contract-function">
<h4 id="setDelegationPeriod">
<code>setDelegationPeriod(<span class="var-type">uint256</span>
monthsCount
, <span class="var-type">uint256</span>
stakeMultiplier
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> checks whether the delegation period is allowed in the system
 </p>
</div>
</div>

##### `removeDelegationPeriod`

<div class="funcnameremoveDelegationPeriod contract-function">
<h4 id="removeDelegationPeriod">
<code>removeDelegationPeriod(<span class="var-type">uint256</span>
monthsCount
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> removes a delegation period from the stake multiplier. </br>
 </p>
</div>
</div>

##### `isDelegationPeriodAllowed`

<div class="funcnameisDelegationPeriodAllowed contract-function">
<h4 id="isDelegationPeriodAllowed">
<code>isDelegationPeriodAllowed(<span class="var-type">uint256</span>
monthsCount
)<span class="var-type"> → bool</span></code>
<span class="item">public</span>
</h4>
<div class="description">

 <p> checks whether the delegation period is allowed in the system
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