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

[wasm/lib/detailed/extensions/signatures/index.ts:63](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/extensions/signatures/index.ts#L63)
