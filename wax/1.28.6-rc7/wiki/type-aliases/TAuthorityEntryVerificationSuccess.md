[@hiveio/wax](../globals) / TAuthorityEntryVerificationSuccess

# Type Alias: TAuthorityEntryVerificationSuccess

> **TAuthorityEntryVerificationSuccess**: `object`

Determines set of information collected when given authority path entry has been processed successfully.

## Type declaration

### entryAccepted

> **entryAccepted**: `true`

### isOpenAuthority

> **isOpenAuthority**: `boolean`

- true when authority is open
- false when any key in the authority matched (it implies sufficient weight)

## Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/08ce2c91a14b1535982771816b21d4f88e6240c8/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L50)
