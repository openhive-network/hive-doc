[@hiveio/wax](../globals) / TAuthorityEntryVerificationSuccess

# Type Alias: TAuthorityEntryVerificationSuccess

> **TAuthorityEntryVerificationSuccess** = `object`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L50)

Determines set of information collected when given authority path entry has been processed successfully.

## Properties

### entryAccepted

> **entryAccepted**: `true`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:51](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L51)

***

### isOpenAuthority

> **isOpenAuthority**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:56](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L56)

- true when authority is open
- false when any key in the authority matched (it implies sufficient weight)
