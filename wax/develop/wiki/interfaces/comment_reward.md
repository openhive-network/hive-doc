[@hiveio/wax](../globals) / comment\_reward

# Interface: comment\_reward

Defined in: wasm/lib/proto/comment\_reward.ts:14

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

Defined in: wasm/lib/proto/comment\_reward.ts:16

#### Param

**author**

author of the comment

***

### author\_rewards

> **author\_rewards**: `string`

Defined in: wasm/lib/proto/comment\_reward.ts:24

#### Param

**author\_rewards**

(HIVE satoshi) raw author reward (@see author_reward_operation) [is it needed?]

***

### beneficiary\_payout\_value

> **beneficiary\_payout\_value**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_reward.ts:34

#### Param

**beneficiary\_payout\_value**

(HBD) overall beneficiary reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]

***

### curator\_payout\_value

> **curator\_payout\_value**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_reward.ts:30

#### Param

**curator\_payout\_value**

(HBD) overall curation reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]

***

### payout

> **payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_reward.ts:20

#### Param

**payout**

(HBD) total value of comment reward recalculated to HBD

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/comment\_reward.ts:18

#### Param

**permlink**

permlink of the comment

***

### total\_payout\_value

> **total\_payout\_value**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/comment\_reward.ts:26

#### Param

**total\_payout\_value**

(HBD) overall author reward (from multiple cashouts prior to HF17) recalculated to HBD [is it needed?]
