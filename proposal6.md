# Microtick Proposal 6: IBC Incentive Allocation

## Purpose

Allocate 10,000.00 TICK from the community pool to add Microtick as a sponsor and as a stakeholder in an Incentivised Test Network on the IBC testnet.

## Description

- BitCanna.io is moving from their BitCore blockchain to Cosmos.
- They are promoting an Incentivized Testnet with some common tasks. One of these tasks is related to IBC.
- They have proposed to collaborate with Microtick to build a test scenario to experiment with connections/paths, send / receive tokens, etc.
- BitCanna will reward participants with their tokens to participants and Microtick as well for this IBC task, each with their respective tokens.

## Benefits

Microtick will get more attention in the Cosmos Ecosystem and BitCanna will provide related marketing, something very needed for Microtick currently.

The funds will be transferred to a multisig account jointly owned by Microtick and Spanish-Node validator operators. Raul from Spanish-Node represents BitCanna for the purpose of this proposal. At the end of the testnet IBC phase, both multisig signers will evaluate and distribute the allocated tokens in line with the results of the IBC competition.

We believe this will be a great way to encourage the use of our testnet and get IBC and relayers moved to a production-ready state. Otherwise, experience has shown that nobody has much interest in participating in a non-incentivised environment.

## Notes

BitCanna and Microtick will promote and coordinate the participation on this Testnet, but both chains remain separate and distinct. In particular, BitCanna has control over the users it admits while Microtick intends to keep participation open.

The multisig account to hold the funds will be:

```
micro1uwp86hhwwglgq0k506w8pdquxjs4j40z64h00s
pubkey: micropub1ytql0csgqgfzd666axrjzq655q6y43w5fz8m7mvk687vrqdx7rk0h2wfe5dq6e2lczsu6j33f5fzd666axrjzquhrlqtsp8633z33drsvma95wrcnq3ysdmjmyhusdm5qf8evnq4v5fmhjtn
```

This account has been generated from the pubkeys from Spanish Node and Microtick's validator accounts and can be validated by anyone using the mtcli tool:

```
$ mtcli query auth account micro1md2qat4zy6uy0r7y5y9y84h8zvu5tymyzp5zm6
  address: micro1md2qat4zy6uy0r7y5y9y84h8zvu5tymyzp5zm6
  public_key: micropub1addwnpepqwt3ls9cqnagc3gck3cxd7j68pufsgjgxaedjt7gxa6qynukfs2k24a8plr
$ mtcli query auth account micro1pjtxlrflsyqtwyqkay3u5rz3flhchnedxkcjgj
  address: micro1pjtxlrflsyqtwyqkay3u5rz3flhchnedxkcjgj
  public_key: micropub1addwnpepqd22qdz2ch2y3raldktdrlxpsxn0pm8m48yu6xsdv40upgwdfgc56ywq8ck
$ mtcli keys add spanishnode --pubkey micropub1addwnpepqwt3ls9cqnagc3gck3cxd7j68pufsgjgxaedjt7gxa6qynukfs2k24a8plr
$ mtcli keys add microtick --pubkey micropub1addwnpepqd22qdz2ch2y3raldktdrlxpsxn0pm8m48yu6xsdv40upgwdfgc56ywq8ck
$ mtcli keys add checkmultisig --multisig microtick,spanishnode --multisig-threshold 2
$ mtcli keys show checkmultisig
  type: multi
  address: micro1uwp86hhwwglgq0k506w8pdquxjs4j40z64h00s
```
