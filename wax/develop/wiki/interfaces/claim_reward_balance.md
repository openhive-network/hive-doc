[@hiveio/wax](../globals) / claim\_reward\_balance

# Interface: claim\_reward\_balance

Defined in: wasm/lib/proto/claim\_reward\_balance.ts:14

An operation claim_reward_balance_operation is used to transfer previously collected
author and/or curation rewards from sub balance for the reward to regular balances.
Rewards expressed in Hive and HBD are transferred to liquid balances, rewards in HP increase vesting balance.
When claimed, HP rewards are immediately active towards governance voting power (compare with transfer_to_vesting_operation).

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/39_claim_reward_balance.md?ref_type=heads

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/claim\_reward\_balance.ts:16

#### Param

**account**

Account name.

***

### reward\_hbd

> **reward\_hbd**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/claim\_reward\_balance.ts:22

#### Param

**reward\_hbd**

The amount of HBD reward to be transferred to liquid balance

***

### reward\_hive

> **reward\_hive**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/claim\_reward\_balance.ts:18

#### Param

**reward\_hive**

The amount of Hive reward to be transferred to liquid balance.

***

### reward\_vests

> **reward\_vests**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/claim\_reward\_balance.ts:26

#### Param

**reward\_vests**

The amount of HP reward to be transferred to vesting balance.
