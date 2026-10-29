[@hiveio/wax](../globals) / TAuthorityEntryVerificationFailure

# Type Alias: TAuthorityEntryVerificationFailure

> **TAuthorityEntryVerificationFailure** = `object`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L11)

Collects information during given authority processing when it was rejected.

## Properties

### accountAuthorityCountExceeded

> **accountAuthorityCountExceeded**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L20)

true if given path entry processing has been interrupted by crossing total number of processed account redirections

***

### accountAuthorityPointsMissingAccount

> **accountAuthorityPointsMissingAccount**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:24](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L24)

true if given path entry points to the account not known by the blockchain

***

### accountAuthorityProcessingDepthExceeded

> **accountAuthorityProcessingDepthExceeded**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L16)

true if given authority processing has been interrupted by crossing recursion limit

***

### entryAccepted

> **entryAccepted**: `false`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L12)

***

### hasAccountAuthorityCycle

> **hasAccountAuthorityCycle**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L28)

true if given path entry created a cycle while processig authority account redirection

***

### hasInsufficientWeight

> **hasInsufficientWeight**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L32)

true when key/account entry matched, but the weight was insufficient

***

### hasMatchingPublicKey

> **hasMatchingPublicKey**: `boolean`

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L37)

- true when authority has matching any key, but the weight is insufficient
- false when authority does not contain any matching key

***

### unrelatedAccountMatchedToPublicKey?

> `optional` **unrelatedAccountMatchedToPublicKey?**: [`TAccountName`](./TAccountName)

Defined in: [wasm/lib/detailed/verify\_authority\_trace\_interface.ts:42](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L42)

Will be set to non-null value when given (decoded from signature) public key matched to some account, but it is not associated in any way to required authority account.
