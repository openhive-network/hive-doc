[@hiveio/wax](../globals) / IVerifyAuthorityTrace

# Interface: IVerifyAuthorityTrace

Holds data produced during authority verification process.

## Properties

### collectedData

> **collectedData**: [`IAuthorityPathTraceData`](./IAuthorityPathTraceData)[]

Stores data acquired during authority verification process associated to given public key (decoded from signature). Simplifies matching data to signatures in multiple signature case.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:147](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L147)

***

### ~~finalAuthorityPath~~

> **finalAuthorityPath**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)[]

Stores data specific to the authority path chosen:
- if verification process has been satisfied, it contains successfull path
- when it failed points last processed path.

#### Deprecated

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:167](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L167)

***

### rootEntries

> **rootEntries**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)[]

Holds information specific to the account which signed a transaction.
Each array element can be specific to separate authority & signature needed to satisfy transaction.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L152)

***

### ~~rootEntry~~

> **rootEntry**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)

Holds information specific to the account which signed a transaction.
Link to last element of [rootEntries](./IVerifyAuthorityTrace#rootentries) array.

#### Deprecated

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:159](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L159)

***

### verificationStatus

> **verificationStatus**: [`TAuthorityEntryProcessingStatus`](../type-aliases/TAuthorityEntryProcessingStatus)

Holds set of gathered information described by [TAuthorityEntryProcessingStatus](../type-aliases/TAuthorityEntryProcessingStatus) type specific to whole authority verification process.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:171](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L171)
