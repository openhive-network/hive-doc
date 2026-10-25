[@hiveio/wax](../globals) / curation\_reward

# Interface: curation\_reward

Related to comment_operation and comment_vote_operation.
Generated during block processing after cashout time passes and comment is eligible for rewards (nonzero reward).
Note: the reward is a fragment of curators' portion of comment reward depending on share of particular curator in overall
curation power for the comment. Only generated when nonzero.

## Properties

### author

> **author**: `string`

#### Param

author of curated comment

#### Defined in

wasm/lib/proto/curation\_reward.ts:20

***

### curator

> **curator**: `string`

#### Param

user that curated the comment (receiver of reward)

#### Defined in

wasm/lib/proto/curation\_reward.ts:14

***

### payout\_must\_be\_claimed

> **payout\_must\_be\_claimed**: `boolean`

#### Param

true if payouts require use of claim_reward_balance_operation

#### Defined in

wasm/lib/proto/curation\_reward.ts:24

***

### permlink

> **permlink**: `string`

#### Param

permlink of curated comment

#### Defined in

wasm/lib/proto/curation\_reward.ts:22

***

### reward

> **reward**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) curation reward

#### Defined in

wasm/lib/proto/curation\_reward.ts:16
