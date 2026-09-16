[@hiveio/wax](../globals) / IOnlineSignatureProvider

# Interface: IOnlineSignatureProvider

## Methods

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Signs a transaction by signing a digest of the transaction

#### Parameters

##### transaction

[`ISignatureTransaction`](./ISignatureTransaction)

transaction to be signed

#### Returns

`Promise`\<`void`\>

resolves when the wallet finished signing (signature(s) appended internally)

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/9050d2bb3048b6ba0f5fba8b2adf4032fc2405d4/ts/wasm/lib/detailed/extensions/signatures/index.ts#L65)
