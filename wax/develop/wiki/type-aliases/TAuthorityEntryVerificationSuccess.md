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

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/cf6608b95d72b7ca1e7b50031e8dc670f196e613/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L50)
