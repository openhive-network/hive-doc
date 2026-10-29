[@hiveio/wax](../globals) / ITransaction

# Interface: ITransaction

Defined in: [wasm/lib/detailed/interfaces.ts:498](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L498)

Transaction allows you to push simple operations (as inline objects)
or use dedicated operation factories
(to create more complex operations or multiple blockchain transactions for specific scenarios)
into underlying transaction.
Furthermore, it allows to perform analysis of the transaction
by examining its id (hash),
evaluating the digest to calculate signatures
or extracting public keys involved in the attached signatures.

Example usage:

## Example

**Base transaction usage**

```typescript
const tx = await waxFoundation.createTransaction();

tx.pushOperation({
  vote: {
    voter: "otom",
    author: "c0ff33a",
    permlink: "ewxhnjbj",
    weight: 2200
  }
});
```

## Extends

- [`ITransactionBase`](./ITransactionBase)

## Accessors

### binaryViewMetadata

#### Get Signature

> **get** **binaryViewMetadata**(): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Defined in: [wasm/lib/detailed/interfaces.ts:375](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L375)

Retrieves transaction binary view packed "AST" data (in same form as in the block_log)

##### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`binaryViewMetadata`](./ITransactionBase#binaryviewmetadata)

***

### id

#### Get Signature

> **get** **id**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:293](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L293)

Generates id of the transaction (HF26 serialization form is used).

##### Throws

on any Wax API-related error

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`id`](./ITransactionBase#id)

***

### impactedAccounts

#### Get Signature

> **get** **impactedAccounts**(): `Set`\<`string`\>

Defined in: [wasm/lib/detailed/interfaces.ts:284](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L284)

Retrieves the set of account names (not authorities!) that are impacted by a whole transaction.

If you want to list impacted accounts per operation, use [IWaxBaseInterface.operationGetImpactedAccounts](./IWaxBaseInterface#operationgetimpactedaccounts) instead.

##### Throws

on any Wax WASM-related error

##### Returns

`Set`\<`string`\>

A set containing the account names that are impacted by the current transaction

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`impactedAccounts`](./ITransactionBase#impactedaccounts)

***

### legacy\_binaryViewMetadata

#### Get Signature

> **get** **legacy\_binaryViewMetadata**(): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Defined in: [wasm/lib/detailed/interfaces.ts:384](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L384)

Retrieves transaction binary view packed "AST" data (in same form as in the block_log) (legacy serialization form is used).

##### Deprecated

##### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_binaryViewMetadata`](./ITransactionBase#legacy_binaryviewmetadata)

***

### legacy\_id

#### Get Signature

> **get** **legacy\_id**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:304](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L304)

Generates id of the transaction (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_id`](./ITransactionBase#legacy_id)

***

### legacy\_sigDigest

#### Get Signature

> **get** **legacy\_sigDigest**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:273](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L273)

Generates digest of the transaction for signing (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_sigDigest`](./ITransactionBase#legacy_sigdigest)

***

### legacy\_signatureKeys

#### Get Signature

> **get** **legacy\_signatureKeys**(): `string`[]

Defined in: [wasm/lib/detailed/interfaces.ts:342](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L342)

Returns signature keys from the transaction signatures (legacy serialization form is used).

##### Throws

on any Wax API-related error

##### Deprecated

##### Returns

`string`[]

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`legacy_signatureKeys`](./ITransactionBase#legacy_signaturekeys)

***

### requiredAuthorities

#### Get Signature

> **get** **requiredAuthorities**(): [`TTransactionRequiredAuthorities`](../type-aliases/TTransactionRequiredAuthorities)

Defined in: [wasm/lib/detailed/interfaces.ts:361](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L361)

Returns required authority accounts from the transaction

##### Throws

on any Wax API-related error

##### Returns

[`TTransactionRequiredAuthorities`](../type-aliases/TTransactionRequiredAuthorities)

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`requiredAuthorities`](./ITransactionBase#requiredauthorities)

***

### sigDigest

#### Get Signature

> **get** **sigDigest**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:192](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L192)

Generates digest of the transaction for signing (HF26 serialization form is used).

##### Throws

on any Wax API-related error

##### Returns

`string`

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`sigDigest`](./ITransactionBase#sigdigest)

***

### signatureKeys

#### Get Signature

> **get** **signatureKeys**(): `string`[]

Defined in: [wasm/lib/detailed/interfaces.ts:331](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L331)

Returns signature keys from the transaction signatures

##### Throws

on any Wax API-related error

##### Returns

`string`[]

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`signatureKeys`](./ITransactionBase#signaturekeys)

***

### transaction

#### Get Signature

> **get** **transaction**(): [`transaction`](./transaction)

Defined in: [wasm/lib/detailed/interfaces.ts:390](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L390)

Fills up constructed transaction object basing on preconfigured TAPOS. Also applies the transaction expiration time.

##### Returns

[`transaction`](./transaction)

protobuf transaction object

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`transaction`](./ITransactionBase#transaction)

## Methods

### addSignature()

> **addSignature**(`signature`): `this`

Defined in: [wasm/lib/detailed/interfaces.ts:209](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L209)

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

***

### decrypt()

> **decrypt**(`provider`): `Promise`\<[`transaction`](./transaction)\>

Defined in: [wasm/lib/detailed/interfaces.ts:353](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L353)

Decrypts all underlying encrypted operations

#### Parameters

##### provider

[`IOnlineEncryptionProvider`](./IOnlineEncryptionProvider)

unlocked wallet to be used for decryption

#### Returns

`Promise`\<[`transaction`](./transaction)\>

protobuf transaction object

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`decrypt`](./ITransactionBase#decrypt)

***

### isSigned()

> **isSigned**(): `boolean`

Defined in: [wasm/lib/detailed/interfaces.ts:250](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L250)

Checks if underlying transaction has been already signed at least one time (after ITransaction.sign)

#### Returns

`boolean`

either true or false based on the signatures amount

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`isSigned`](./ITransactionBase#issigned)

***

### performOperationEncryption()

> **performOperationEncryption**(`provider`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/interfaces.ts:322](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L322)

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

***

### pushOperation()

> **pushOperation**(`op`): `this`

Defined in: [wasm/lib/detailed/interfaces.ts:470](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L470)

Pushes given operation to the operations array in the transaction
This can also add **multiple** operations to the transaction using a straightforward complex operation interface.

We provide a standard set of factories with our implementation, but you can also create custom factories by extending the [OperationBase](../classes/OperationBase) class.

#### Parameters

##### op

[`operation`](./operation) \| [`OperationBase`](../classes/OperationBase)

operation to append to the transaction (can be hive apps operation)
or Class instance for a complex operation that will produce operations including given params

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

**Building blog post**

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

**Building recurrent transfer with pair id and automatically generated removal**

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

***

### startEncrypt()

> **startEncrypt**(`mainEncryptionKey`, `otherEncryptionKey?`): `ITransaction` & [`IEncryptingTransaction`](./IEncryptingTransaction)\<`ITransaction`\>

Defined in: [wasm/lib/detailed/interfaces.ts:412](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L412)

Starts encryption chain

Remember that in order to encrypt operations with given mainEncryptionKey and optional otherEncryptionKey
you have to import those keys into the wallet passed to the ITransaction.sign method

#### Parameters

##### mainEncryptionKey

`string`

First key to encrypt operations

##### otherEncryptionKey?

`string`

Optional second key to encrypt operations

#### Returns

`ITransaction` & [`IEncryptingTransaction`](./IEncryptingTransaction)\<`ITransaction`\>

current transaction instance

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`startEncrypt`](./ITransactionBase#startencrypt)

***

### toApi()

> **toApi**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:243](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L243)

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

***

### toApiJson()

> **toApiJson**(): [`ApiTransaction`](../type-aliases/ApiTransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:399](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L399)

Converts the created transaction into the Hive API-form JSON

#### Returns

[`ApiTransaction`](../type-aliases/ApiTransaction)

transaction in Hive API-form

#### Throws

on any Wax API-related error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toApiJson`](./ITransactionBase#toapijson)

***

### toBinaryForm()

> **toBinaryForm**(`stripToUnsignedTransaction?`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:419](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L419)

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

***

### ~~toLegacyApi()~~

> **toLegacyApi**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:232](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L232)

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

***

### toString()

> **toString**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:313](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L313)

Converts transaction object into the protobuf JSON string

#### Returns

`string`

protobuf JSON string

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`toString`](./ITransactionBase#tostring)

***

### validate()

> **validate**(): `void`

Defined in: [wasm/lib/detailed/interfaces.ts:368](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L368)

Validates current transaction. Throws on error

#### Returns

`void`

#### Throws

on any Wax API-related error including validation error

#### Inherited from

[`ITransactionBase`](./ITransactionBase).[`validate`](./ITransactionBase#validate)
