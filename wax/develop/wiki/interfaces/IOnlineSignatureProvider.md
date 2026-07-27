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

[wasm/lib/detailed/extensions/signatures/index.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/02d56f12bdde25ea29d8b1c19340e25bb82631db/ts/wasm/lib/detailed/extensions/signatures/index.ts#L65)
