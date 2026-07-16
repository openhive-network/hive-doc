[@hiveio/wax](../globals) / update\_proposal

# Interface: update\_proposal

A user who created the proposal may update it. A user may decrease {daily_pay},
change subject, permlink and {end_date} (using {extensions}).
In order to update the proposal parameters, all parameters should be entered.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/47_update_proposal.md?ref_type=heads

## Properties

### creator

> **creator**: `string`

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:27

***

### daily\_pay

> **daily\_pay**: `undefined` \| [`asset`](./asset)

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:29

***

### extensions

> **extensions**: [`update_proposal_extension`](./update_proposal_extension)[]

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:37

***

### permlink

> **permlink**: `string`

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:35

***

### proposal\_id

> **proposal\_id**: `string`

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:25

***

### subject

> **subject**: `string`

#### Param

#### Defined in

wasm/lib/proto/update\_proposal.ts:33
