[@hiveio/wax](../globals) / comment\_benefactor\_reward

# Interface: comment\_benefactor\_reward

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:13

Related to comment_operation and comment_options_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is a fragment of the author portion of comment reward depending on share assigned to benefactor
in comment options (can be zero due to rounding).

## See

author_reward

## Properties

### author

> **author**: `string`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:17

#### Param

**author**

author of the comment

***

### benefactor

> **benefactor**: `string`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:15

#### Param

**benefactor**

user assigned to receive share of author reward (receiver of payouts)

***

### hbd\_payout

> **hbd\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:21

#### Param

**hbd\_payout**

(HBD) part of reward

***

### hive\_payout

> **hive\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:25

#### Param

**hive\_payout**

(HIVE) part of reward

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:33

#### Param

**payout\_must\_be\_claimed**

true if payouts require use of claim_reward_balance_operation

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:19

#### Param

**permlink**

permlink of the comment

***

### vesting\_payout

> **vesting\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_benefactor\_reward.ts:29

#### Param

**vesting\_payout**

(VESTS) part of reward
