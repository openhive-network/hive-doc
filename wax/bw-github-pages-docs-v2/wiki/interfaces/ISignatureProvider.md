[@hiveio/wax](../globals) / ISignatureProvider

# Interface: ISignatureProvider

## Methods

### decryptData()

> **decryptData**(`content`, `key`, `anotherKey`?): `string`

Decrypts given data from a specific entity and returns the decrypted message

#### Parameters

##### content

`string`

Base58 content to be decrypted

##### key

`string`

public key to find the private key in the underlying container and decrypt the data

##### anotherKey?

`string`

other public key to find the private key in the underlying container and decrypt the data (optional - use if the message was encrypted for somebody else)

#### Returns

`string`

decrypted buffer

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/39ccd143761fb683bd6b99ed65ccf3cfe7af2648/ts/wasm/lib/detailed/extensions/signatures/index.ts#L33)

***

### encryptData()

> **encryptData**(`content`, `key`, `anotherKey`?, `nonce`?): `string`

Encrypts given data for a specific entity and returns the encrypted message

#### Parameters

##### content

`string`

Content to be encrypted

##### key

`string`

public key to find the private key in the underlying container and encrypt the data

##### anotherKey?

`string`

other public key to find the private key in the underlying container and encrypt the data (optional - use if the message is to encrypt for somebody else)

##### nonce?

`number`

optional nonce to be explicitly specified for encryption

#### Returns

`string`

base58 encrypted buffer

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:23](https://gitlab.syncad.com/hive/wax/-/blob/39ccd143761fb683bd6b99ed65ccf3cfe7af2648/ts/wasm/lib/detailed/extensions/signatures/index.ts#L23)

***

### signDigest()

> **signDigest**(`publicKey`, `sigDigest`): `string`

Signs a transaction by signing a digest of the transaction

#### Parameters

##### publicKey

`string`

public key in WIF format to match the private key in the underlying container. It will be used to sign the provided data

##### sigDigest

`string`

digest of a transaction in hex format

#### Returns

`string`

signed data in hex format

#### Defined in

[wasm/lib/detailed/extensions/signatures/index.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/39ccd143761fb683bd6b99ed65ccf3cfe7af2648/ts/wasm/lib/detailed/extensions/signatures/index.ts#L12)
