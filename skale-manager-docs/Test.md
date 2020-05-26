# `DelegationController`

This contract performs all delegation functions including delegation
requests, undelegation, slashing, etc.

Delegators and validators may both perform delegations. Validators who perform
delegations to themselves are effectively self-delegating or self-bonding.

Delegated tokens may be in one of several states:

- PROPOSED: token holder proposes tokens to delegate to a validator
- ACCEPTED: token delegations are accepted by a validator and are locked-by-delegation
- CANCELED: token holder cancels delegation proposal. Only allowed before the proposal is accepted by the validator
- REJECTED: token proposal expires at the UTC start of the next month
- DELEGATED: accepted delegations are delegated at the UTC start of the month
- UNDELEGATION_REQUESTED: token holder requests delegations to undelegate from the validator
- COMPLETED: undelegation request is completed at the end of the delegation period


<div class="funcnameDelegationController contract-index">Modifiers</div>
---
[<code>checkDelegationExists(delegationId)</code>](DelegationController-checkDelegationExists)

<span class="inherited-title">ILocker</span>

<span class="inherited-title">Permissions</span>
[<code>allow(contractName)</code>](Permissions-allow)
[<code>allowTwo(contractName1, contractName2)</code>](Permissions-allowTwo)
[<code>allowThree(contractName1, contractName2, contractName3)</code>](Permissions-allowThree)

<span class="inherited-title">OwnableUpgradeSafe</span>
[<code>onlyOwner()</code>](OwnableUpgradeSafe-onlyOwner)

<span class="inherited-title">ContextUpgradeSafe</span>

<span class="inherited-title">Initializable</span>
[<code>initializer()</code>](Initializable-initializer)


---


<div class="funcnameDelegationController contract-index">Events</div>
---
[<code>DelegationProposed(delegationId)</code>](DelegationController-DelegationProposed)
[<code>DelegationAccepted(delegationId)</code>](DelegationController-DelegationAccepted)
[<code>DelegationRequestCanceledByUser(delegationId)</code>](DelegationController-DelegationRequestCanceledByUser)
[<code>UndelegationRequested(delegationId)</code>](DelegationController-UndelegationRequested)

<span class="inherited-title">ILocker</span>

<span class="inherited-title">Permissions</span>

<span class="inherited-title">OwnableUpgradeSafe</span>
[<code>OwnershipTransferred(previousOwner, newOwner)</code>](OwnableUpgradeSafe-OwnershipTransferred)

<span class="inherited-title">ContextUpgradeSafe</span>

<span class="inherited-title">Initializable</span>

---


---

## Modifiers


<div class="funcnamecheckDelegationExists contract-item">
    <h4 id="hfuncnamecheckDelegationExists">
        <a class="anchor" href="#funcnamecheckDelegationExists"></a>
        <code>checkDelegationExists(uint256 delegationId)</code>
        <span class="item-kind">modifier</span>
    </h4>
    <div class="description">
        
        
         <p> Modifier to make a function callable only if delegation exists. </p>
    </div>
</div>



## Functions


- [getAndUpdateDelegatedToValidatorNow(validatorId)](#getAndUpdateDelegatedToValidatorNow)
- [getAndUpdateDelegatedAmount(holder)](#getAndUpdateDelegatedAmount)
- [getAndUpdateEffectiveDelegatedByHolderToValidator(holder, validatorId, month)](#getAndUpdateEffectiveDelegatedByHolderToValidator)
- [delegate(validatorId, amount, delegationPeriod, info)](#delegate)
- [getAndUpdateLockedAmount(wallet)](#getAndUpdateLockedAmount)
- [getAndUpdateForbiddenForDelegationAmount(wallet)](#getAndUpdateForbiddenForDelegationAmount)
- [cancelPendingDelegation(delegationId)](#cancelPendingDelegation)
- [acceptPendingDelegation(delegationId)](#acceptPendingDelegation)
- [requestUndelegation(delegationId)](#requestUndelegation)
- [confiscate(validatorId, amount)](#confiscate)
- [getAndUpdateEffectiveDelegatedToValidator(validatorId, month)](#getAndUpdateEffectiveDelegatedToValidator)
- [getDelegation(delegationId)](#getDelegation)
- [getFirstDelegationMonth(holder, validatorId)](#getFirstDelegationMonth)
- [getDelegationsByValidatorLength(validatorId)](#getDelegationsByValidatorLength)
- [getDelegationsByHolderLength(holder)](#getDelegationsByHolderLength)
- [initialize(_contractsAddress)](#initialize)
- [getAndUpdateDelegatedToValidator(validatorId, month)](#getAndUpdateDelegatedToValidator)
- [processSlashes(holder, limit)](#processSlashes)
- [processAllSlashes(holder)](#processAllSlashes)
- [getState(delegationId)](#getState)
- [getLockedInPendingDelegations(holder)](#getLockedInPendingDelegations)
- [hasUnprocessedSlashes(holder)](#hasUnprocessedSlashes)
- [_addDelegation(holder, validatorId, amount, delegationPeriod, info)](#_addDelegation)
- [_isTerminated(state)](#_isTerminated)
- [_isLocked(state)](#_isLocked)
- [_isDelegated(state)](#_isDelegated)
- [_calculateDelegationEndMonth(delegationId)](#_calculateDelegationEndMonth)
- [_addToDelegatedToValidator(validatorId, amount, month)](#_addToDelegatedToValidator)
- [_addToEffectiveDelegatedToValidator(validatorId, effectiveAmount, month)](#_addToEffectiveDelegatedToValidator)
- [_addToDelegatedByHolder(holder, amount, month)](#_addToDelegatedByHolder)
- [_addToDelegatedByHolderToValidator(holder, validatorId, amount, month)](#_addToDelegatedByHolderToValidator)
- [_removeFromDelegatedByHolder(holder, amount, month)](#_removeFromDelegatedByHolder)
- [_removeFromDelegatedByHolderToValidator(holder, validatorId, amount, month)](#_removeFromDelegatedByHolderToValidator)
- [_addToEffectiveDelegatedByHolderToValidator(holder, validatorId, effectiveAmount, month)](#_addToEffectiveDelegatedByHolderToValidator)
- [_removeFromEffectiveDelegatedByHolderToValidator(holder, validatorId, effectiveAmount, month)](#_removeFromEffectiveDelegatedByHolderToValidator)
- [_getAndUpdateDelegatedByHolder(holder)](#_getAndUpdateDelegatedByHolder)
- [_getAndUpdateDelegatedByHolderToValidator(holder, validatorId, month)](#_getAndUpdateDelegatedByHolderToValidator)
- [_addToLockedInPendingDelegations(holder, amount)](#_addToLockedInPendingDelegations)
- [_subtractFromLockedInPendingDelegations(holder, amount)](#_subtractFromLockedInPendingDelegations)
- [_getCurrentMonth()](#_getCurrentMonth)
- [_getAndUpdateLockedAmount(wallet)](#_getAndUpdateLockedAmount)
- [_updateFirstDelegationMonth(holder, validatorId, month)](#_updateFirstDelegationMonth)
- [_everDelegated(holder)](#_everDelegated)
- [_removeFromDelegatedToValidator(validatorId, amount, month)](#_removeFromDelegatedToValidator)
- [_removeFromEffectiveDelegatedToValidator(validatorId, effectiveAmount, month)](#_removeFromEffectiveDelegatedToValidator)
- [_calculateDelegationAmountAfterSlashing(delegationId)](#_calculateDelegationAmountAfterSlashing)
- [_putToSlashingLog(log, coefficient, month)](#_putToSlashingLog)
- [_processSlashesWithoutSignals(holder, limit)](#_processSlashesWithoutSignals)
- [_processAllSlashesWithoutSignals(holder)](#_processAllSlashesWithoutSignals)
- [_sendSlashingSignals(slashingSignals)](#_sendSlashingSignals)
- [_addToAllStatistics(delegationId)](#_addToAllStatistics)
---






## Modifiers


    ### checkDelegationExists(delegationId)

---



<div class="funcnamegetAndUpdateDelegatedToValidatorNow contract-item">
<h4 id="hfuncnamegetAndUpdateDelegatedToValidatorNow"><a class="anchor" href="#funcnamegetAndUpdateDelegatedToValidatorNow"></a>
<code>getAndUpdateDelegatedToValidatorNow(uint256 validatorId) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetAndUpdateDelegatedAmount contract-item">
<h4 id="hfuncnamegetAndUpdateDelegatedAmount"><a class="anchor" href="#funcnamegetAndUpdateDelegatedAmount"></a>
<code>getAndUpdateDelegatedAmount(address holder) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetAndUpdateEffectiveDelegatedByHolderToValidator contract-item">
<h4 id="hfuncnamegetAndUpdateEffectiveDelegatedByHolderToValidator"><a class="anchor" href="#funcnamegetAndUpdateEffectiveDelegatedByHolderToValidator"></a>
<code>getAndUpdateEffectiveDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 month) <span class="var-type"> → uint256 effectiveDelegated</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamedelegate contract-item">
<h4 id="hfuncnamedelegate"><a class="anchor" href="#funcnamedelegate"></a>
<code>delegate(uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> Allows a token holder to create a delegation proposal of an `amount`
and `delegationPeriod` to a `validatorId`. Delegation must be accepted
by the validator before the UTC start of the month, otherwise the
delegation will be rejected.

The token holder may add additional information in each proposal.

 </p>
</div>

</div>

<div class="funcnamegetAndUpdateLockedAmount contract-item">
<h4 id="hfuncnamegetAndUpdateLockedAmount"><a class="anchor" href="#funcnamegetAndUpdateLockedAmount"></a>
<code>getAndUpdateLockedAmount(address wallet) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> See {ILocker}. </p>
</div>

</div>

<div class="funcnamegetAndUpdateForbiddenForDelegationAmount contract-item">
<h4 id="hfuncnamegetAndUpdateForbiddenForDelegationAmount"><a class="anchor" href="#funcnamegetAndUpdateForbiddenForDelegationAmount"></a>
<code>getAndUpdateForbiddenForDelegationAmount(address wallet) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> See {ILocker}. </p>
</div>

</div>

<div class="funcnamecancelPendingDelegation contract-item">
<h4 id="hfuncnamecancelPendingDelegation"><a class="anchor" href="#funcnamecancelPendingDelegation"></a>
<code>cancelPendingDelegation(uint256 delegationId) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> Allows a token holder to cancel a delegation proposal.

Requirements:

- the sender must be the token holder of the delegation proposal.
- the delegation must still be in a PROPOSED state.

Emits a [DelegationRequestCanceledByUser](DelegationRequestCanceledByUser) event.

 </p>
</div>

</div>

<div class="funcnameacceptPendingDelegation contract-item">
<h4 id="hfuncnameacceptPendingDelegation"><a class="anchor" href="#funcnameacceptPendingDelegation"></a>
<code>acceptPendingDelegation(uint256 delegationId) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> Allows a validator to accept a proposed delegation.
Successful acceptance of delegations then transition the tokens from a
PROPOSED state to ACCEPTED, and tokens are locked for the remainder of the
delegation period.

Emits a {DelegationAccepted} event.

 </p>
</div>

</div>

<div class="funcnamerequestUndelegation contract-item">
<h4 id="hfuncnamerequestUndelegation"><a class="anchor" href="#funcnamerequestUndelegation"></a>
<code>requestUndelegation(uint256 delegationId) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> Allows a delegator to undelegate a specific delegation.

Requirements:

- the sender must be the delegator.
- the delegation must be in DELEGATED state.

Emits an {UndelegationRequested} event.

 </p>
</div>

</div>

<div class="funcnameconfiscate contract-item">
<h4 id="hfuncnameconfiscate"><a class="anchor" href="#funcnameconfiscate"></a>
<code>confiscate(uint256 validatorId, uint256 amount) <span class="var-type"></span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">


 <p> Allows the Punisher to confiscate an `amount` of stake from 
`validatorId` by slashing. This slashes all delegations of the validator,
which reduces the amount that the validator has staked. This consequence 
may force the SKALE Manger to reduce the number of nodes a validator is 
operating so the validator can meet the Minimum Staking Requirement.

See {Punisher}.

Emits a {SlashingEvent}.

 </p>
</div>

</div>

<div class="funcnamegetAndUpdateEffectiveDelegatedToValidator contract-item">
<h4 id="hfuncnamegetAndUpdateEffectiveDelegatedToValidator"><a class="anchor" href="#funcnamegetAndUpdateEffectiveDelegatedToValidator"></a>
<code>getAndUpdateEffectiveDelegatedToValidator(uint256 validatorId, uint256 month) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetDelegation contract-item">
<h4 id="hfuncnamegetDelegation"><a class="anchor" href="#funcnamegetDelegation"></a>
<code>getDelegation(uint256 delegationId) <span class="var-type"> → struct DelegationController.Delegation</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetFirstDelegationMonth contract-item">
<h4 id="hfuncnamegetFirstDelegationMonth"><a class="anchor" href="#funcnamegetFirstDelegationMonth"></a>
<code>getFirstDelegationMonth(address holder, uint256 validatorId) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetDelegationsByValidatorLength contract-item">
<h4 id="hfuncnamegetDelegationsByValidatorLength"><a class="anchor" href="#funcnamegetDelegationsByValidatorLength"></a>
<code>getDelegationsByValidatorLength(uint256 validatorId) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetDelegationsByHolderLength contract-item">
<h4 id="hfuncnamegetDelegationsByHolderLength"><a class="anchor" href="#funcnamegetDelegationsByHolderLength"></a>
<code>getDelegationsByHolderLength(address holder) <span class="var-type"> → uint256</span></code>
<span class="item-kind">external</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnameinitialize contract-item">
<h4 id="hfuncnameinitialize"><a class="anchor" href="#funcnameinitialize"></a>
<code>initialize(address _contractsAddress) <span class="var-type"></span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetAndUpdateDelegatedToValidator contract-item">
<h4 id="hfuncnamegetAndUpdateDelegatedToValidator"><a class="anchor" href="#funcnamegetAndUpdateDelegatedToValidator"></a>
<code>getAndUpdateDelegatedToValidator(uint256 validatorId, uint256 month) <span class="var-type"> → uint256</span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnameprocessSlashes contract-item">
<h4 id="hfuncnameprocessSlashes"><a class="anchor" href="#funcnameprocessSlashes"></a>
<code>processSlashes(address holder, uint256 limit) <span class="var-type"></span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnameprocessAllSlashes contract-item">
<h4 id="hfuncnameprocessAllSlashes"><a class="anchor" href="#funcnameprocessAllSlashes"></a>
<code>processAllSlashes(address holder) <span class="var-type"></span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamegetState contract-item">
<h4 id="hfuncnamegetState"><a class="anchor" href="#funcnamegetState"></a>
<code>getState(uint256 delegationId) <span class="var-type"> → enum DelegationController.State state</span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">


 <p> Returns the token state of a given delegation.

 </p>
</div>

</div>

<div class="funcnamegetLockedInPendingDelegations contract-item">
<h4 id="hfuncnamegetLockedInPendingDelegations"><a class="anchor" href="#funcnamegetLockedInPendingDelegations"></a>
<code>getLockedInPendingDelegations(address holder) <span class="var-type"> → uint256</span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcnamehasUnprocessedSlashes contract-item">
<h4 id="hfuncnamehasUnprocessedSlashes"><a class="anchor" href="#funcnamehasUnprocessedSlashes"></a>
<code>hasUnprocessedSlashes(address holder) <span class="var-type"> → bool</span></code>
<span class="item-kind">public</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addDelegation contract-item">
<h4 id="hfuncname_addDelegation"><a class="anchor" href="#funcname_addDelegation"></a>
<code>_addDelegation(address holder, uint256 validatorId, uint256 amount, uint256 delegationPeriod, string info) <span class="var-type"> → uint256 delegationId</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_isTerminated contract-item">
<h4 id="hfuncname_isTerminated"><a class="anchor" href="#funcname_isTerminated"></a>
<code>_isTerminated(enum DelegationController.State state) <span class="var-type"> → bool</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_isLocked contract-item">
<h4 id="hfuncname_isLocked"><a class="anchor" href="#funcname_isLocked"></a>
<code>_isLocked(enum DelegationController.State state) <span class="var-type"> → bool</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_isDelegated contract-item">
<h4 id="hfuncname_isDelegated"><a class="anchor" href="#funcname_isDelegated"></a>
<code>_isDelegated(enum DelegationController.State state) <span class="var-type"> → bool</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_calculateDelegationEndMonth contract-item">
<h4 id="hfuncname_calculateDelegationEndMonth"><a class="anchor" href="#funcname_calculateDelegationEndMonth"></a>
<code>_calculateDelegationEndMonth(uint256 delegationId) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToDelegatedToValidator contract-item">
<h4 id="hfuncname_addToDelegatedToValidator"><a class="anchor" href="#funcname_addToDelegatedToValidator"></a>
<code>_addToDelegatedToValidator(uint256 validatorId, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToEffectiveDelegatedToValidator contract-item">
<h4 id="hfuncname_addToEffectiveDelegatedToValidator"><a class="anchor" href="#funcname_addToEffectiveDelegatedToValidator"></a>
<code>_addToEffectiveDelegatedToValidator(uint256 validatorId, uint256 effectiveAmount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToDelegatedByHolder contract-item">
<h4 id="hfuncname_addToDelegatedByHolder"><a class="anchor" href="#funcname_addToDelegatedByHolder"></a>
<code>_addToDelegatedByHolder(address holder, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToDelegatedByHolderToValidator contract-item">
<h4 id="hfuncname_addToDelegatedByHolderToValidator"><a class="anchor" href="#funcname_addToDelegatedByHolderToValidator"></a>
<code>_addToDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_removeFromDelegatedByHolder contract-item">
<h4 id="hfuncname_removeFromDelegatedByHolder"><a class="anchor" href="#funcname_removeFromDelegatedByHolder"></a>
<code>_removeFromDelegatedByHolder(address holder, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_removeFromDelegatedByHolderToValidator contract-item">
<h4 id="hfuncname_removeFromDelegatedByHolderToValidator"><a class="anchor" href="#funcname_removeFromDelegatedByHolderToValidator"></a>
<code>_removeFromDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToEffectiveDelegatedByHolderToValidator contract-item">
<h4 id="hfuncname_addToEffectiveDelegatedByHolderToValidator"><a class="anchor" href="#funcname_addToEffectiveDelegatedByHolderToValidator"></a>
<code>_addToEffectiveDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 effectiveAmount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_removeFromEffectiveDelegatedByHolderToValidator contract-item">
<h4 id="hfuncname_removeFromEffectiveDelegatedByHolderToValidator"><a class="anchor" href="#funcname_removeFromEffectiveDelegatedByHolderToValidator"></a>
<code>_removeFromEffectiveDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 effectiveAmount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_getAndUpdateDelegatedByHolder contract-item">
<h4 id="hfuncname_getAndUpdateDelegatedByHolder"><a class="anchor" href="#funcname_getAndUpdateDelegatedByHolder"></a>
<code>_getAndUpdateDelegatedByHolder(address holder) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_getAndUpdateDelegatedByHolderToValidator contract-item">
<h4 id="hfuncname_getAndUpdateDelegatedByHolderToValidator"><a class="anchor" href="#funcname_getAndUpdateDelegatedByHolderToValidator"></a>
<code>_getAndUpdateDelegatedByHolderToValidator(address holder, uint256 validatorId, uint256 month) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToLockedInPendingDelegations contract-item">
<h4 id="hfuncname_addToLockedInPendingDelegations"><a class="anchor" href="#funcname_addToLockedInPendingDelegations"></a>
<code>_addToLockedInPendingDelegations(address holder, uint256 amount) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_subtractFromLockedInPendingDelegations contract-item">
<h4 id="hfuncname_subtractFromLockedInPendingDelegations"><a class="anchor" href="#funcname_subtractFromLockedInPendingDelegations"></a>
<code>_subtractFromLockedInPendingDelegations(address holder, uint256 amount) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_getCurrentMonth contract-item">
<h4 id="hfuncname_getCurrentMonth"><a class="anchor" href="#funcname_getCurrentMonth"></a>
<code>_getCurrentMonth() <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_getAndUpdateLockedAmount contract-item">
<h4 id="hfuncname_getAndUpdateLockedAmount"><a class="anchor" href="#funcname_getAndUpdateLockedAmount"></a>
<code>_getAndUpdateLockedAmount(address wallet) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_updateFirstDelegationMonth contract-item">
<h4 id="hfuncname_updateFirstDelegationMonth"><a class="anchor" href="#funcname_updateFirstDelegationMonth"></a>
<code>_updateFirstDelegationMonth(address holder, uint256 validatorId, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_everDelegated contract-item">
<h4 id="hfuncname_everDelegated"><a class="anchor" href="#funcname_everDelegated"></a>
<code>_everDelegated(address holder) <span class="var-type"> → bool</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_removeFromDelegatedToValidator contract-item">
<h4 id="hfuncname_removeFromDelegatedToValidator"><a class="anchor" href="#funcname_removeFromDelegatedToValidator"></a>
<code>_removeFromDelegatedToValidator(uint256 validatorId, uint256 amount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_removeFromEffectiveDelegatedToValidator contract-item">
<h4 id="hfuncname_removeFromEffectiveDelegatedToValidator"><a class="anchor" href="#funcname_removeFromEffectiveDelegatedToValidator"></a>
<code>_removeFromEffectiveDelegatedToValidator(uint256 validatorId, uint256 effectiveAmount, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_calculateDelegationAmountAfterSlashing contract-item">
<h4 id="hfuncname_calculateDelegationAmountAfterSlashing"><a class="anchor" href="#funcname_calculateDelegationAmountAfterSlashing"></a>
<code>_calculateDelegationAmountAfterSlashing(uint256 delegationId) <span class="var-type"> → uint256</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_putToSlashingLog contract-item">
<h4 id="hfuncname_putToSlashingLog"><a class="anchor" href="#funcname_putToSlashingLog"></a>
<code>_putToSlashingLog(struct DelegationController.SlashingLog log, struct FractionUtils.Fraction coefficient, uint256 month) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_processSlashesWithoutSignals contract-item">
<h4 id="hfuncname_processSlashesWithoutSignals"><a class="anchor" href="#funcname_processSlashesWithoutSignals"></a>
<code>_processSlashesWithoutSignals(address holder, uint256 limit) <span class="var-type"> → struct DelegationController.SlashingSignal[] slashingSignals</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_processAllSlashesWithoutSignals contract-item">
<h4 id="hfuncname_processAllSlashesWithoutSignals"><a class="anchor" href="#funcname_processAllSlashesWithoutSignals"></a>
<code>_processAllSlashesWithoutSignals(address holder) <span class="var-type"> → struct DelegationController.SlashingSignal[] slashingSignals</span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_sendSlashingSignals contract-item">
<h4 id="hfuncname_sendSlashingSignals"><a class="anchor" href="#funcname_sendSlashingSignals"></a>
<code>_sendSlashingSignals(struct DelegationController.SlashingSignal[] slashingSignals) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<div class="funcname_addToAllStatistics contract-item">
<h4 id="hfuncname_addToAllStatistics"><a class="anchor" href="#funcname_addToAllStatistics"></a>
<code>_addToAllStatistics(uint256 delegationId) <span class="var-type"></span></code>
<span class="item-kind">internal</span>
</h4>
<div class="description">



</div>

</div>

<style>
    .contract-index {
        color: #6d79e9;
        font-weight: 600;
        text-transform: uppercase;
    }

    .contact-subindex-inherited {
        border-top: solid 1px #cacbcc;
        margin-top: 1.2em;
        padding-top: 0.25em;
        opacity: 0.7;
    }

    .inherited-title {
        float: right;
        color: black;
        margin-top: 0.8em;
        font-size: 0.8em;
        opacity: 0.7;
    }

    .contract-subindex.

    .contract-item {
        border-radius: 3rem;
        border: solid 1px #ddd;
        max-width: 90vw;
        padding: 0;
        margin-top: 1em;
        margin-bottom: 1em;
        word-wrap: break-word;
    }

    .contract-item>* {
        margin-right: 1em;
        margin-left: 1em;
    }

    .contract-item h4 {
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

    .contract-item h4 code {
        color: inherit;
        background-color: transparent;
        padding: 0;
    }

    .contract-item h4 code span.var-type {
        font-weight: 400;
    }

    .contract-item h4::before {
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

    .contract-item h4 .item-kind {
        font-weight: 300;
        opacity: .8;
    }

    .contract-item .description{
        padding: 5px
    }

    .contract-item .box {
        margin: 20px 10px;
        padding: 10px 30px;
        background-color: #EEE;
        border: 1px solid #CCC;
    }
</style>
