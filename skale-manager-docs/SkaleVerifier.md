# `SkaleVerifier`



--- 


## Functions

- [constructor(newContractsAddress)](#constructor)
- [verifySchainSignature(signA, signB, hash, counter, hashA, hashB, schainName)](#verifySchainSignature)
- [verify(signA, signB, hash, counter, hashA, hashB, pkx1, pky1, pkx2, pky2)](#verify)
- [checkHashToGroupWithHelper(hash, counter, hashA, hashB)](#checkHashToGroupWithHelper)

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


</div>
</div>

##### `verifySchainSignature`

<div class="funcnameverifySchainSignature contract-function">
<h4 id="verifySchainSignature">
<code>verifySchainSignature(<span class="var-type">uint256</span>
signA
, <span class="var-type">uint256</span>
signB
, <span class="var-type">bytes32</span>
hash
, <span class="var-type">uint256</span>
counter
, <span class="var-type">uint256</span>
hashA
, <span class="var-type">uint256</span>
hashB
, <span class="var-type">string</span>
schainName
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `verify`

<div class="funcnameverify contract-function">
<h4 id="verify">
<code>verify(<span class="var-type">uint256</span>
signA
, <span class="var-type">uint256</span>
signB
, <span class="var-type">bytes32</span>
hash
, <span class="var-type">uint256</span>
counter
, <span class="var-type">uint256</span>
hashA
, <span class="var-type">uint256</span>
hashB
, <span class="var-type">uint256</span>
pkx1
, <span class="var-type">uint256</span>
pky1
, <span class="var-type">uint256</span>
pkx2
, <span class="var-type">uint256</span>
pky2
)<span class="var-type"> → bool</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `checkHashToGroupWithHelper`

<div class="funcnamecheckHashToGroupWithHelper contract-function">
<h4 id="checkHashToGroupWithHelper">
<code>checkHashToGroupWithHelper(<span class="var-type">bytes32</span>
hash
, <span class="var-type">uint256</span>
counter
, <span class="var-type">uint256</span>
hashA
, <span class="var-type">uint256</span>
hashB
)<span class="var-type"> → bool</span></code>
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