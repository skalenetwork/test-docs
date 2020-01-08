# `IDelegatableToken`

 Token that can be used for delegation, unlocked

--- 


## Functions

- [getLockedOf(wallet)](#getLockedOf)
- [getDelegatedOf(wallet)](#getDelegatedOf)

--- 




##### `getLockedOf`

<div class="funcnamegetLockedOf contract-function">
<h4 id="getLockedOf">
<code>getLockedOf(<span class="var-type">address</span>
wallet
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> returns if the token is locked
 </p>
</div>
</div>

##### `getDelegatedOf`

<div class="funcnamegetDelegatedOf contract-function">
<h4 id="getDelegatedOf">
<code>getDelegatedOf(<span class="var-type">address</span>
wallet
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">

 <p> returns if the token is delegated
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