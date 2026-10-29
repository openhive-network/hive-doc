[@hiveio/wax](../globals) / IOnlineSignatureProvider

# Interface: IOnlineSignatureProvider

Defined in: [wasm/lib/detailed/extensions/signatures/index.ts:57](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/extensions/signatures/index.ts#L57)

## Methods

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/extensions/signatures/index.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/extensions/signatures/index.ts#L65)

Signs a transaction by signing a digest of the transaction

#### Parameters

##### transaction

[`ISignatureTransaction`](./ISignatureTransaction)

transaction to be signed

#### Returns

`Promise`\<`void`\>

resolves when the wallet finished signing (signature(s) appended internally)
