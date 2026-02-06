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

[wasm/lib/detailed/extensions/signatures/index.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/99f67a8c04ccce81c4687346434ed0802c9d7d6a/ts/wasm/lib/detailed/extensions/signatures/index.ts#L64)
