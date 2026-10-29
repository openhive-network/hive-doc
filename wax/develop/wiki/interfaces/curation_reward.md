[@hiveio/wax](../globals) / curation\_reward

# Interface: curation\_reward

Defined in: wasm/lib/proto/curation\_reward.ts:12

Related to comment_operation and comment_vote_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is a fragment of curators' portion of comment reward depending on share of particular curator in overall
curation power for the comment. Only generated when nonzero.

## Properties

### author

> **author**: `string`

Defined in: wasm/lib/proto/curation\_reward.ts:20

#### Param

**author**

author of curated comment

***

### curator

> **curator**: `string`

Defined in: wasm/lib/proto/curation\_reward.ts:14

#### Param

**curator**

user that curated the comment (receiver of reward)

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

Defined in: wasm/lib/proto/curation\_reward.ts:24

#### Param

**payout\_must\_be\_claimed**

true if payouts require use of claim_reward_balance_operation

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/curation\_reward.ts:22

#### Param

**permlink**

permlink of curated comment

***

### reward

> **reward**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/curation\_reward.ts:16

#### Param

**reward**

(VESTS) curation reward
