[@hiveio/wax](../globals) / ISignatureTransaction

# Interface: ISignatureTransaction

Defined in: [wasm/lib/detailed/interfaces.ts:199](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L199)

## Extended by

- [`ITransactionBase`](./ITransactionBase)

## Accessors

### sigDigest

#### Get Signature

> **get** **sigDigest**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:207](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L207)

Generates digest of the transaction for signing (HF26 serialization form is used).

##### Throws

on any Wax API-related error

##### Returns

`string`

## Methods

### addSignature()

> **addSignature**(`signature`): `this`

Defined in: [wasm/lib/detailed/interfaces.ts:224](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L224)

Adds your signature to the internal signatures array inside underlying transaction.

#### Parameters

##### signature

`string`

signature to add

#### Returns

`this`

current transaction instance

#### Note

If you do not have a signature, create one using dedicated signature providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-hb-auth`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

***

### isSigned()

> **isSigned**(): `boolean`

Defined in: [wasm/lib/detailed/interfaces.ts:265](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L265)

Checks if underlying transaction has been already signed at least one time (after ITransaction.sign)

#### Returns

`boolean`

either true or false based on the signatures amount

***

### performOperationEncryption()?

> `optional` **performOperationEncryption**(`provider`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/interfaces.ts:274](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L274)

**`Internal`**

Allows to encrypt all operations selected to this process by calls to startEncrypt/stopEncrypt methods.

If you are implementing your transaction class and do not have operations to encrypt, you can leave this method not implemented

 This method should be called only internally by the encryption providers

#### Parameters

##### provider

[`IOnlineEncryptionProvider`](./IOnlineEncryptionProvider)

#### Returns

`Promise`\<`void`\>

***

### toApi()

> **toApi**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:258](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L258)

Converts the created transaction into the Hive API-form string

#### Returns

`string`

transaction in Hive API-form

#### Note

This must always return an L1 API transaction form, as signers do not support any other forms for digest generation.

#### Throws

on any Wax API-related error

***

### ~~toLegacyApi()~~

> **toLegacyApi**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:247](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L247)

Converts the created transaction into the Hive API-legacy form JSON string.

Legacy form differs in few aspects to regular (HF26) one:
- for operations type/value dictionary object is replaced by array tuple, where first item points operation type and second operation body
- asset values are encoded in their legacy form having specified token names after amount values, i.e. 1.000 HIVE

Transaction legacy form (even it has shorter JSON code for the first look) is much more error prone, like also
produces **larger binary serialization output**, what is directly stored in blocks. Binary form is the input for signature generation too.
In general, preferred way of generating transactions is HF-26 form (default in this library).

This method is added only for convenience and better cooperation to other transaction processing tools accepting only this form.

#### Returns

`string`

transaction in Legacy Hive API-form

#### Note

This must always return an L1 API transaction form, as signers do not support any other forms for digest generation.

#### Throws

on any Wax API-related error

#### Deprecated
