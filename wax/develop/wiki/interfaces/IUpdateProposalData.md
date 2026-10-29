[@hiveio/wax](../globals) / IUpdateProposalData

# Interface: IUpdateProposalData

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:7](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L7)

## Properties

### creator

> **creator**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L15)

The account name of the proposal creator.

***

### dailyPay

> **dailyPay**: [`asset`](./asset)

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L20)

The daily pay of the proposal.
**A user who created the proposal may modify it**.

***

### endDate?

> `optional` **endDate?**: `string` \| `number` \| `Date`

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L35)

The end date of the proposal.
**A user who created the proposal may modify it**.

***

### permlink

> **permlink**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L30)

The permlink of the proposal.
**A user who created the proposal may modify it**.

***

### proposalId

> **proposalId**: `string` \| `number`

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L11)

The identifier of the proposal to be updated.

***

### subject

> **subject**: `string`

Defined in: [wasm/lib/detailed/complex\_operations/update\_proposal.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/update_proposal.ts#L25)

The subject of the proposal.
**A user who created the proposal may modify it**.
