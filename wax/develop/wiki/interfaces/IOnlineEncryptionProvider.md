[@hiveio/wax](../globals) / IOnlineEncryptionProvider

# Interface: IOnlineEncryptionProvider

Defined in: [wasm/lib/detailed/extensions/signatures/index.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/extensions/signatures/index.ts#L37)

## Methods

### decryptData()

> **decryptData**(`buffer`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/extensions/signatures/index.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/extensions/signatures/index.ts#L54)

Decrypts data

#### Parameters

##### buffer

`string`

The string to decrypt.

#### Returns

`Promise`\<`string`\>

The decrypted data as a string.

***

### encryptData()

> **encryptData**(`buffer`, `recipient`, `nonce?`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/extensions/signatures/index.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/extensions/signatures/index.ts#L46)

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
