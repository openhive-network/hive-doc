[@hiveio/wax](../globals) / IHiveChainInterface

# Interface: IHiveChainInterface

Defined in: [wasm/lib/detailed/interfaces.ts:1242](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1242)

## Extends

- [`IWaxBaseInterface`](./IWaxBaseInterface)

## Properties

### api

> `readonly` **api**: [`TDefaultJsonRpcApi`](../type-aliases/TDefaultJsonRpcApi)

Defined in: [wasm/lib/detailed/interfaces.ts:1363](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1363)

***

### ASSETS

> `readonly` **ASSETS**: `Readonly`\<`Record`\<[`EAssetName`](../enumerations/EAssetName), [`NaiAsset`](./NaiAsset)\>\>

Defined in: [wasm/lib/detailed/interfaces.ts:598](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L598)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`ASSETS`](./IWaxBaseInterface#assets)

***

### chainId

> `readonly` **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:608](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L608)

Retrieves the chain id. Defined in the Wax base / chain creator functions

#### Returns

chain id in hex string format

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`chainId`](./IWaxBaseInterface#chainid)

***

### formatter

> `readonly` **formatter**: [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

Defined in: [wasm/lib/detailed/interfaces.ts:600](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L600)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`formatter`](./IWaxBaseInterface#formatter)

***

### restApi

> `readonly` **restApi**: [`TDefaultRestApi`](../type-aliases/TDefaultRestApi)

Defined in: [wasm/lib/detailed/interfaces.ts:1365](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1365)

***

### waxify

> `readonly` **waxify**: (`strings`, ...`args`) => `string`

Defined in: [wasm/lib/detailed/interfaces.ts:601](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L601)

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

Defined in: [wasm/lib/detailed/interfaces.ts:615](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L615)

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

Defined in: [wasm/lib/detailed/interfaces.ts:667](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L667)

Holds the protocol configuration for the current chain

##### Returns

[`IChainConfig`](./IChainConfig)

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`config`](./IWaxBaseInterface#config)

***

### endpointUrl

#### Get Signature

> **get** **endpointUrl**(): `string`

Defined in: [wasm/lib/detailed/interfaces.ts:1297](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1297)

Allows to query for endpoint url used to perform API calls.

##### Returns

`string`

#### Set Signature

> **set** **endpointUrl**(`endpoint`): `void`

Defined in: [wasm/lib/detailed/interfaces.ts:1292](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1292)

Allows to override default endpoint URL used to call RPC APIs initially configured by [IWaxOptionsChain](./IWaxOptionsChain) passed to [createHiveChain](../functions/createHiveChain) builder function.

##### Parameters

###### endpoint

`string`

##### Returns

`void`

## Methods

### broadcast()

> **broadcast**(`transaction`): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/interfaces.ts:1251](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1251)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1026](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1026)

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

Defined in: [wasm/lib/detailed/interfaces.ts:998](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L998)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1342](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1342)

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

### calculateDelegableHp()

> **calculateDelegableHp**(`account`, `now`, `downvotePoolPercent`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:1041](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1041)

Calculates HP which the account can delegate to another account, following the rules applied by the chain to the delegate_vesting_shares operation:
own VESTS (excluding received delegations) reduced by the already delegated VESTS and the whole remaining power down,
additionally limited by the current upvote and downvote mana of the account.

#### Parameters

##### account

[`TDelegableHpAccountData`](../type-aliases/TDelegableHpAccountData)

account data. Can be obtained using the find_accounts API call

##### now

`number`

head block time (in seconds). Can be obtained using time property from dynamic global properties

##### downvotePoolPercent

`number`

downvote pool percent. Can be obtained using downvote_pool_percent property from dynamic global properties

##### totalVestingFundHive

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

HIVE asset total vesting fund

##### totalVestingShares

[`TNaiAssetSource`](../type-aliases/TNaiAssetSource)

VESTS asset total shares

#### Returns

[`NaiAsset`](./NaiAsset)

delegable HP in nai form (zero when the account cannot delegate anything)

#### Throws

on any Wax WASM related error

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`calculateDelegableHp`](./IWaxBaseInterface#calculatedelegablehp)

***

### calculateDelegableHpForAccount()

> **calculateDelegableHpForAccount**(`account`): `Promise`\<[`NaiAsset`](./NaiAsset)\>

Defined in: [wasm/lib/detailed/interfaces.ts:1361](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1361)

Calculates HP which the given account can delegate to another account (see [IWaxBaseInterface.calculateDelegableHp](./IWaxBaseInterface#calculatedelegablehp))

#### Parameters

##### account

`string`

account for which we want to calculate the delegable HP

#### Returns

`Promise`\<[`NaiAsset`](./NaiAsset)\>

delegable HP in nai form

***

### calculateHpApr()

> **calculateHpApr**(`headBlockNum`, `vestingRewardPercent`, `virtualSupply`, `totalVestingFundHive`): `number`

Defined in: [wasm/lib/detailed/interfaces.ts:1064](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1064)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1015](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1015)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1352](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1352)

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

Defined in: [wasm/lib/detailed/interfaces.ts:930](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L930)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1052](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1052)

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

Defined in: [wasm/lib/detailed/interfaces.ts:938](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L938)

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

Defined in: [wasm/lib/detailed/interfaces.ts:946](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L946)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1131](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1131)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1121](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1121)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1269](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1269)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1082](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1082)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1093](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1093)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1071](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1071)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1110](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1110)

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

Defined in: [wasm/lib/detailed/interfaces.ts:981](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L981)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1137](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1137)

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

Defined in: [wasm/lib/detailed/interfaces.ts:965](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L965)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1287](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1287)

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

Defined in: [wasm/lib/detailed/interfaces.ts:702](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L702)

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

Defined in: [wasm/lib/detailed/interfaces.ts:690](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L690)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1307](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1307)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1325](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1325)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1332](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1332)

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

Defined in: [wasm/lib/detailed/interfaces.ts:1317](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1317)

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

Defined in: [wasm/lib/detailed/interfaces.ts:675](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L675)

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

Defined in: [wasm/lib/detailed/interfaces.ts:920](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L920)

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

Defined in: [wasm/lib/detailed/interfaces.ts:895](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L895)

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

Defined in: [wasm/lib/detailed/interfaces.ts:662](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L662)

Retrieves the bundled package version string

#### Returns

`string`

application version

#### Inherited from

[`IWaxBaseInterface`](./IWaxBaseInterface).[`getVersion`](./IWaxBaseInterface#getversion)

***

### ~~hbd()~~

> **hbd**(`amount`): [`NaiAsset`](./NaiAsset)

Defined in: [wasm/lib/detailed/interfaces.ts:826](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L826)

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

Defined in: [wasm/lib/detailed/interfaces.ts:732](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L732)

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

Defined in: [wasm/lib/detailed/interfaces.ts:777](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L777)

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

Defined in: [wasm/lib/detailed/interfaces.ts:873](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L873)

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

Defined in: [wasm/lib/detailed/interfaces.ts:809](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L809)

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

Defined in: [wasm/lib/detailed/interfaces.ts:717](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L717)

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

Defined in: [wasm/lib/detailed/interfaces.ts:762](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L762)

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

Defined in: [wasm/lib/detailed/interfaces.ts:883](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L883)

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

Defined in: [wasm/lib/detailed/interfaces.ts:863](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L863)

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

Defined in: [wasm/lib/detailed/interfaces.ts:633](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L633)

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

Defined in: [wasm/lib/detailed/interfaces.ts:655](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L655)

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

Defined in: [wasm/lib/detailed/interfaces.ts:643](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L643)

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

Defined in: [wasm/lib/detailed/interfaces.ts:908](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L908)

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

Defined in: [wasm/lib/detailed/interfaces.ts:843](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L843)

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

Defined in: [wasm/lib/detailed/interfaces.ts:747](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L747)

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

Defined in: [wasm/lib/detailed/interfaces.ts:792](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L792)

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

Defined in: [wasm/lib/detailed/interfaces.ts:853](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L853)

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
