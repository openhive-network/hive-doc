[@hiveio/wax](../globals) / comment\_benefactor\_reward

# Interface: comment\_benefactor\_reward

Related to comment_operation and comment_options_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is a fragment of the author portion of comment reward depending on share assigned to benefactor
in comment options (can be zero due to rounding).

## See

author_reward

## Properties

### author

> **author**: `string`

#### Param

author of the comment

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:17

***

### benefactor

> **benefactor**: `string`

#### Param

user assigned to receive share of author reward (receiver of payouts)

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:15

***

### hbd\_payout

> **hbd\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) part of reward

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:21

***

### hive\_payout

> **hive\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) part of reward

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:25

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

#### Param

true if payouts require use of claim_reward_balance_operation

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:33

***

### permlink

> **permlink**: `string`

#### Param

permlink of the comment

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:19

***

### vesting\_payout

> **vesting\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) part of reward

#### Defined in

wasm/lib/proto/comment\_benefactor\_reward.ts:29
