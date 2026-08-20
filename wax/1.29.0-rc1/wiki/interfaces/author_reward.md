[@hiveio/wax](../globals) / author\_reward

# Interface: author\_reward

Related to comment_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is the author portion of comment reward lowered by the rewards distributed towards beneficiaries
(therefore it can be zero).

## See

comment_benefactor_reward_operation

## Properties

### author

> **author**: `string`

#### Param

author of the comment (receiver of hbd_payout, hive_payout, vesting_payout)

#### Defined in

wasm/lib/proto/author\_reward.ts:15

***

### curators\_vesting\_payout

> **curators\_vesting\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) curators' portion of comment reward (@see curation_reward_operation)

#### Defined in

wasm/lib/proto/author\_reward.ts:31

***

### hbd\_payout

> **hbd\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) part of reward

#### Defined in

wasm/lib/proto/author\_reward.ts:19

***

### hive\_payout

> **hive\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) part of reward

#### Defined in

wasm/lib/proto/author\_reward.ts:23

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

#### Param

true if payouts require use of claim_reward_balance_operation

#### Defined in

wasm/lib/proto/author\_reward.ts:35

***

### permlink

> **permlink**: `string`

#### Param

permlink of the comment

#### Defined in

wasm/lib/proto/author\_reward.ts:17

***

### vesting\_payout

> **vesting\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) part of reward

#### Defined in

wasm/lib/proto/author\_reward.ts:27
