[@hiveio/wax](../globals) / ASignatureProvider

# Class: `abstract` ASignatureProvider

Helper class encapsulating transaction signing flow. Derived class must implement signature generation logic.

## Extended by

- [`AEncryptionProvider`](./AEncryptionProvider)

## Implements

- [`IOnlineSignatureProvider`](../interfaces/IOnlineSignatureProvider)

## Constructors

### new ASignatureProvider()

> **new ASignatureProvider**(): [`ASignatureProvider`](./ASignatureProvider)

#### Returns

[`ASignatureProvider`](./ASignatureProvider)

## Methods

### generateSignatures()

> `abstract` `protected` **generateSignatures**(`transaction`): `Promise`\<`string`[]\>

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

#### Returns

`Promise`\<`string`[]\>

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/a9eb358591a30de507c01893e4d42a1e3b370322/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L17)

***

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Signs a transaction by signing a digest of the transaction

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

transaction to be signed

#### Returns

`Promise`\<`void`\>

resolves when the wallet finished signing (signature(s) appended internally)

#### Implementation of

[`IOnlineSignatureProvider`](../interfaces/IOnlineSignatureProvider).[`signTransaction`](../interfaces/IOnlineSignatureProvider#signtransaction)

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/a9eb358591a30de507c01893e4d42a1e3b370322/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L8)
