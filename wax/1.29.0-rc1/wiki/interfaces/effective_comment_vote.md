[@hiveio/wax](../globals) / effective\_comment\_vote

# Interface: effective\_comment\_vote

Related to vote_operation.
Generated every time vote is cast for the first time or edited, but only as long as it is effective, that is,
the target comment was not yet cashed out.

## Properties

### author

> **author**: `string`

#### Param

author of comment voted on

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:15

***

### pending\_payout

> **pending\_payout**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) estimated reward on target comment; supplemented by AH RocksDB plugin

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:25

***

### permlink

> **permlink**: `string`

#### Param

permlink of comment voted on

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:17

***

### rshares

> **rshares**: `string`

#### Param

power of the vote

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:21

***

### total\_vote\_weight

> **total\_vote\_weight**: `string`

#### Param

sum of all vote weights on the target comment in the moment of casting current vote

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:23

***

### voter

> **voter**: `string`

#### Param

account that casts a vote

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:13

***

### weight

> **weight**: `string`

#### Param

weight of vote depending on when vote was cast and with what power

#### Defined in

wasm/lib/proto/effective\_comment\_vote.ts:19
