[@hiveio/wax](../globals) / comment\_reward

# Interface: comment\_reward

Related to comment_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: for informational purposes only, shows summary of comment reward, does not indicate any transfers.

## See

 - curation_reward_operation
 - comment_benefactor_reward_operation
 - author_reward_operation

## Properties

### author

> **author**: `string`

#### Param

author of the comment

#### Defined in

wasm/lib/proto/comment\_reward.ts:16

***

### author\_rewards

> **author\_rewards**: `string`

#### Param

(HIVE satoshi) raw author reward (@see author_reward_operation) [is it needed?]

#### Defined in

wasm/lib/proto/comment\_reward.ts:24

***

### beneficiary\_payout\_value

> **beneficiary\_payout\_value**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) overall beneficiary reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]

#### Defined in

wasm/lib/proto/comment\_reward.ts:34

***

### curator\_payout\_value

> **curator\_payout\_value**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) overall curation reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]

#### Defined in

wasm/lib/proto/comment\_reward.ts:30

***

### payout

> **payout**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) total value of comment reward recalculated to HBD

#### Defined in

wasm/lib/proto/comment\_reward.ts:20

***

### permlink

> **permlink**: `string`

#### Param

permlink of the comment

#### Defined in

wasm/lib/proto/comment\_reward.ts:18

***

### total\_payout\_value

> **total\_payout\_value**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) overall author reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]

#### Defined in

wasm/lib/proto/comment\_reward.ts:26
