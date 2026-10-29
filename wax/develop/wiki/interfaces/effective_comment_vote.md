[@hiveio/wax](../globals) / effective\_comment\_vote

# Interface: effective\_comment\_vote

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:11

Related to vote_operation.
Generated every time vote is cast for the first time or edited, but only as long as it is effective, that is,
the target comment was not yet cashed out.

## Properties

### author

> **author**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:15

#### Param

**author**

author of comment voted on

***

### pending\_payout

> **pending\_payout**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:25

#### Param

**pending\_payout**

(HBD) estimated reward on target comment; supplemented by AH RocksDB plugin

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:17

#### Param

**permlink**

permlink of comment voted on

***

### rshares

> **rshares**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:21

#### Param

**rshares**

power of the vote

***

### total\_vote\_weight

> **total\_vote\_weight**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:23

#### Param

**total\_vote\_weight**

sum of all vote weights on the target comment in the moment of casting current vote

***

### voter

> **voter**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:13

#### Param

**voter**

account that casts a vote

***

### weight

> **weight**: `string`

Defined in: wasm/lib/proto/effective\_comment\_vote.ts:19

#### Param

**weight**

weight of vote depending on when vote was cast and with what power
