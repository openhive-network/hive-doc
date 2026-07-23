[@hiveio/wax](../globals) / IOnlineEncryptionProvider

# Interface: IOnlineEncryptionProvider

## Methods

### decryptData()

> **decryptData**(`buffer`): `Promise`\<`string`\>

Decrypts data

#### Parameters

##### buffer

`string`

The string to decrypt.

#### Returns

`Promise`\<`string`\>

The decrypted data as a string.

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/6eb6afa1549899990efe840059f15e4a01129384/ts/wasm/lib/detailed/extensions/signatures/index.ts#L54)

***

### encryptData()

> **encryptData**(`buffer`, `recipient`, `nonce`?): `Promise`\<`string`\>

Encrypts data

#### Parameters

##### buffer

The string or binary buffer to encrypt.

`string` | [`TBinaryBuffer`](../type-aliases/TBinaryBuffer)

##### recipient

`string`

The public key of the recipient to encrypt the data for, or its account name - if supported by the signer.

##### nonce?

`number`

optional nonce to be explicitly specified for encryption. If not provided, a random nonce will be generated.

#### Returns

`Promise`\<`string`\>

A string containing the encrypted data.

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/6eb6afa1549899990efe840059f15e4a01129384/ts/wasm/lib/detailed/extensions/signatures/index.ts#L46)
