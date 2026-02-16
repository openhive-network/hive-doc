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

[wasm/lib/detailed/extensions/signatures/index.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/25b077f1212af270804d5f80de54dc9af4e3c0b0/ts/wasm/lib/detailed/extensions/signatures/index.ts#L53)

***

### encryptData()

> **encryptData**(`buffer`, `recipient`): `Promise`\<`string`\>

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

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/25b077f1212af270804d5f80de54dc9af4e3c0b0/ts/wasm/lib/detailed/extensions/signatures/index.ts#L45)
