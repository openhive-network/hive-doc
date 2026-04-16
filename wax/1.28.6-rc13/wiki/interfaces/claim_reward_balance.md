[@hiveio/wax](../globals) / claim\_reward\_balance

# Interface: claim\_reward\_balance

An operation claim_reward_balance_operation is used to transfer previously collected
author and/or curation rewards from sub balance for the reward to regular balances.
Rewards expressed in Hive and HBD are transferred to liquid balances, rewards in HP increase vesting balance.
When claimed, HP rewards are immediately active towards governance voting power (compare with transfer_to_vesting_operation).

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/39_claim_reward_balance.md?ref_type=heads

## Properties

### account

> **account**: `string`

#### Param

Account name.

#### Defined in

wasm/lib/proto/claim\_reward\_balance.ts:16

***

### reward\_hbd

> **reward\_hbd**: `undefined` \| [`asset`](./asset)

#### Param

The amount of HBD reward to be transferred to liquid balance

#### Defined in

wasm/lib/proto/claim\_reward\_balance.ts:22

***

### reward\_hive

> **reward\_hive**: `undefined` \| [`asset`](./asset)

#### Param

The amount of Hive reward to be transferred to liquid balance.

#### Defined in

wasm/lib/proto/claim\_reward\_balance.ts:18

***

### reward\_vests

> **reward\_vests**: `undefined` \| [`asset`](./asset)

#### Param

The amount of HP reward to be transferred to vesting balance.

#### Defined in

wasm/lib/proto/claim\_reward\_balance.ts:26
