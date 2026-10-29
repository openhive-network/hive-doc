[@hiveio/wax](../globals) / IVerifyAuthorityTrace

# Interface: IVerifyAuthorityTrace

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:142](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L142)

Holds data produced during authority verification process.

## Properties

### collectedData

> **collectedData**: [`IAuthorityPathTraceData`](./IAuthorityPathTraceData)[]

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L147)

Stores data acquired during authority verification process associated to given public key (decoded from signature). Simplifies matching data to signatures in multiple signature case.

***

### ~~finalAuthorityPath~~

> **finalAuthorityPath**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)[]

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:167](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L167)

Stores data specific to the authority path chosen:
- if verification process has been satisfied, it contains successfull path
- when it failed points last processed path.

#### Deprecated

***

### rootEntries

> **rootEntries**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)[]

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L152)

Holds information specific to the account which signed a transaction.
Each array element can be specific to separate authority & signature needed to satisfy transaction.

***

### ~~rootEntry~~

> **rootEntry**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:159](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L159)

Holds information specific to the account which signed a transaction.
Link to last element of [rootEntries](./#rootentries) array.

#### Deprecated

***

### verificationStatus

> **verificationStatus**: [`TAuthorityEntryProcessingStatus`](../type-aliases/TAuthorityEntryProcessingStatus)

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:171](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L171)

Holds set of gathered information described by [TAuthorityEntryProcessingStatus](../type-aliases/TAuthorityEntryProcessingStatus) type specific to whole authority verification process.
