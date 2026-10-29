[@hiveio/wax](../globals) / author\_reward

# Interface: author\_reward

Defined in: wasm/lib/proto/author\_reward.ts:13

Related to comment_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is the author portion of comment reward lowered by the rewards distributed towards beneficiaries
(therefore it can be zero).

## See

comment_benefactor_reward_operation

## Properties

### author

> **author**: `string`

Defined in: wasm/lib/proto/author\_reward.ts:15

#### Param

**author**

author of the comment (receiver of hbd_payout, hive_payout, vesting_payout)

***

### curators\_vesting\_payout

> **curators\_vesting\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/author\_reward.ts:31

#### Param

**curators\_vesting\_payout**

(VESTS) curators' portion of comment reward (@see curation_reward_operation)

***

### hbd\_payout

> **hbd\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/author\_reward.ts:19

#### Param

**hbd\_payout**

(HBD) part of reward

***

### hive\_payout

> **hive\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/author\_reward.ts:23

#### Param

**hive\_payout**

(HIVE) part of reward

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

Defined in: wasm/lib/proto/author\_reward.ts:35

#### Param

**payout\_must\_be\_claimed**

true if payouts require use of claim_reward_balance_operation

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/author\_reward.ts:17

#### Param

**permlink**

permlink of the comment

***

### vesting\_payout

> **vesting\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/author\_reward.ts:27

#### Param

**vesting\_payout**

(VESTS) part of reward
