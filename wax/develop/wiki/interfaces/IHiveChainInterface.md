[@hiveio/wax](../globals) / IHiveChainInterface

# Interface: IHiveChainInterface

Defined in: [wasm/lib/detailed/interfaces.ts:1212](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1212)

## Extends

- [`IWaxBaseInterface`](./IWaxBaseInterface)

## Properties

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](../type-aliases/TDefaultJsonRpcApi)

Defined in: [wasm/lib/detailed/interfaces.ts:1324](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1324)

***

### ASSETS

> `readonly` **ASSETS**: `Readonly`\<`Record`\<[`EAssetName`](../enumerations/EAssetName), [`NaiAsset`](./NaiAsset)\>\>

Defined in: [wasm/lib/detailed/interfaces.ts:583](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L583)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`ASSETS`](./IWaxBaseInterface#assets)

***

### chainId

> `readonly` **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:593](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L593)

Retrieves the chain id. Defined in the Wax base / chain creator functions

#### Returns

chain id in hex string format

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`chainId`](./IWaxBaseInterface#chainid)

***

### formatter

> `readonly` **formatter**: [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

Defined in: [wasm/lib/detailed/interfaces.ts:585](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L585)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`formatter`](./IWaxBaseInterface#formatter)

***

### restApi

> `readonly` **restApi**: [`TDefaultRestApi`](../type-aliases/TDefaultRestApi)

Defined in: [wasm/lib/detailed/interfaces.ts:1326](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1326)

***

### waxify

> `readonly` **waxify**: (`strings`, ...`args`) => `string`

Defined in: [wasm/lib/detailed/interfaces.ts:586](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L586)

Formats given text based on arguments structure

#### Parameters

##### strings

`TemplateStringsArray`

raw strings

##### args

...`unknown`[]

arguments to be parsed using custom wax formatters

#### Returns

`string`

formatted data

#### Example

**Formatting data**

```typescript
formatter.waxify`Hello, ${"alice"}! My account value is ${naiObject}`
```

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`waxify`](./IWaxBaseInterface#waxify)

## Accessors

### addressPrefix

#### Get Signature

> **get** **addressPrefix**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:600](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L600)

Retrieves the public key address prefix

##### Returns

`string`

public key prefix

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`addressPrefix`](./IWaxBaseInterface#addressprefix)

***

### config

#### Get Signature

> **get** **config**(): [`IChainConfig`](./IChainConfig)

Defined in: [wasm/lib/detailed/interfaces.ts:652](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L652)

Holds the protocol configuration for the current chain

##### Returns

[`IChainConfig`](./IChainConfig)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`config`](./IWaxBaseInterface#config)

***

### endpointUrl

#### Get Signature

> **get** **endpointUrl**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:1267](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1267)

Allows to query for endpoint url used to perform API calls.

##### Returns

`string`

#### Set Signature

> **set** **endpointUrl**(`endpoint`): `void`

Defined in: [wasm/lib/detailed/interfaces.ts:1262](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1262)

Allows to override default endpoint URL used to call RPC APIs initially configured by [IWaxOptionsChain](./IWaxOptionsChain) passed to [createHiveChain](../functions/createHiveChain) builder function.

##### Parameters

###### endpoint

`string`

##### Returns

`void`

## Methods

### broadcast()

> **broadcast**(`transaction`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1221](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1221)

Broadcast transaction to the selected during Wax Chain initialization Hive Node

#### Parameters

##### transaction

[`ApiTransaction`](../type-aliases/ApiTransaction) \| [`ITransaction`](./ITransaction) \| [`IOnlineTransaction`](./IOnlineTransaction)

Transaction object to be broadcasted.
If online-transaction is provided, additionally `performOnChainVerification` method is called.

#### Returns

`Promise`\<`void`\>

#### Throws

on any Wax API-related error

***

### calculateAccountHp()

> **calculateAccountHp**(`vests`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:1011](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1011)

Calculates account HP based on given vests, total vesting fund HIVE and total vesting shares

#### Parameters

##### vests

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund

##### totalVestingShares

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset total shares

#### Returns

[`NaiAsset`](./NaiAsset)

HP in nai form

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateAccountHp`](./IWaxBaseInterface#calculateaccounthp)

***

### calculateCurrentManabarValue()

> **calculateCurrentManabarValue**(`now`, `maxMana`, `currentMana`, `lastUpdateTime`): [`IManabarData`](./IManabarData)

Defined in: [wasm/lib/detailed/interfaces.ts:983](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L983)

Calculates current manabar value for Hive account based on given arguments

#### Parameters

##### now

`number`

head block time. Can be obtained using time property from dynamic global properties

##### maxMana

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

maximum account mana. Should equal post_voting_power.amount from the find_account API call for upvotes.
                                      For downvotes remember to multiply this value by downvote_pool_percent from the dynamic global properties API call.
                                      For rc manabar calculations use max_rc value from the rc_accounts API call.

##### currentMana

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

current account mana. Should equal voting_manabar.current_mana from the find_account API call for upvotes or downvote_manabar.current_mana for downvotes
                                          For rc manabar calculations use rc_manabar value from the rc_accounts API call

##### lastUpdateTime

`number`

last update of the current account mana. Should equal voting_manabar.last_update_time from the find_account API call for upvotes or downvote_manabar.current_mana for downvotes
                               For rc manabar calculations use rc_manabar value from the rc_accounts API call

#### Returns

[`IManabarData`](./IManabarData)

Manabar data

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateCurrentManabarValue`](./IWaxBaseInterface#calculatecurrentmanabarvalue)

***

### calculateCurrentManabarValueForAccount()

> **calculateCurrentManabarValueForAccount**(`account`, `manabarType?`): `Promise`\<[`IManabarData`](./IManabarData)\>

Defined in: [wasm/lib/detailed/interfaces.ts:1312](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1312)

Calculates current manabar value for Hive account based on given arguments

#### Parameters

##### account

`string`

account for which we want to calculate current manabar value

##### manabarType?

[`EManabarType`](../enumerations/EManabarType)

manabar type to calculate (can be upvote, downvote or rc manabar. Defaults to [EManabarType.UPVOTE](../enumerations/EManabarType#upvote))

#### Returns

`Promise`\<[`IManabarData`](./IManabarData)\>

Manabar data

***

### calculateHpApr()

> **calculateHpApr**(`headBlockNum`, `vestingRewardPercent`, `virtualSupply`, `totalVestingFundHive`): `number`

Defined in: [wasm/lib/detailed/interfaces.ts:1034](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1034)

Calculate current HP APR

#### Parameters

##### headBlockNum

`number`

head block number

##### vestingRewardPercent

`number`

vesting reward percent

##### virtualSupply

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

virtual supply

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund HIVE

#### Returns

`number`

HP APR percent with 2 decimals

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateHpApr`](./IWaxBaseInterface#calculatehpapr)

***

### calculateManabarFullRegenerationTime()

> **calculateManabarFullRegenerationTime**(`now`, `maxMana`, `currentMana`, `lastUpdateTime`): `number`

Defined in: [wasm/lib/detailed/interfaces.ts:1000](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1000)

Calculates full regeneration time of the manabar value for Hive account based on given arguments

#### Parameters

##### now

`number`

head block time. Can be obtained using time property from dynamic global properties

##### maxMana

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

maximum account mana. Should equal post_voting_power.amount from the find_account API call for upvotes.
                                      For downvotes remember to multiply this value by downvote_pool_percent from the dynamic global properties API call.
                                      For rc manabar calculations use max_rc value from the rc_accounts API call.

##### currentMana

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

current account mana. Should equal voting_manabar.current_mana from the find_account API call for upvotes or downvote_manabar.current_mana for downvotes
                                          For rc manabar calculations use rc_manabar value from the rc_accounts API call

##### lastUpdateTime

`number`

last update of the current account mana. Should equal voting_manabar.last_update_time from the find_account API call for upvotes or downvote_manabar.current_mana for downvotes
                               For rc manabar calculations use rc_manabar value from the rc_accounts API call

#### Returns

`number`

Full regeneration timestamp (in seconds)

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateManabarFullRegenerationTime`](./IWaxBaseInterface#calculatemanabarfullregenerationtime)

***

### calculateManabarFullRegenerationTimeForAccount()

> **calculateManabarFullRegenerationTimeForAccount**(`account`, `manabarType?`): `Promise`\<`Date`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1322](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1322)

Calculates full regeneration time of the manabar value for Hive account based on given arguments

#### Parameters

##### account

`string`

account for which we want to calculate manabar full regeneration time

##### manabarType?

[`EManabarType`](../enumerations/EManabarType)

manabar type to calculate (can be upvote, downvote or rc manabar. Defaults to [EManabarType.UPVOTE](../enumerations/EManabarType#upvote))

#### Returns

`Promise`\<`Date`\>

Full regeneration time

***

### calculatePublicKey()

> **calculatePublicKey**(`wifPrivateKey`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:915](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L915)

Calculates the public key from a given private key in WIF format

#### Parameters

##### wifPrivateKey

`string`

Private key in WIF format

#### Returns

`string`

Public key in WIF format (including prefix)

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculatePublicKey`](./IWaxBaseInterface#calculatepublickey)

***

### calculateWitnessVotesHp()

> **calculateWitnessVotesHp**(`votes`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:1022](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1022)

Calculates witness votes HP based on given votes (expressed in VESTS), total vesting fund HIVE and total vesting shares

#### Parameters

##### votes

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

power of witness votes (assumed in VESTS asset)

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund

##### totalVestingShares

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset total shares

#### Returns

[`NaiAsset`](./NaiAsset)

HP in nai form

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateWitnessVotesHp`](./IWaxBaseInterface#calculatewitnessvoteshp)

***

### convertRawPrivateKeyToWif()

> **convertRawPrivateKeyToWif**(`rawPrivateKey`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:923](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L923)

Allows to convert raw private key to WIF format.

#### Parameters

##### rawPrivateKey

`string`

32 bytes buffer (64 characters hex string) representing private key secret

#### Returns

`string`

WIF formatted private key

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`convertRawPrivateKeyToWif`](./IWaxBaseInterface#convertrawprivatekeytowif)

***

### convertRawPublicKeyToWif()

> **convertRawPublicKeyToWif**(`rawPublicKey`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:931](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L931)

Allows to convert raw public key to WIF format.

#### Parameters

##### rawPublicKey

`string`

33 or 65 bytes buffer (doubled characters hex string) representing compressed or uncompressed public key data

#### Returns

`string`

WIF formatted public key (including prefix)

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`convertRawPublicKeyToWif`](./IWaxBaseInterface#convertrawpublickeytowif)

***

### convertTransactionFromBinaryForm()

> **convertTransactionFromBinaryForm**(`transaction`): [`ApiTransaction`](../type-aliases/ApiTransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:1101](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1101)

Converts given transaction from HF26 specific binary form to Hive API-form JSON

#### Parameters

##### transaction

`string`

transaction in hexstring

#### Returns

[`ApiTransaction`](../type-aliases/ApiTransaction)

transaction in Hive API-form JSON

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`convertTransactionFromBinaryForm`](./IWaxBaseInterface#converttransactionfrombinaryform)

***

### convertTransactionToBinaryForm()

> **convertTransactionToBinaryForm**(`transaction`, `stripToUnsignedTransaction?`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:1091](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1091)

Converts given transaction from Hive API-form JSON to HF26 specific binary form

#### Parameters

##### transaction

[`ApiTransaction`](../type-aliases/ApiTransaction)

transaction in Hive API-form JSON

##### stripToUnsignedTransaction?

`boolean`

optional flag to strip the transaction to unsigned form (without signature container).
       This form can be useful for external transaction hash calculation.

#### Returns

`string`

transaction in hexstring

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`convertTransactionToBinaryForm`](./IWaxBaseInterface#converttransactiontobinaryform)

***

### createTransaction()

> **createTransaction**(`expirationTime?`): `Promise`\<[`IOnlineTransaction`](./IOnlineTransaction)\>

Defined in: [wasm/lib/detailed/interfaces.ts:1239](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1239)

Allows to start transaction preparing process.

Same as [IWaxBaseInterface.createTransactionWithTaPoS](./IWaxBaseInterface#createtransactionwithtapos), but pulls the reference block data from the remote

#### Parameters

##### expirationTime?

[`TTimestamp`](../type-aliases/TTimestamp)

expiration time for the transaction. Applies upon the ITransaction.sign call or reading [ITransaction.transaction](./ITransactionBase#transaction) property.
                                    Can be either any argument parsable by the Date constructor or relative time in seconds, minutes or hours
                                    (remember maximum expiration time for the transaction in mainnet is 1 hour), e.g.:
                                    `1699550966300` `"2023-11-09T17:29:30.028Z"` `new Date()` `"+10s"` `+30m` `+1h`. Defaults to `+1m`.
                                    Expiration time will be applied when calling any non-push-related method in [ITransaction](./ITransaction)

#### Returns

`Promise`\<[`IOnlineTransaction`](./IOnlineTransaction)\>

ready to use transaction interface allowing to fill transaction with its contents like Hive operations

#### Throws

on any Wax API-related error

#### Throws

on any Hive API-related error

***

### createTransactionFromJson()

> **createTransactionFromJson**(`transactionData`): [`ITransaction`](./ITransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:1052](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1052)

Converts Hive API-form transaction in JSON form to our transaction

#### Parameters

##### transactionData

`string` \| `object` \| [`ApiTransaction`](../type-aliases/ApiTransaction)

transaction data to be converted

#### Returns

[`ITransaction`](./ITransaction)

transaction containing ready to sign transaction (or to convert to protobuf structure using [ITransaction.transaction](./ITransactionBase#transaction) property)

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`createTransactionFromJson`](./IWaxBaseInterface#createtransactionfromjson)

***

### createTransactionFromLegacyJson()

> **createTransactionFromLegacyJson**(`transactionData`): [`ITransaction`](./ITransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:1063](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1063)

Converts Hive API-form transaction in legacy JSON form to our transaction

#### Parameters

##### transactionData

`string` \| `object` \| [`LegacyApiTransaction`](../type-aliases/LegacyApiTransaction)

transaction data to be converted

#### Returns

[`ITransaction`](./ITransaction)

transaction containing ready to sign transaction (or to convert to protobuf structure using [ITransaction.transaction](./ITransactionBase#transaction) property)

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`createTransactionFromLegacyJson`](./IWaxBaseInterface#createtransactionfromlegacyjson)

***

### createTransactionFromProto()

> **createTransactionFromProto**(`protoTransaction`): [`ITransaction`](./ITransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:1041](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1041)

Constructs a new Transaction object with ready protobuf transaction

#### Parameters

##### protoTransaction

[`transaction`](./transaction)

protobuf transaction

#### Returns

[`ITransaction`](./ITransaction)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`createTransactionFromProto`](./IWaxBaseInterface#createtransactionfromproto)

***

### createTransactionWithTaPoS()

> **createTransactionWithTaPoS**(`taposBlockId`, `expirationTime?`): [`ITransaction`](./ITransaction)

Defined in: [wasm/lib/detailed/interfaces.ts:1080](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1080)

Constructs a new Transaction object with given data

#### Parameters

##### taposBlockId

`string`

reference block id (can be head block id) for TaPoS

##### expirationTime?

[`TTimestamp`](../type-aliases/TTimestamp)

expiration time for the transaction. Applies upon the ITransaction.sign call or reading [ITransaction.transaction](./ITransactionBase#transaction) property.
                                   Can be either any argument parsable by the Date constructor or relative time in seconds, minutes or hours
                                   (remember maximum expiration time for the transaction in mainnet is 1 hour), e.g.:
                                   `1699550966300` `"2023-11-09T17:29:30.028Z"` `new Date()` `"+10s"` `+30m` `+1h`.
                                   Expiration time will be applied when calling any non-push-related method in [ITransaction](./ITransaction)

#### Returns

[`ITransaction`](./ITransaction)

ready to use transaction interface allowing to fill transaction with its contents like Hive operations

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`createTransactionWithTaPoS`](./IWaxBaseInterface#createtransactionwithtapos)

***

### ~~decrypt()~~

> **decrypt**(`wallet`, `encrypted`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/interfaces.ts:966](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L966)

Decrypts given data from the encrypted string in `#encrypted` format

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

Wallet with imported encryption keys

##### encrypted

`string`

Content to be decoded

#### Returns

`Promise`\<`string`\>

Decoded content

#### Deprecated

Use dedicated encryption providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`decrypt`](./IWaxBaseInterface#decrypt)

***

### delete()

> **delete**(): `void`

Defined in: [wasm/lib/detailed/interfaces.ts:1107](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1107)

Deletes the created wax proto_protocol instance

#### Returns

`void`

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`delete`](./IWaxBaseInterface#delete)

***

### ~~encrypt()~~

> **encrypt**(`wallet`, `content`, `mainEncryptionKey`, `otherEncryptionKey?`, `nonce?`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/interfaces.ts:950](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L950)

Encrypts given data using two keys and dumps result to the encrypted string in `#encrypted` format

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

Wallet with imported mainEncryptionKey and otherEncryptionKey keys

##### content

`string`

Content to be encoded

##### mainEncryptionKey

`string`

First key to encrypt operations

##### otherEncryptionKey?

`string`

Optional second key to encrypt operations

##### nonce?

`number`

optional nonce to be explicitly specified for encryption

#### Returns

`Promise`\<`string`\>

Encrypted content

#### Deprecated

Use dedicated encryption providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`encrypt`](./IWaxBaseInterface#encrypt)

***

### ~~encryptForAccounts()~~

> **encryptForAccounts**(`wallet`, `content`, `fromAccount`, `toAccount`): `Promise`\<`string`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1257](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1257)

Encrypts given data using memo public keys of two accounts and dumps result to the encrypted string in `#encrypted` format

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

Wallet with imported fromAccount and toAccount memo public keys

##### content

`string`

Content to be encoded

##### fromAccount

`string`

first account to retrieve the memo public key used for encryption

##### toAccount

`string`

second account to retrieve the memo public key used for encryption

#### Returns

`Promise`\<`string`\>

Encrypted content

#### Deprecated

Use dedicated encryption providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

***

### estimateHbdInterest()

> **estimateHbdInterest**(`accountHdbSeconds`, `hbdBalance`, `lastCompoundingDate`, `now`, `interestRate`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:687](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L687)

Allows to estimate HBD interest value based on given parameters

#### Parameters

##### accountHdbSeconds

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

value representing already accumulated HBD (amount of HBD * number of seconds held in savings). Usually received e.g. from `savings_hbd_seconds` field of database_api.find_accounts call.

##### hbdBalance

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

the HBD balance to calculate interest for

##### lastCompoundingDate

[`TTimestamp`](../type-aliases/TTimestamp)

last intererest capitalization date to be taken e.g. from `savings_hbd_seconds_last_update` field of database_api.find_accounts call.

##### now

[`TTimestamp`](../type-aliases/TTimestamp)

current date string or unix timestamp number in seconds. It can be received from `time` field of database_api.get_dynamic_global_properties call.

##### interestRate

`number`

interest rate in percent basis points (0-10000). It can be received from `hbd_interest_rate` field of database_api.get_dynamic_global_properties call.

#### Returns

[`NaiAsset`](./NaiAsset)

estimated interest value in HBD asset

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`estimateHbdInterest`](./IWaxBaseInterface#estimatehbdinterest)

***

### estimateHiveCollateral()

> **estimateHiveCollateral**(`currentMedianHistoryBase`, `currentMedianHistoryQuote`, `currentMinHistoryBase`, `currentMinHistoryQuote`, `hbdAmountToGet`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:675](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L675)

Estimate hive collateral

#### Parameters

##### currentMedianHistoryBase

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Base for Current median price retrieved by `get_feed_history`

##### currentMedianHistoryQuote

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Quote for Current median price retrieved by `get_feed_history`

##### currentMinHistoryBase

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Base for Current minimal price retrieved by `get_feed_history`

##### currentMinHistoryQuote

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

Quote for Current minimal price retrieved by `get_feed_history`

##### hbdAmountToGet

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HBD asset used to get HIVE asset

#### Returns

[`NaiAsset`](./NaiAsset)

value in HIVE asset

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`estimateHiveCollateral`](./IWaxBaseInterface#estimatehivecollateral)

***

### extend()

#### Call Signature

> **extend**\<`YourApi`\>(`extendedHiveApiData`): [`TWaxExtended`](../type-aliases/TWaxExtended)\<`YourApi`, `IHiveChainInterface`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1277](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1277)

Extends hive chain interface with your custom API definitions

##### Type Parameters

###### YourApi

`YourApi`

##### Parameters

###### extendedHiveApiData

`YourApi`

your custom api definitions for use with class-validators and class-transformers

##### Returns

[`TWaxExtended`](../type-aliases/TWaxExtended)\<`YourApi`, `IHiveChainInterface`\>

Wax Hive chain instance containing extended api

#### Call Signature

> **extend**\<`YourApi`\>(): [`TWaxExtended`](../type-aliases/TWaxExtended)\<`YourApi`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1295](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1295)

Extends hive chain interface with your custom API definitions (allows you to call remote endpoints without response validation)

##### Type Parameters

###### YourApi

`YourApi`

##### Returns

[`TWaxExtended`](../type-aliases/TWaxExtended)\<`YourApi`\>

Wax Hive chain instance containing extended api

***

### extendConfig()

> **extendConfig**(`config`): `this`

Defined in: [wasm/lib/detailed/interfaces.ts:1302](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1302)

Extends the current wax Chain instance with your custom options, creating a copy of the current instance with altered config.

#### Parameters

##### config

[`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions)

configuration options to extend

#### Returns

`this`

#### Overrides

[`IWaxBaseInterface`](./IWaxBaseInterface).[`extendConfig`](./IWaxBaseInterface#extendconfig)

***

### extendRest()

> **extendRest**\<`YourRestApi`\>(`extendedHiveRestApiData?`): [`TWaxRestExtended`](../type-aliases/TWaxRestExtended)\<`YourRestApi`, `IHiveChainInterface`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1287](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L1287)

Extends hive chain interface with your custom REST API definitions

#### Type Parameters

##### YourRestApi

`YourRestApi`

#### Parameters

##### extendedHiveRestApiData?

[`TDeepWaxApiRequestPartial`](../type-aliases/TDeepWaxApiRequestPartial)\<`YourRestApi`\>

your custom Rest api definitions for use with class-validators and class-transformers

#### Returns

[`TWaxRestExtended`](../type-aliases/TWaxRestExtended)\<`YourRestApi`, `IHiveChainInterface`\>

Wax Hive chain instance containing extended Rest api

***

### getAsset()

> **getAsset**(`nai`): [`IHiveAssetData`](./IHiveAssetData)

Defined in: [wasm/lib/detailed/interfaces.ts:660](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L660)

Retrieves asset amount and symbol from the api data

#### Parameters

##### nai

[`NaiAsset`](./NaiAsset)

API asset

#### Returns

[`IHiveAssetData`](./IHiveAssetData)

asset data

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`getAsset`](./IWaxBaseInterface#getasset)

***

### getPrivateKeyFromPassword()

> **getPrivateKeyFromPassword**(`account`, `role`, `password`): [`IPrivateKeyData`](./IPrivateKeyData)

Defined in: [wasm/lib/detailed/interfaces.ts:905](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L905)

Derives private key for a given role from so-called Master Password

#### Parameters

##### account

`string`

the name of the account to retrieve key for

##### role

`string`

active | owner | posting | memo

##### password

`string`

the Master Password to derive key from

#### Returns

[`IPrivateKeyData`](./IPrivateKeyData)

Generated private key along with the associated public key in WIF format

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`getPrivateKeyFromPassword`](./IWaxBaseInterface#getprivatekeyfrompassword)

***

### getPublicKeyFromSignature()

> **getPublicKeyFromSignature**(`sigDigest`, `signature`): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:880](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L880)

Retrieves the public key in wif format from the given sig digest and signature in hexadecimal format

#### Parameters

##### sigDigest

`string`

digest data in hexadecimal format

##### signature

`string`

signature in hexadecimal format

#### Returns

`string`

public key used in the signature

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`getPublicKeyFromSignature`](./IWaxBaseInterface#getpublickeyfromsignature)

***

### getVersion()

> **getVersion**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:647](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L647)

Retrieves the bundled package version string

#### Returns

`string`

application version

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`getVersion`](./IWaxBaseInterface#getversion)

***

### ~~hbd()~~

> **hbd**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:811](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L811)

Retrieves HBD in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [hbdCoins](./IWaxBaseInterface#hbdcoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of HBD

#### Returns

[`NaiAsset`](./NaiAsset)

HBD in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Deprecated

Use [hbdSatoshis](./IWaxBaseInterface#hbdsatoshis) or [hbdCoins](./IWaxBaseInterface#hbdcoins) instead

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hbd`](./IWaxBaseInterface#hbd)

***

### hbdCoins()

> **hbdCoins**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:717](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L717)

Retrieves HBD in nai form with given amount

Note: This function works with precision and only accepts JS Double-precision floating-point format (IEEE 754),
which does not support numbers greater than 2^53 - 1 or less than -(2^53 - 1).
If you want to pass large number values, use [hbdSatoshis](./IWaxBaseInterface#hbdsatoshis) instead.

#### Parameters

##### amount

`number`

amount of HBD

#### Returns

[`NaiAsset`](./NaiAsset)

HBD in nai form

#### Example

```ts
Inputs: `1000`, `1000.2`, `1000.300`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hbdCoins`](./IWaxBaseInterface#hbdcoins)

***

### hbdSatoshis()

> **hbdSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:762](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L762)

Retrieves HBD in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [hbdCoins](./IWaxBaseInterface#hbdcoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of HBD

#### Returns

[`NaiAsset`](./NaiAsset)

HBD in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hbdSatoshis`](./IWaxBaseInterface#hbdsatoshis)

***

### hbdToHive()

> **hbdToHive**(`hbd`, `base`, `quote`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:858](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L858)

Converts HBD to HIVE in nai form

#### Parameters

##### hbd

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HBD asset

##### base

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HBD asset price base

##### quote

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset price quote

#### Returns

[`NaiAsset`](./NaiAsset)

HIVE in nai form

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hbdToHive`](./IWaxBaseInterface#hbdtohive)

***

### ~~hive()~~

> **hive**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:794](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L794)

Retrieves HIVE in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [hiveCoins](./IWaxBaseInterface#hivecoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of HIVE

#### Returns

[`NaiAsset`](./NaiAsset)

HIVE in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Deprecated

Use [hiveSatoshis](./IWaxBaseInterface#hivesatoshis) or [hiveCoins](./IWaxBaseInterface#hivecoins) instead

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hive`](./IWaxBaseInterface#hive)

***

### hiveCoins()

> **hiveCoins**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:702](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L702)

Retrieves HIVE in nai form with given amount

Note: This function works with precision and only accepts JS Double-precision floating-point format (IEEE 754),
which does not support numbers greater than 2^53 - 1 or less than -(2^53 - 1).
If you want to pass large number values, use [hiveSatoshis](./IWaxBaseInterface#hivesatoshis) instead.

#### Parameters

##### amount

`number`

amount of HIVE

#### Returns

[`NaiAsset`](./NaiAsset)

HIVE in nai form

#### Example

```ts
Inputs: `1000`, `1000.2`, `1000.300`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hiveCoins`](./IWaxBaseInterface#hivecoins)

***

### hiveSatoshis()

> **hiveSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:747](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L747)

Retrieves HIVE in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [hiveCoins](./IWaxBaseInterface#hivecoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of HIVE

#### Returns

[`NaiAsset`](./NaiAsset)

HIVE in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hiveSatoshis`](./IWaxBaseInterface#hivesatoshis)

***

### hiveToHbd()

> **hiveToHbd**(`amount`, `base`, `quote`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:868](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L868)

Converts given amount of HIVE asset to HBD (nai form)

#### Parameters

##### amount

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset

##### base

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HBD asset price base taken i.e. from database_api.get_current_price_feed call

##### quote

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset price quote taken i.e. from database_api.get_current_price_feed call

#### Returns

[`NaiAsset`](./NaiAsset)

HBD in nai form

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hiveToHbd`](./IWaxBaseInterface#hivetohbd)

***

### hpToVests()

> **hpToVests**(`hive`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:848](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L848)

Converts HP to VESTS in nai form

#### Parameters

##### hive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund

##### totalVestingShares

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset total shares

#### Returns

[`NaiAsset`](./NaiAsset)

VESTS in nai form

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`hpToVests`](./IWaxBaseInterface#hptovests)

***

### isValidAccountName()

> **isValidAccountName**(`name`): `boolean`

Defined in: [wasm/lib/detailed/interfaces.ts:618](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L618)

Check if given account name is valid, which means it follows given rules:
- Names must comply with RFC 1035 grammar
- All letters must be lowercase
- Length is between (inclusive) HIVE_MIN_ACCOUNT_NAME_LENGTH and HIVE_MAX_ACCOUNT_NAME_LENGTH. See: [config](./IWaxBaseInterface#config)

#### Parameters

##### name

`string`

account name to be checked

#### Returns

`boolean`

true if account name is valid, false otherwise

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`isValidAccountName`](./IWaxBaseInterface#isvalidaccountname)

***

### operationBinaryViewMetadata()

> **operationBinaryViewMetadata**(`operation`, `isHf26Serialization?`): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Defined in: [wasm/lib/detailed/interfaces.ts:640](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L640)

Retrieves given operation binary view packed "AST" data (in same form as in the block_log)

#### Parameters

##### operation

[`operation`](./operation) \| [`ApiOperation`](./ApiOperation)

The operation object which could be either a protobuf operation or operation returned from the Hive Nodes API

##### isHf26Serialization?

`boolean`

A flag indicating if serialization should be done in HF26 form or legacy form (defaults to `true` - hf26 type)

#### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`operationBinaryViewMetadata`](./IWaxBaseInterface#operationbinaryviewmetadata)

***

### operationGetImpactedAccounts()

> **operationGetImpactedAccounts**(`operation`): `Set`\<`string`\>

Defined in: [wasm/lib/detailed/interfaces.ts:628](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L628)

Retrieves the set of account names (not authorities!) that are impacted by a given operation.

#### Parameters

##### operation

[`operation`](./operation) \| [`ApiOperation`](./ApiOperation)

The operation object which could be either a protobuf operation or operation returned from the Hive Nodes API

#### Returns

`Set`\<`string`\>

A set containing the account names that are impacted by the given operation.

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`operationGetImpactedAccounts`](./IWaxBaseInterface#operationgetimpactedaccounts)

***

### suggestBrainKey()

> **suggestBrainKey**(): [`IBrainKeyData`](./IBrainKeyData)

Defined in: [wasm/lib/detailed/interfaces.ts:893](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L893)

Suggests a safe brain key to use for creating your account.
Returns a brain key and the corresponding private key and public key.
Brain key is a long passphrase that provides enough entropy to generate cryptographic
keys. This function will suggest a suitably random string that should
be easy to write down (and, with effort, memorize).

#### Returns

[`IBrainKeyData`](./IBrainKeyData)

Brain key data

#### Throws

on any Wax API-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`suggestBrainKey`](./IWaxBaseInterface#suggestbrainkey)

***

### ~~vests()~~

> **vests**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:828](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L828)

Retrieves VESTS in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [vestsCoins](./IWaxBaseInterface#vestscoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of VESTS

#### Returns

[`NaiAsset`](./NaiAsset)

VESTS in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Deprecated

Use [vestsSatoshis](./IWaxBaseInterface#vestssatoshis) or [vestsCoins](./IWaxBaseInterface#vestscoins) instead

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`vests`](./IWaxBaseInterface#vests)

***

### vestsCoins()

> **vestsCoins**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:732](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L732)

Retrieves VESTS in nai form with given amount

Note: This function works with precision and only accepts JS Double-precision floating-point format (IEEE 754),
which does not support numbers greater than 2^53 - 1 or less than -(2^53 - 1).
If you want to pass large number values, use [vestsSatoshis](./IWaxBaseInterface#vestssatoshis) instead.

#### Parameters

##### amount

`number`

amount of VESTS

#### Returns

[`NaiAsset`](./NaiAsset)

VESTS in nai form

#### Example

```ts
Inputs: `1000`, `1000.2`, `1000.300`, `1000.000005`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`vestsCoins`](./IWaxBaseInterface#vestscoins)

***

### vestsSatoshis()

> **vestsSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:777](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L777)

Retrieves VESTS in nai form with given amount

Note: This function only accepts integer values.
If you want to pass fractional number values, use [vestsCoins](./IWaxBaseInterface#vestscoins) instead.
This function copies the input value to the output `amount` property without any conversion - adds just a `nai` id.

#### Parameters

##### amount

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

amount of VESTS

#### Returns

[`NaiAsset`](./NaiAsset)

VESTS in nai form

#### Example

```ts
Input: `10000`, `"10000000000000000"`, `BigInt("10000000000000000")`
```

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`vestsSatoshis`](./IWaxBaseInterface#vestssatoshis)

***

### vestsToHp()

> **vestsToHp**(`vests`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:838](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L838)

Converts VESTS to HP in nai form

#### Parameters

##### vests

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund

##### totalVestingShares

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset total shares

#### Returns

[`NaiAsset`](./NaiAsset)

HP in nai form

#### Throws

on any Wax WASM-related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`vestsToHp`](./IWaxBaseInterface#veststohp)
