# `ITokenSaleManager`

 Token Sale Manager will initially hold all tokens for the sale and allow users to retrieve them

--- 


## Functions

- [approve(walletAddress, value)](#approve)
- [retrieve()](#retrieve)
- [registerSeller(seller)](#registerSeller)

--- 




##### `approve`

<div class="funcnameapprove contract-function">
<h4 id="approve">
<code>approve(<span class="var-type">address[]</span>
walletAddress
, <span class="var-type">uint256[]</span>
value
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Allocates values for `walletAddresses` 
At the end of the sale token approval function will be called (can be called multiple times)
 </p>
</div>
</div>

##### `retrieve`

<div class="funcnameretrieve contract-function">
<h4 id="retrieve">
<code>retrieve()<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p>  Transfers the entire value to sender address. Tokens are locked. 
Each sale participant calls retrieve() - the entire value is transferred to walletAddress
After the transfer, the token in walletAddress will be locked through DelegationService contract
User will be able to see the token in the wallet. </p>
</div>
</div>

##### `registerSeller`

<div class="funcnameregisterSeller contract-function">
<h4 id="registerSeller">
<code>registerSeller(<span class="var-type">address</span>
seller
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> Allows seller address to approve tokens transfers
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