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

[wasm/lib/detailed/extensions/signatures/index.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/fd756288e9a34740db6a53e19d17ae5e94b49e4a/ts/wasm/lib/detailed/extensions/signatures/index.ts#L64)
