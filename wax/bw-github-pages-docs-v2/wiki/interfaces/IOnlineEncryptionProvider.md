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

[wasm/lib/detailed/extensions/signatures/index.ts:52](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/extensions/signatures/index.ts#L52)

***

### encryptData()

> **encryptData**(`buffer`, `recipient`): `Promise`\<`string`\>

Encrypts data

#### Parameters

##### buffer

`string`

The string to encrypt.

##### recipient

`string`

The public key of the recipient to encrypt the data for. The recipient should be a valid public key, starting with "STM".

#### Returns

`Promise`\<`string`\>

A string containing the encrypted data.

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/extensions/signatures/index.ts#L44)
