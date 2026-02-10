[@hiveio/wax](../globals) / IAuthorityPathEntry

# Interface: IAuthorityPathEntry

Holds data specific to single authority path entry.
Authority paths are created while processing Account authority definitions, which contain entries describing authority details (built over account or direct key).

## Properties

### processedEntry

> **processedEntry**: `string`

Account name or public key specified at given authority entry definition.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L76)

***

### processedRole

> **processedRole**: `string`

Role level (posting/active/owner) specific to processed authority entry.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:80](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L80)

***

### processingStatus

> **processingStatus**: [`TAuthorityEntryProcessingStatus`](../type-aliases/TAuthorityEntryProcessingStatus)

Holds set of gathered information described by [TAuthorityEntryProcessingStatus](../type-aliases/TAuthorityEntryProcessingStatus) type specific to given entry.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:98](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L98)

***

### recursionDepth

> **recursionDepth**: `number`

Current processing nest level (in case of account authority redirection it can be > 1).

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:93](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L93)

***

### threshold

> **threshold**: `number`

A threashold specific to processed authority role definition.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:84](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L84)

***

### visitedEntries

> **visitedEntries**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)[]

Holds entries being visited during traversing redirected account authority definifions.
This structure allows to see all paths entered during authority verification process, i.e. just to simplify debugging or analysis.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:104](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L104)

***

### weight

> **weight**: `number`

A weight specific to processed (account or key) entry definition.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:88](https://gitlab.syncad.com/hive/wax/-/blob/dd21546b2a1482e8fec320162c50aa2b81e41cf0/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L88)
