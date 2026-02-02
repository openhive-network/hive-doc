[@hiveio/wax](../globals) / IUpdateProposalData

# Interface: IUpdateProposalData

## Properties

### creator

> **creator**: `string`

The account name of the proposal creator.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L15)

***

### dailyPay

> **dailyPay**: [`asset`](./asset)

The daily pay of the proposal.
**A user who created the proposal may modify it**.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L20)

***

### endDate?

> `optional` **endDate**: `string` \| `number` \| `Date`

The end date of the proposal.
**A user who created the proposal may modify it**.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L35)

***

### permlink

> **permlink**: `string`

The permlink of the proposal.
**A user who created the proposal may modify it**.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L30)

***

### proposalId

> **proposalId**: `string` \| `number`

The identifier of the proposal to be updated.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L11)

***

### subject

> **subject**: `string`

The subject of the proposal.
**A user who created the proposal may modify it**.

#### Defined in

[wasm/lib/detailed/complex\_operations/update\_proposal.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L25)
