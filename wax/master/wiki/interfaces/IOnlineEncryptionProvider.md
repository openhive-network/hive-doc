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

[wasm/lib/detailed/extensions/signatures/index.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/extensions/signatures/index.ts#L53)

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

[wasm/lib/detailed/extensions/signatures/index.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/extensions/signatures/index.ts#L45)
