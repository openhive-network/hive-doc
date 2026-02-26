[@hiveio/wax](../globals) / IOnlineSignatureProvider

# Interface: IOnlineSignatureProvider

## Methods

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Signs a transaction by signing a digest of the transaction

#### Parameters

##### transaction

[`ITransaction`](./ITransaction)

transaction to be signed

#### Returns

`Promise`\<`void`\>

resolves when the wallet finished signing (signature(s) appended internally)

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/extensions/signatures/index.ts#L64)
