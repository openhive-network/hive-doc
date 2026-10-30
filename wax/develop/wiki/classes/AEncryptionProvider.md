[@hiveio/wax](../globals) / AEncryptionProvider

# Abstract Class: AEncryptionProvider

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L26)

Helper class encapsulating transaction signing and encryption flow. Derived class must implement signature
generation logic like also methods related to data encryption.

## Extends

- [`ASignatureProvider`](./ASignatureProvider)

## Implements

- [`IOnlineEncryptionProvider`](../interfaces/IOnlineEncryptionProvider)

## Constructors

### Constructor

> **new AEncryptionProvider**(): `AEncryptionProvider`

#### Returns

`AEncryptionProvider`

#### Inherited from

[`ASignatureProvider`](./ASignatureProvider).[`constructor`](./ASignatureProvider#constructor)

## Methods

### decryptData()

> `abstract` **decryptData**(`buffer`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L38)

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

***

### encryptData()

> `abstract` **encryptData**(`buffer`, `recipient`, `nonce?`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L35)

Encrypts data

#### Parameters

##### buffer

`string` \| [`TBinaryBuffer`](../type-aliases/TBinaryBuffer)

The string or binary buffer to encrypt.

##### recipient

`string`

The public key of the recipient to encrypt the data for, or its account name - if supported by the signer.

##### nonce?

`number`

optional nonce to be explicitly specified for encryption. If not provided, a random nonce will be generated.

#### Returns

`Promise`\<`string`\>

A string containing the encrypted data.

#### Implementation of

[`IOnlineEncryptionProvider`](../interfaces/IOnlineEncryptionProvider).[`encryptData`](../interfaces/IOnlineEncryptionProvider#encryptdata)

***

### generateSignatures()

> `abstract` `protected` **generateSignatures**(`transaction`): `Promise`\<`string`[]\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L17)

#### Parameters

##### transaction

[`ISignatureTransaction`](../interfaces/ISignatureTransaction)

#### Returns

`Promise`\<`string`[]\>

#### Inherited from

[`ASignatureProvider`](./ASignatureProvider).[`generateSignatures`](./ASignatureProvider#generatesignatures)

***

### signTransaction()

> **signTransaction**(`transaction`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/extensions/signatures/extension\_helpers.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/extensions/signatures/extension_helpers.ts#L28)

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
