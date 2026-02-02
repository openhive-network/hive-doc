[@hiveio/wax](../globals) / TAuthorityEntryVerificationFailure

# Type Alias: TAuthorityEntryVerificationFailure

> **TAuthorityEntryVerificationFailure**: `object`

Collects information during given authority processing when it was rejected.

## Type declaration

### accountAuthorityCountExceeded

> **accountAuthorityCountExceeded**: `boolean`

true if given path entry processing has been interrupted by crossing total number of processed account redirections

### accountAuthorityPointsMissingAccount

> **accountAuthorityPointsMissingAccount**: `boolean`

true if given path entry points to the account not known by the blockchain

### accountAuthorityProcessingDepthExceeded

> **accountAuthorityProcessingDepthExceeded**: `boolean`

true if given authority processing has been interrupted by crossing recursion limit

### entryAccepted

> **entryAccepted**: `false`

### hasAccountAuthorityCycle

> **hasAccountAuthorityCycle**: `boolean`

true if given path entry created a cycle while processig authority account redirection

### hasInsufficientWeight

> **hasInsufficientWeight**: `boolean`

true when key/account entry matched, but the weight was insufficient

### hasMatchingPublicKey

> **hasMatchingPublicKey**: `boolean`

- true when authority has matching any key, but the weight is insufficient
- false when authority does not contain any matching key

### unrelatedAccountMatchedToPublicKey?

> `optional` **unrelatedAccountMatchedToPublicKey**: [`TAccountName`](./TAccountName)

Will be set to non-null value when given (decoded from signature) public key matched to some account, but it is not associated in any way to required authority account.

## Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/39ccd143761fb683bd6b99ed65ccf3cfe7af2648/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L11)
