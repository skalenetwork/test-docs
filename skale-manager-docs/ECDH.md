# `ECDH`



--- 


## Functions

- [publicKey(privKey)](#publicKey)
- [deriveKey(privKey, pubX, pubY)](#deriveKey)
- [jAdd(x1, z1, x2, z2)](#jAdd)
- [jSub(x1, z1, x2, z2)](#jSub)
- [jMul(x1, z1, x2, z2)](#jMul)
- [jDiv(x1, z1, x2, z2)](#jDiv)
- [inverse(a)](#inverse)
- [ecAdd(x1, y1, z1, x2, y2, z2)](#ecAdd)
- [ecDouble(x1, y1, z1)](#ecDouble)
- [ecMul(d, x1, y1, z1)](#ecMul)

--- 




##### `publicKey`

<div class="funcnamepublicKey contract-function">
<h4 id="publicKey">
<code>publicKey(<span class="var-type">uint256</span>
privKey
)<span class="var-type"> → uint256 qx, uint256 qy</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deriveKey`

<div class="funcnamederiveKey contract-function">
<h4 id="deriveKey">
<code>deriveKey(<span class="var-type">uint256</span>
privKey
, <span class="var-type">uint256</span>
pubX
, <span class="var-type">uint256</span>
pubY
)<span class="var-type"> → uint256 qx, uint256 qy</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `jAdd`

<div class="funcnamejAdd contract-function">
<h4 id="jAdd">
<code>jAdd(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
z1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
z2
)<span class="var-type"> → uint256 x3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `jSub`

<div class="funcnamejSub contract-function">
<h4 id="jSub">
<code>jSub(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
z1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
z2
)<span class="var-type"> → uint256 x3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `jMul`

<div class="funcnamejMul contract-function">
<h4 id="jMul">
<code>jMul(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
z1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
z2
)<span class="var-type"> → uint256 x3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `jDiv`

<div class="funcnamejDiv contract-function">
<h4 id="jDiv">
<code>jDiv(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
z1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
z2
)<span class="var-type"> → uint256 x3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `inverse`

<div class="funcnameinverse contract-function">
<h4 id="inverse">
<code>inverse(<span class="var-type">uint256</span>
a
)<span class="var-type"> → uint256 invA</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `ecAdd`

<div class="funcnameecAdd contract-function">
<h4 id="ecAdd">
<code>ecAdd(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
y1
, <span class="var-type">uint256</span>
z1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
y2
, <span class="var-type">uint256</span>
z2
)<span class="var-type"> → uint256 x3, uint256 y3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `ecDouble`

<div class="funcnameecDouble contract-function">
<h4 id="ecDouble">
<code>ecDouble(<span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
y1
, <span class="var-type">uint256</span>
z1
)<span class="var-type"> → uint256 x3, uint256 y3, uint256 z3</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `ecMul`

<div class="funcnameecMul contract-function">
<h4 id="ecMul">
<code>ecMul(<span class="var-type">uint256</span>
d
, <span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
y1
, <span class="var-type">uint256</span>
z1
)<span class="var-type"> → uint256 x3, uint256 y3, uint256 z3</span></code>
<span class="item">public</span>
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