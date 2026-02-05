[@hiveio/wax](../globals) / IAuthorityPathTraceData

# Interface: IAuthorityPathTraceData

Holds data produced during authority verification process.

## Properties

### finalAuthorityPath

> **finalAuthorityPath**: [`IAuthorityPathEntry`](./IAuthorityPathEntry)

Stores data specific to the authority path chosen:
- if verification process has been satisfied, it contains successfull path
- when it failed points last processed path.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:134](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L134)

***

### matchingSignatures

> **matchingSignatures**: [`IAuthorityTraceSignatureInfo`](./IAuthorityTraceSignatureInfo)[]

Optionally filled when procesed authority path matched to the signatures and its decoded public key.
Can be empty when no matching signature has been found.

#### Defined in

[wasm/lib/detailed/verify\_authority\_trace\_interface.ts:127](https://gitlab.syncad.com/hive/wax/-/blob/da2f35291da85a3882dd223725b24e1a8e00958b/ts/wasm/lib/detailed/verify_authority_trace_interface.ts#L127)
