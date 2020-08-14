# Microtick Proposal 1: Post-Genesis Validator Rewards

**The issue at hand:**

In the lead-up to Microtick’s genesis block, external validators (those not related to Microtick or ShapeShift) were incentivized at a rate of 20,000 TICK per validator. The resulting genesis distribution can be seen here: [https://microtick.com/mainnet-genesis.html](https://microtick.com/mainnet-genesis.html)

Left undefined, however, was how new validators would be incentivized. If Microtick is to meet its goal of achieving maximal consensus security, it’ll require a large and diverse validator set – ideally, something eventually approximating that of the Cosmos Hub.

With that in mind, this proposal entails a three-pronged policy that applies to the next 20 validators that join the network: \
 \
1.) New validators (who are not ShapeShift employees) should be incentivised at the rate of 5,000 TICK. These tokens would come from the remaining supply of 310,002 unallocated TICK. This TICK is held jointly by Microtick and ShapeShift in a multi-sig account. Current TICK supply is shown here: [https://microtick.com/chain-parameters.html](https://microtick.com/chain-parameters.html).

(Note that as with the pre-genesis validators, new validators will need to complete the ShapeShift KYC process.)

2.) In order to facilitate decentralization, ShapeShift employees serving as new validators should receive 1,000 TICK, the number of such validators not to exceed 10 under this proposal. (In other words, no more than 10 ShapeShift employees will be represented in the cohort of the next 20 overall validators).

3.)In order to allay concerns that new validators will simply take their new TICK and leave without helping to secure the network, there will be a six-month "waiting period" before TICK is actually distributed. Specifically, for the first six months of validation - with the validator's initial funding beginning the countdown - the appropriate amount of TICK will be delegated, rather than transferred.

New validators will be funded 1 TICK for their initial account creation, and then delegated the appropriate amount  (4,999 for non-ShapeShift validators; 999 for ShapeShift validators) . After six months, the TICK will be undelegated, and the actual TICK tokens (4,999 for non-ShapeShift validators; 999 for ShapeShift validators) will be sent to the account that was used to create and self-fund the validator initially.

This arguably strikes a good balance between incentivizing new validators, while doing so in a way that’s a.) sustainable, and b.) fair to the pre-genesis validators who took on a higher risk by supporting the zone prior to its launch.

Following the onboarding of 20 new validators, the community will need to decide what to do next, via the governance process. This will allow for adjustments and course corrections depending on future conditions.

**Arguments against:**

Clearly the zone must add validators over time in order to improve its security. However, there is potentially room for discussion around the amount of TICK to be distributed to each new validator.

Additionally, concerns have been raised that some validators could commit to supporting the network, and then simply disappear with their new tokens. This is certainly possible – although it’s worth noting that in those cases the “free riders” would need to delegate their TICK to existing validators (and therefore support the network’s security) in order to profit from their holdings.

**The formal proposal:**

If this vote passes, the following will apply to the next 20 onboarded validators:

1.) New validators who are not ShapeShift employees will be incentivised at the rate of 5,000 TICK. 

2.) ShapeShift employees serving as new validators will receive 1,000 TICK, the number of such validators not to exceed 10 under this proposal.

3.) New validators will be funded 1 TICK for their initial account creation, and then delegated the appropriate amount  (4,999 for non-ShapeShift validators; 999 for ShapeShift validators) . After six months, the TICK will be undelegated, and the actual TICK tokens (4,999 for non-ShapeShift validators; 999 for ShapeShift validators) will be sent to the account that was used to create and self-fund the validator initially.

**Voting Stage**

The next stage in the governance process is the voting stage which lasts 1 week. Votes will be a simple "Yes" or "No" on the proposal. Only staked tokens are eligible to be used for governance voting. The amount of voting power is measured in terms of stake. The number of TICK a person or group has determined how much influence their vote will have on the outcome of a proposal. Voters can also change their vote until the closing period.

**Tallying Stage**

After one week the proposal voting will end and the following condition will be taken into consideration to determine if it passes or not:

Quorum: more than 40% of the total staked tokens at the end of the voting period need to have voted.

Threshold: More than 50% or a majority of the tokens that participated in the vote, have voted "Yes."

If any of these conditions are not met, the deposit associated with the denied proposal will not be refunded. These funds will be sent to the community pool.

Once a parameter change or software upgrade proposal is voted on and passes all conditions it will need to be integrated into a new version of the Microtick network software by validators while the previous working version continues to run. This is signalling that a switch will occur. Once more than 2⁄3 of the validators download this new version and signal they are ready to make the switch the rest of the network will be expected to do the same.