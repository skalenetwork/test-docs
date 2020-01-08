# `SkaleDKG`



--- 

## Modifiers
- [correctGroup(groupIndex)](#correctGroup)
- [correctNode(groupIndex, nodeIndex)](#correctNode)

--- 


## Functions

- [constructor(contractsAddress)](#constructor)
- [openChannel(groupIndex)](#openChannel)
- [deleteChannel(groupIndex)](#deleteChannel)
- [broadcast(groupIndex, nodeIndex, verificationVector, secretKeyContribution)](#broadcast)
- [complaint(groupIndex, fromNodeIndex, toNodeIndex)](#complaint)
- [response(groupIndex, fromNodeIndex, secretNumber, multipliedShare)](#response)
- [allright(groupIndex, fromNodeIndex)](#allright)
- [isChannelOpened(groupIndex)](#isChannelOpened)
- [verify(index, secret, multipliedShare, verificationVector)](#verify)
- [getCommonPublicKey(groupIndex, secretNumber)](#getCommonPublicKey)
- [decryptMessage(groupIndex, secretNumber)](#decryptMessage)
- [adding(groupIndex, x1, y1, x2, y2)](#adding)
- [isBroadcast(groupIndex, nodeIndex, sc, vv)](#isBroadcast)
- [isBroadcasted(groupIndex, nodeIndex)](#isBroadcasted)
- [findNode(groupIndex, nodeIndex)](#findNode)
- [isNodeByMessageSender(nodeIndex, from)](#isNodeByMessageSender)
- [addFp2(a, b)](#addFp2)
- [scalarMulFp2(scalar, a)](#scalarMulFp2)
- [minusFp2(a, b)](#minusFp2)
- [mulFp2(a, b)](#mulFp2)
- [squaredFp2(a)](#squaredFp2)
- [inverseFp2(a)](#inverseFp2)
- [isG2Zero(x, y)](#isG2Zero)
- [doubleG2(x1, y1)](#doubleG2)
- [u1(x1)](#u1)
- [u2(x2)](#u2)
- [s1(y1)](#s1)
- [s2(y2)](#s2)
- [isEqual(u1Value, u2Value, s1Value, s2Value)](#isEqual)
- [addG2(x1, y1, x2, y2)](#addG2)
- [mulG2(scalar, x1, y1)](#mulG2)
- [bigModExp(base, power)](#bigModExp)
- [loop(index, verificationVector, loopIndex)](#loop)
- [checkDKGVerification(valX, valY, multipliedShare)](#checkDKGVerification)
- [checkCorrectMultipliedShare(multipliedShare, secret)](#checkCorrectMultipliedShare)
- [bytesToPublicKey(someBytes)](#bytesToPublicKey)
- [bytesToG2(someBytes)](#bytesToG2)

--- 



##### `correctGroup`

<div class="funcnamecorrectGroup contract-function">
<h4 id="correctGroup"><a class="anchor" href="#correctGroup"></a>
<code>correctGroup(<span class="var-type">bytes32</span>
groupIndex
) <span class="var-type"></span></code>
<span class="item"></span>
</h4>
<div class="description">


</div>
</div>

##### `correctNode`

<div class="funcnamecorrectNode contract-function">
<h4 id="correctNode"><a class="anchor" href="#correctNode"></a>
<code>correctNode(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
) <span class="var-type"></span></code>
<span class="item"></span>
</h4>
<div class="description">


</div>
</div>

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

##### `openChannel`

<div class="funcnameopenChannel contract-function">
<h4 id="openChannel">
<code>openChannel(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `deleteChannel`

<div class="funcnamedeleteChannel contract-function">
<h4 id="deleteChannel">
<code>deleteChannel(<span class="var-type">bytes32</span>
groupIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `broadcast`

<div class="funcnamebroadcast contract-function">
<h4 id="broadcast">
<code>broadcast(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes</span>
verificationVector
, <span class="var-type">bytes</span>
secretKeyContribution
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `complaint`

<div class="funcnamecomplaint contract-function">
<h4 id="complaint">
<code>complaint(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
fromNodeIndex
, <span class="var-type">uint256</span>
toNodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `response`

<div class="funcnameresponse contract-function">
<h4 id="response">
<code>response(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
fromNodeIndex
, <span class="var-type">uint256</span>
secretNumber
, <span class="var-type">bytes</span>
multipliedShare
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `allright`

<div class="funcnameallright contract-function">
<h4 id="allright">
<code>allright(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
fromNodeIndex
)<span class="var-type"></span></code>
<span class="item">external</span>
</h4>
<div class="description">


</div>
</div>

##### `isChannelOpened`

<div class="funcnameisChannelOpened contract-function">
<h4 id="isChannelOpened">
<code>isChannelOpened(<span class="var-type">bytes32</span>
groupIndex
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
index
, <span class="var-type">uint256</span>
secret
, <span class="var-type">bytes</span>
multipliedShare
, <span class="var-type">bytes</span>
verificationVector
)<span class="var-type"> → bool</span></code>
<span class="item">public</span>
</h4>
<div class="description">


</div>
</div>

##### `getCommonPublicKey`

<div class="funcnamegetCommonPublicKey contract-function">
<h4 id="getCommonPublicKey">
<code>getCommonPublicKey(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
secretNumber
)<span class="var-type"> → bytes32 key</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `decryptMessage`

<div class="funcnamedecryptMessage contract-function">
<h4 id="decryptMessage">
<code>decryptMessage(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
secretNumber
)<span class="var-type"> → uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `adding`

<div class="funcnameadding contract-function">
<h4 id="adding">
<code>adding(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
x1
, <span class="var-type">uint256</span>
y1
, <span class="var-type">uint256</span>
x2
, <span class="var-type">uint256</span>
y2
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isBroadcast`

<div class="funcnameisBroadcast contract-function">
<h4 id="isBroadcast">
<code>isBroadcast(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">bytes</span>
sc
, <span class="var-type">bytes</span>
vv
)<span class="var-type"></span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isBroadcasted`

<div class="funcnameisBroadcasted contract-function">
<h4 id="isBroadcasted">
<code>isBroadcasted(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `findNode`

<div class="funcnamefindNode contract-function">
<h4 id="findNode">
<code>findNode(<span class="var-type">bytes32</span>
groupIndex
, <span class="var-type">uint256</span>
nodeIndex
)<span class="var-type"> → uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isNodeByMessageSender`

<div class="funcnameisNodeByMessageSender contract-function">
<h4 id="isNodeByMessageSender">
<code>isNodeByMessageSender(<span class="var-type">uint256</span>
nodeIndex
, <span class="var-type">address</span>
from
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `addFp2`

<div class="funcnameaddFp2 contract-function">
<h4 id="addFp2">
<code>addFp2(<span class="var-type">struct SkaleDKG.Fp2</span>
a
, <span class="var-type">struct SkaleDKG.Fp2</span>
b
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `scalarMulFp2`

<div class="funcnamescalarMulFp2 contract-function">
<h4 id="scalarMulFp2">
<code>scalarMulFp2(<span class="var-type">uint256</span>
scalar
, <span class="var-type">struct SkaleDKG.Fp2</span>
a
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `minusFp2`

<div class="funcnameminusFp2 contract-function">
<h4 id="minusFp2">
<code>minusFp2(<span class="var-type">struct SkaleDKG.Fp2</span>
a
, <span class="var-type">struct SkaleDKG.Fp2</span>
b
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `mulFp2`

<div class="funcnamemulFp2 contract-function">
<h4 id="mulFp2">
<code>mulFp2(<span class="var-type">struct SkaleDKG.Fp2</span>
a
, <span class="var-type">struct SkaleDKG.Fp2</span>
b
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `squaredFp2`

<div class="funcnamesquaredFp2 contract-function">
<h4 id="squaredFp2">
<code>squaredFp2(<span class="var-type">struct SkaleDKG.Fp2</span>
a
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `inverseFp2`

<div class="funcnameinverseFp2 contract-function">
<h4 id="inverseFp2">
<code>inverseFp2(<span class="var-type">struct SkaleDKG.Fp2</span>
a
)<span class="var-type"> → struct SkaleDKG.Fp2 x</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isG2Zero`

<div class="funcnameisG2Zero contract-function">
<h4 id="isG2Zero">
<code>isG2Zero(<span class="var-type">struct SkaleDKG.Fp2</span>
x
, <span class="var-type">struct SkaleDKG.Fp2</span>
y
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `doubleG2`

<div class="funcnamedoubleG2 contract-function">
<h4 id="doubleG2">
<code>doubleG2(<span class="var-type">struct SkaleDKG.Fp2</span>
x1
, <span class="var-type">struct SkaleDKG.Fp2</span>
y1
)<span class="var-type"> → struct SkaleDKG.Fp2 x3, struct SkaleDKG.Fp2 y3</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `u1`

<div class="funcnameu1 contract-function">
<h4 id="u1">
<code>u1(<span class="var-type">struct SkaleDKG.Fp2</span>
x1
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `u2`

<div class="funcnameu2 contract-function">
<h4 id="u2">
<code>u2(<span class="var-type">struct SkaleDKG.Fp2</span>
x2
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `s1`

<div class="funcnames1 contract-function">
<h4 id="s1">
<code>s1(<span class="var-type">struct SkaleDKG.Fp2</span>
y1
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `s2`

<div class="funcnames2 contract-function">
<h4 id="s2">
<code>s2(<span class="var-type">struct SkaleDKG.Fp2</span>
y2
)<span class="var-type"> → struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `isEqual`

<div class="funcnameisEqual contract-function">
<h4 id="isEqual">
<code>isEqual(<span class="var-type">struct SkaleDKG.Fp2</span>
u1Value
, <span class="var-type">struct SkaleDKG.Fp2</span>
u2Value
, <span class="var-type">struct SkaleDKG.Fp2</span>
s1Value
, <span class="var-type">struct SkaleDKG.Fp2</span>
s2Value
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `addG2`

<div class="funcnameaddG2 contract-function">
<h4 id="addG2">
<code>addG2(<span class="var-type">struct SkaleDKG.Fp2</span>
x1
, <span class="var-type">struct SkaleDKG.Fp2</span>
y1
, <span class="var-type">struct SkaleDKG.Fp2</span>
x2
, <span class="var-type">struct SkaleDKG.Fp2</span>
y2
)<span class="var-type"> → struct SkaleDKG.Fp2 x3, struct SkaleDKG.Fp2 y3</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `mulG2`

<div class="funcnamemulG2 contract-function">
<h4 id="mulG2">
<code>mulG2(<span class="var-type">uint256</span>
scalar
, <span class="var-type">struct SkaleDKG.Fp2</span>
x1
, <span class="var-type">struct SkaleDKG.Fp2</span>
y1
)<span class="var-type"> → struct SkaleDKG.Fp2 x, struct SkaleDKG.Fp2 y</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `bigModExp`

<div class="funcnamebigModExp contract-function">
<h4 id="bigModExp">
<code>bigModExp(<span class="var-type">uint256</span>
base
, <span class="var-type">uint256</span>
power
)<span class="var-type"> → uint256</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `loop`

<div class="funcnameloop contract-function">
<h4 id="loop">
<code>loop(<span class="var-type">uint256</span>
index
, <span class="var-type">bytes</span>
verificationVector
, <span class="var-type">uint256</span>
loopIndex
)<span class="var-type"> → struct SkaleDKG.Fp2, struct SkaleDKG.Fp2</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `checkDKGVerification`

<div class="funcnamecheckDKGVerification contract-function">
<h4 id="checkDKGVerification">
<code>checkDKGVerification(<span class="var-type">struct SkaleDKG.Fp2</span>
valX
, <span class="var-type">struct SkaleDKG.Fp2</span>
valY
, <span class="var-type">bytes</span>
multipliedShare
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `checkCorrectMultipliedShare`

<div class="funcnamecheckCorrectMultipliedShare contract-function">
<h4 id="checkCorrectMultipliedShare">
<code>checkCorrectMultipliedShare(<span class="var-type">bytes</span>
multipliedShare
, <span class="var-type">uint256</span>
secret
)<span class="var-type"> → bool</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `bytesToPublicKey`

<div class="funcnamebytesToPublicKey contract-function">
<h4 id="bytesToPublicKey">
<code>bytesToPublicKey(<span class="var-type">bytes</span>
someBytes
)<span class="var-type"> → uint256 x, uint256 y</span></code>
<span class="item">internal</span>
</h4>
<div class="description">


</div>
</div>

##### `bytesToG2`

<div class="funcnamebytesToG2 contract-function">
<h4 id="bytesToG2">
<code>bytesToG2(<span class="var-type">bytes</span>
someBytes
)<span class="var-type"> → struct SkaleDKG.Fp2 x, struct SkaleDKG.Fp2 y</span></code>
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