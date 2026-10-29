[@hiveio/wax](../globals) / update\_proposal

# Interface: update\_proposal

Defined in: wasm/lib/proto/update\_proposal.ts:23

A user who created the proposal may update it. A user may decrease {daily_pay},
change subject, permlink and {end_date} (using {extensions}).
In order to update the proposal parameters, all parameters should be entered.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/47_update_proposal.md?ref_type=heads

## Properties

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/update\_proposal.ts:27

#### Param

**creator**

***

### daily\_pay

> **daily\_pay**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/update\_proposal.ts:29

#### Param

**daily\_pay**

***

### extensions

> **extensions**: [`update_proposal_extension`](./update_proposal_extension)[]

Defined in: wasm/lib/proto/update\_proposal.ts:37

#### Param

**extensions**

***

### permlink

> **permlink**: `string`

Defined in: wasm/lib/proto/update\_proposal.ts:35

#### Param

**permlinks**

***

### proposal\_id

> **proposal\_id**: `string`

Defined in: wasm/lib/proto/update\_proposal.ts:25

#### Param

**proposal\_id**

***

### subject

> **subject**: `string`

Defined in: wasm/lib/proto/update\_proposal.ts:33

#### Param

**subject**
