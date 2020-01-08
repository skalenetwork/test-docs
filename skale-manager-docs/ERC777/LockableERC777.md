# `LockableERC777`



--- 


## Functions

- [constructor(name, symbol, defaultOperators)](#constructor)
- [send(recipient, amount, data)](#send)
- [transfer(recipient, amount)](#transfer)
- [burn(amount, data)](#burn)
- [authorizeOperator(operator)](#authorizeOperator)
- [revokeOperator(operator)](#revokeOperator)
- [operatorSend(sender, recipient, amount, data, operatorData)](#operatorSend)
- [operatorBurn(account, amount, data, operatorData)](#operatorBurn)
- [approve(spender, value)](#approve)
- [transferFrom(holder, recipient, amount)](#transferFrom)
- [name()](#name)
- [symbol()](#symbol)
- [decimals()](#decimals)
- [granularity()](#granularity)
- [totalSupply()](#totalSupply)
- [balanceOf(tokenHolder)](#balanceOf)
- [isOperatorFor(operator, tokenHolder)](#isOperatorFor)
- [defaultOperators()](#defaultOperators)
- [allowance(holder, spender)](#allowance)
- [_mint(operator, account, amount, userData, operatorData)](#_mint)

--- 




##### `constructor`

<div class="funcnameconstructor contract-function">
<h4 id="constructor">
<code>constructor(<span class="var-type">string</span>
name
, <span class="var-type">string</span>
symbol
, <span class="var-type">address[]</span>
defaultOperators
)<span class="var-type"></span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `send`

<div class="funcnamesend contract-function">
<h4 id="send">
<code>send(<span class="var-type">address</span>
recipient
, <span class="var-type">uint256</span>
amount
, <span class="var-type">bytes</span>
data
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `transfer`

<div class="funcnametransfer contract-function">
<h4 id="transfer">
<code>transfer(<span class="var-type">address</span>
recipient
, <span class="var-type">uint256</span>
amount
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `burn`

<div class="funcnameburn contract-function">
<h4 id="burn">
<code>burn(<span class="var-type">uint256</span>
amount
, <span class="var-type">bytes</span>
data
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `authorizeOperator`

<div class="funcnameauthorizeOperator contract-function">
<h4 id="authorizeOperator">
<code>authorizeOperator(<span class="var-type">address</span>
operator
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `revokeOperator`

<div class="funcnamerevokeOperator contract-function">
<h4 id="revokeOperator">
<code>revokeOperator(<span class="var-type">address</span>
operator
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `operatorSend`

<div class="funcnameoperatorSend contract-function">
<h4 id="operatorSend">
<code>operatorSend(<span class="var-type">address</span>
sender
, <span class="var-type">address</span>
recipient
, <span class="var-type">uint256</span>
amount
, <span class="var-type">bytes</span>
data
, <span class="var-type">bytes</span>
operatorData
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `operatorBurn`

<div class="funcnameoperatorBurn contract-function">
<h4 id="operatorBurn">
<code>operatorBurn(<span class="var-type">address</span>
account
, <span class="var-type">uint256</span>
amount
, <span class="var-type">bytes</span>
data
, <span class="var-type">bytes</span>
operatorData
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `approve`

<div class="funcnameapprove contract-function">
<h4 id="approve">
<code>approve(<span class="var-type">address</span>
spender
, <span class="var-type">uint256</span>
value
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `transferFrom`

<div class="funcnametransferFrom contract-function">
<h4 id="transferFrom">
<code>transferFrom(<span class="var-type">address</span>
holder
, <span class="var-type">address</span>
recipient
, <span class="var-type">uint256</span>
amount
)<span class="var-type"> → bool</span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `name`

<div class="funcnamename contract-function">
<h4 id="name">
<code>name()<span class="var-type"> → string</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `symbol`

<div class="funcnamesymbol contract-function">
<h4 id="symbol">
<code>symbol()<span class="var-type"> → string</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `decimals`

<div class="funcnamedecimals contract-function">
<h4 id="decimals">
<code>decimals()<span class="var-type"> → uint8</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `granularity`

<div class="funcnamegranularity contract-function">
<h4 id="granularity">
<code>granularity()<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `totalSupply`

<div class="funcnametotalSupply contract-function">
<h4 id="totalSupply">
<code>totalSupply()<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `balanceOf`

<div class="funcnamebalanceOf contract-function">
<h4 id="balanceOf">
<code>balanceOf(<span class="var-type">address</span>
tokenHolder
)<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `isOperatorFor`

<div class="funcnameisOperatorFor contract-function">
<h4 id="isOperatorFor">
<code>isOperatorFor(<span class="var-type">address</span>
operator
, <span class="var-type">address</span>
tokenHolder
)<span class="var-type"> → bool</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `defaultOperators`

<div class="funcnamedefaultOperators contract-function">
<h4 id="defaultOperators">
<code>defaultOperators()<span class="var-type"> → address[]</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `allowance`

<div class="funcnameallowance contract-function">
<h4 id="allowance">
<code>allowance(<span class="var-type">address</span>
holder
, <span class="var-type">address</span>
spender
)<span class="var-type"> → uint256</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `_mint`

<div class="funcname_mint contract-function">
<h4 id="_mint">
<code>_mint(<span class="var-type">address</span>
operator
, <span class="var-type">address</span>
account
, <span class="var-type">uint256</span>
amount
, <span class="var-type">bytes</span>
userData
, <span class="var-type">bytes</span>
operatorData
)<span class="var-type"></span></code>
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