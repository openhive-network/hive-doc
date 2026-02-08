[@hiveio/wax](../globals) / IOnlineTransaction

# Interface: IOnlineTransaction

Extends [ITransaction](./ITransaction) interface by functionality which requires online chain access (i.e. accessing account
authority to prevent private keys leak).

## Extends

- [`ITransactionBase`](./ITransactionBase)

## Accessors

### binaryViewMetadata

#### Get Signature

> **get** **binaryViewMetadata**(): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Retrieves transaction binary view packed "AST" data (in same form as in the block_log)

##### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`binaryViewMetadata`](./ITransactionBase#binaryviewmetadata)

#### Defined in

[wasm/lib/detailed/interfaces.ts:376](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L376)

***

### id

#### Get Signature

> **get** **id**(): `string`

Generates id of the transaction (HF26 serialization form is used).

##### Throws

on any Wax API-related error

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`id`](./ITransactionBase#id)

#### Defined in

[wasm/lib/detailed/interfaces.ts:293](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L293)

***

### impactedAccounts

#### Get Signature

> **get** **impactedAccounts**(): `Set`\<`string`\>

Retrieves the set of account names (not authorities!) that are impacted by a whole transaction.

If you want to list impacted accounts per operation, use [IWaxBaseInterface.operationGetImpactedAccounts](./IWaxBaseInterface#operationgetimpactedaccounts) instead.

##### Throws

on any Wax WASM-related error

##### Returns

`Set`\<`string`\>

A set containing the account names that are impacted by the current transaction

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`impactedAccounts`](./ITransactionBase#impactedaccounts)

#### Defined in

[wasm/lib/detailed/interfaces.ts:284](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L284)

***

### legacy\_binaryViewMetadata

#### Get Signature

> **get** **legacy\_binaryViewMetadata**(): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Retrieves transaction binary view packed "AST" data (in same form as in the block_log) (legacy serialization form is used).

##### Deprecated

##### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_binaryViewMetadata`](./ITransactionBase#legacy_binaryviewmetadata)

#### Defined in

[wasm/lib/detailed/interfaces.ts:385](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L385)

***

### legacy\_id

#### Get Signature

> **get** **legacy\_id**(): `string`

Generates id of the transaction (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_id`](./ITransactionBase#legacy_id)

#### Defined in

[wasm/lib/detailed/interfaces.ts:304](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L304)

***

### legacy\_sigDigest

#### Get Signature

> **get** **legacy\_sigDigest**(): `string`

Generates digest of the transaction for signing (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_sigDigest`](./ITransactionBase#legacy_sigdigest)

#### Defined in

[wasm/lib/detailed/interfaces.ts:273](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L273)

***

### legacy\_signatureKeys

#### Get Signature

> **get** **legacy\_signatureKeys**(): `string`[]

Returns signature keys from the transaction signatures (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`[]

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_signatureKeys`](./ITransactionBase#legacy_signaturekeys)

#### Defined in

[wasm/lib/detailed/interfaces.ts:342](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L342)

***

### requiredAuthorities

#### Get Signature

> **get** **requiredAuthorities**(): [`TTransactionRequiredAuthorities`](../type-aliases/TTransactionRequiredAuthorities)

Returns required authority accounts from the transaction

##### Throws

on any Wax API-related error

##### Returns

[`TTransactionRequiredAuthorities`](../type-aliases/TTransactionRequiredAuthorities)

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`requiredAuthorities`](./ITransactionBase#requiredauthorities)

#### Defined in

[wasm/lib/detailed/interfaces.ts:362](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L362)

***

### sigDigest

#### Get Signature

> **get** **sigDigest**(): `string`

Generates digest of the transaction for signing (HF26 serialization form is used).

##### Throws

on any Wax API-related error

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`sigDigest`](./ITransactionBase#sigdigest)

#### Defined in

[wasm/lib/detailed/interfaces.ts:192](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L192)

***

### signatureKeys

#### Get Signature

> **get** **signatureKeys**(): `string`[]

Returns signature keys from the transaction signatures

##### Throws

on any Wax API-related error

##### Returns

`string`[]

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`signatureKeys`](./ITransactionBase#signaturekeys)

#### Defined in

[wasm/lib/detailed/interfaces.ts:331](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L331)

***

### transaction

#### Get Signature

> **get** **transaction**(): [`transaction`](./transaction)

Fills up constructed transaction object basing on preconfigured TAPOS. Also applies the transaction expiration time.

##### Returns

[`transaction`](./transaction)

protobuf transaction object

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`transaction`](./ITransactionBase#transaction)

#### Defined in

[wasm/lib/detailed/interfaces.ts:391](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L391)

## Methods

### addSignature()

> **addSignature**(`signature`): `this`

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

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`addSignature`](./ITransactionBase#addsignature)

#### Defined in

[wasm/lib/detailed/interfaces.ts:209](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L209)

***

### decrypt()

> **decrypt**(`wallet`): [`transaction`](./transaction)

Decrypts all underlying encrypted operations

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

unlocked wallet to be used for decryption

#### Returns

[`transaction`](./transaction)

protobuf transaction object

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`decrypt`](./ITransactionBase#decrypt)

#### Defined in

[wasm/lib/detailed/interfaces.ts:353](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L353)

***

### generateAuthorityVerificationTrace()

> **generateAuthorityVerificationTrace**(`useLegacySerialization`?, `externalTx`?): `Promise`\<[`IVerifyAuthorityTrace`](./IVerifyAuthorityTrace)\>

Allows to generate authority verification trace for the currently loaded/built transaction.
Transaction should be already signed, otherwise the function throws.
The authority trace process requires online access to the chain APIs to retrieve account data.

#### Parameters

##### useLegacySerialization?

`boolean`

optional flag to force using legacy (pre HF26) serialization mode on processed transaction

##### externalTx?

[`ITransaction`](./ITransaction)

optional external transaction to be used for authority verification trace generation. If omitted, defaults to HF26

#### Returns

`Promise`\<[`IVerifyAuthorityTrace`](./IVerifyAuthorityTrace)\>

#### Defined in

[wasm/lib/detailed/interfaces.ts:585](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L585)

***

### isSigned()

> **isSigned**(): `boolean`

Checks if underlying transaction has been already signed at least one time (after [ITransaction.sign](./ITransactionBase#sign))

#### Returns

`boolean`

either true or false based on the signatures amount

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`isSigned`](./ITransactionBase#issigned)

#### Defined in

[wasm/lib/detailed/interfaces.ts:250](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L250)

***

### performOnChainVerification()

> **performOnChainVerification**(): `Promise`\<`void`\>

Allows to perform transaction checks which require additional access to chain APIs i.e. to retrieve account data.

Supported checks:

- [x] private key leakage prevention
- [ ] new authority definition validation (prevent creation of cycles, extending chain limits specific to authority verification, referencing nonexisting accounts)

#### Returns

`Promise`\<`void`\>

#### Throws

when any of supported checks failed.

#### Defined in

[wasm/lib/detailed/interfaces.ts:575](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L575)

***

### performOperationEncryption()

> **performOperationEncryption**(`provider`): `Promise`\<`void`\>

**`Internal`**

Allows to encrypt all operations selected to this process by calls to startEncrypt/stopEncrypt methods.\

If you are implementing your transaction class and do not have operations to encrypt, you can leave this method empty

 This method should be called only internally by the encryption providers

#### Parameters

##### provider

[`IOnlineEncryptionProvider`](./IOnlineEncryptionProvider)

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`performOperationEncryption`](./ITransactionBase#performoperationencryption)

#### Defined in

[wasm/lib/detailed/interfaces.ts:322](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L322)

***

### pushOperation()

> **pushOperation**(`op`): `this`

Pushes given operation to the operations array in the transaction
This can also add **multiple** operations to the transaction using a straightforward complex operation interface.

We provide a standard set of factories with our implementation, but you can also create custom factories by extending the [OperationBase](../classes/OperationBase) class.

#### Parameters

##### op

operation to append to the transaction (can be hive apps operation)
or Class instance for a complex operation that will produce operations including given params

[`operation`](./operation) | [`OperationBase`](../classes/OperationBase)

#### Returns

`this`

current transaction instance

#### See

 - Complex operations:
 [AccountAuthorityUpdateOperation](../classes/AccountAuthorityUpdateOperation) Creates an account authority update operation
 [BlogPostOperation](../classes/BlogPostOperation) Creates a blog post. It requires the category on blog post to be set,
 [ReplyOperation](../classes/ReplyOperation) Creates a reply to a comment or a blog post. It requires parent author and parent permlink to be set,
 [DefineRecurrentTransferOperation](../classes/DefineRecurrentTransferOperation) Creates or updates a recurrent transfer. It requires the amount to be set and to be non-zero, otherwise the removal will be generated automatically,
 [RecurrentTransferRemovalOperation](../classes/RecurrentTransferRemovalOperation) Creates an operation removing existing recurrent transfer
 [UpdateProposalOperation](../classes/UpdateProposalOperation) Creates an update proposal operation. You can optionally set the end date of the proposal,
 [WitnessSetPropertiesOperation](../classes/WitnessSetPropertiesOperation) Creates a witness set properties operation with automatic data serialization,
 - Hive Apps operations:
 [CommunityOperation](../classes/CommunityOperation) Allows to manipulate the community options,
 [FollowOperation](../classes/FollowOperation) Allows to manipulate the follow options,
 [ResourceCreditsOperation](../classes/ResourceCreditsOperation) Allows to delegate or remove delegation of resource credits to given account(s),

#### Examples

```typescript
 tx.pushOperation(new BlogPostOperation({
   category: "test-category",
   author: "gtg",
   title: "Post with category",
   body: "Post with category",
   permlink: "post-with-category",
   tags: ["spam"],
   description: "Post with category"
 }));
```

```typescript
 tx.pushOperation(new DefineRecurrentTransferOperation({
   from: "initminer",
   to: "gtg",
   pairId: 100
 }));
```

#### Throws

on any Wax API-related error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`pushOperation`](./ITransactionBase#pushoperation)

#### Defined in

[wasm/lib/detailed/interfaces.ts:471](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L471)

***

### ~~sign()~~

> **sign**(`wallet`, `publicKey`): `string`

Signs the transaction using given public key. Applies the transaction expiration time

Encrypts operations if any were created using [IEncryptingTransaction](./IEncryptingTransaction) interface

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

unlocked wallet to be used for signing

##### publicKey

`string`

publicKey for signing (should be available in the wallet)

#### Returns

`string`

transaction signature signed using given key

#### Throws

on any Wax API-related error or no public key found in the unlocked wallet or wallet is locked

#### Deprecated

Use dedicated signature providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-hb-auth`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`sign`](./ITransactionBase#sign)

#### Defined in

[wasm/lib/detailed/interfaces.ts:492](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L492)

***

### startEncrypt()

> **startEncrypt**(`mainEncryptionKey`, `otherEncryptionKey`?): [`IOnlineTransaction`](./IOnlineTransaction) & [`IEncryptingTransaction`](./IEncryptingTransaction)\<[`IOnlineTransaction`](./IOnlineTransaction)\>

Starts encryption chain

Remember that in order to encrypt operations with given mainEncryptionKey and optional otherEncryptionKey
you have to import those keys into the wallet passed to the [ITransaction.sign](./ITransactionBase#sign) method

#### Parameters

##### mainEncryptionKey

`string`

First key to encrypt operations

##### otherEncryptionKey?

`string`

Optional second key to encrypt operations

#### Returns

[`IOnlineTransaction`](./IOnlineTransaction) & [`IEncryptingTransaction`](./IEncryptingTransaction)\<[`IOnlineTransaction`](./IOnlineTransaction)\>

current transaction instance

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`startEncrypt`](./ITransactionBase#startencrypt)

#### Defined in

[wasm/lib/detailed/interfaces.ts:413](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L413)

***

### toApi()

> **toApi**(): `string`

Converts the created transaction into the Hive API-form string

#### Returns

`string`

transaction in Hive API-form

#### Note

This must always return an L1 API transaction form, as signers do not support any other forms for digest generation.

#### Throws

on any Wax API-related error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toApi`](./ITransactionBase#toapi)

#### Defined in

[wasm/lib/detailed/interfaces.ts:243](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L243)

***

### toApiJson()

> **toApiJson**(): [`ApiTransaction`](../type-aliases/ApiTransaction)

Converts the created transaction into the Hive API-form JSON

#### Returns

[`ApiTransaction`](../type-aliases/ApiTransaction)

transaction in Hive API-form

#### Throws

on any Wax API-related error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toApiJson`](./ITransactionBase#toapijson)

#### Defined in

[wasm/lib/detailed/interfaces.ts:400](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L400)

***

### toBinaryForm()

> **toBinaryForm**(`stripToUnsignedTransaction`?): `string`

Allows to serialize underlying transaction to HF26 specific binary form, then return it as hexstring.

#### Parameters

##### stripToUnsignedTransaction?

`boolean`

optional flag to strip the transaction to unsigned form (without signature container).
       This form can be useful for external transaction hash calculation.

#### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toBinaryForm`](./ITransactionBase#tobinaryform)

#### Defined in

[wasm/lib/detailed/interfaces.ts:420](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L420)

***

### ~~toLegacyApi()~~

> **toLegacyApi**(): `string`

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

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toLegacyApi`](./ITransactionBase#tolegacyapi)

#### Defined in

[wasm/lib/detailed/interfaces.ts:232](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L232)

***

### toString()

> **toString**(): `string`

Converts transaction object into the protobuf JSON string

#### Returns

`string`

protobuf JSON string

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toString`](./ITransactionBase#tostring)

#### Defined in

[wasm/lib/detailed/interfaces.ts:313](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L313)

***

### validate()

> **validate**(): `void`

Validates current transaction. Throws on error

#### Returns

`void`

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`validate`](./ITransactionBase#validate)

#### Defined in

[wasm/lib/detailed/interfaces.ts:369](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/interfaces.ts#L369)
