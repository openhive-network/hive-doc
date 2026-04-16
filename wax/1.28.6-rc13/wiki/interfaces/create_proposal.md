[@hiveio/wax](../globals) / create\_proposal

# Interface: create\_proposal

There is a Decentralized Hive Fund (DHF) on the Hive.
Users may submit proposals for funding and if the proposal receives enough votes, it will be funded.
In order to create a proposal user should create a post first and then marked it as
a proposal with the operation create_proposal_operation.
User defines when the proposal starts and ends and how many funds need to realize it.
The creating proposal costs 10 HBD and additionally 1 HBD for each day over 60 days. The fee goes back to DHF.
Every hour all active proposals are processed and taking into consideration a current number of votes payments are done.
Accounts can create/remove votes anytime.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/44_create_proposal.md?ref_type=heads

## Properties

### creator

> **creator**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:21

***

### daily\_pay

> **daily\_pay**: `undefined` \| [`asset`](./asset)

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:29

***

### end\_date

> **end\_date**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:27

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:37

***

### permlink

> **permlink**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:35

***

### receiver

> **receiver**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:23

***

### start\_date

> **start\_date**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:25

***

### subject

> **subject**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_proposal.ts:33
