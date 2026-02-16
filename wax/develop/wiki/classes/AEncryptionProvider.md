[@hiveio/wax](../globals) / AEncryptionProvider

# Class: `abstract` AEncryptionProvider

Helper class encapsulating transaction signing and encryption flow. Derived class must implement signature
generation logic like also methods related to data encryption.

## Extends

- [`ASignatureProvider`](./ASignatureProvider)

## Implements

- [`IOnlineEncryptionProvider`](../interfaces/IOnlineEncryptionProvider)

## Constructors

### new AEncryptionProvider()

> **new AEncryptionProvider**(): [`AEncryptionProvider`](./AEncryptionProvider)

#### Returns

[`AEncryptionProvider`](./AEncryptionProvider)

#### Inherited from

[`ASignatureProvider`](./ASignatureProvider).[`constructor`](./ASignatureProvider#constructors)

## Methods

### decryptData()

> `abstract` **decryptData**(`buffer`): `Promise`\<`string`\>

Decrypts data

#### Parameters

##### buffer

`string`

The string to decrypt.

#### Returns

`Promise`\<`string`\>

The decrypted data as a string.

#### Implementation of

[`IOnlineEncryptionProvider`](../interfaces/IOnlineEncryptionProvider).[`decryptData`](../interfaces/IOnlineEncryptionProvider#decryptdata)

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L38)

***

### encryptData()

> `abstract` **encryptData**(`buffer`, `recipient`): `Promise`\<`string`\>

Encrypts data

#### Parameters

##### buffer

The string or binary buffer to encrypt.

`string` | [`TBinaryBuffer`](../type-aliases/TBinaryBuffer)

##### recipient

`string`

The public key of the recipient to encrypt the data for, or its account name - if supported by the signer.

#### Returns

`Promise`\<`string`\>

A string containing the encrypted data.

#### Implementation of

[`IOnlineEncryptionProvider`](../interfaces/IOnlineEncryptionProvider).[`encryptData`](../interfaces/IOnlineEncryptionProvider#encryptdata)

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L35)

***

### generateSignatures()

> `abstract` `protected` **generateSignatures**(`transaction`): `Promise`\<`string`[]\>

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

#### Returns

`Promise`\<`string`[]\>

#### Inherited from

[`ASignatureProvider`](./ASignatureProvider).[`generateSignatures`](./ASignatureProvider#generatesignatures)

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L17)

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

#### Overrides

[`ASignatureProvider`](./ASignatureProvider).[`signTransaction`](./ASignatureProvider#signtransaction)

#### Defined in

[wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L28)
