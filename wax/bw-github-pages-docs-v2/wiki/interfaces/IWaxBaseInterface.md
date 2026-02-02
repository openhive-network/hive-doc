[@hiveio/wax](../globals) / IWaxBaseInterface

# Interface: IWaxBaseInterface

## Extended by

- [`IHiveChainInterface`](./IHiveChainInterface)

## Properties

### ASSETS

> `readonly` **ASSETS**: `Readonly`\<`Record`\<[`EAssetName`](../enumerations/EAssetName), [`NaiAsset`](./NaiAsset)\>\>

#### Defined in

[wasm/lib/detailed/interfaces.ts:605](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L605)

***

### chainId

> `readonly` **chainId**: `string`

Retrieves the chain id. Defined in the Wax base / chain creator functions

#### Returns

chain id in hex string format

#### Defined in

[wasm/lib/detailed/interfaces.ts:615](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L615)

***

### formatter

> `readonly` **formatter**: [`IWaxExtendableFormatter`](./IWaxExtendableFormatter)

#### Defined in

[wasm/lib/detailed/interfaces.ts:607](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L607)

***

### waxify()

> `readonly` **waxify**: (`strings`, ...`args`) => `string`

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

```typescript
formatter.waxify`Hello, ${"alice"}! My account value is ${naiObject}`
```

#### Defined in

[wasm/lib/detailed/interfaces.ts:608](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L608)

## Accessors

### addressPrefix

#### Get Signature

> **get** **addressPrefix**(): `string`

Retrieves the public key address prefix

##### Returns

`string`

public key prefix

#### Defined in

[wasm/lib/detailed/interfaces.ts:622](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L622)

***

### config

#### Get Signature

> **get** **config**(): [`IChainConfig`](./IChainConfig)

Holds the protocol configuration for the current chain

##### Returns

[`IChainConfig`](./IChainConfig)

#### Defined in

[wasm/lib/detailed/interfaces.ts:674](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L674)

## Methods

### calculateAccountHp()

> **calculateAccountHp**(`vests`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1033](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1033)

***

### calculateCurrentManabarValue()

> **calculateCurrentManabarValue**(`now`, `maxMana`, `currentMana`, `lastUpdateTime`): [`IManabarData`](./IManabarData)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1005](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1005)

***

### calculateHpApr()

> **calculateHpApr**(`headBlockNum`, `vestingRewardPercent`, `virtualSupply`, `totalVestingFundHive`): `number`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1056](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1056)

***

### calculateManabarFullRegenerationTime()

> **calculateManabarFullRegenerationTime**(`now`, `maxMana`, `currentMana`, `lastUpdateTime`): `number`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1022](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1022)

***

### calculatePublicKey()

> **calculatePublicKey**(`wifPrivateKey`): `string`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:937](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L937)

***

### calculateWitnessVotesHp()

> **calculateWitnessVotesHp**(`votes`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1044](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1044)

***

### convertRawPrivateKeyToWif()

> **convertRawPrivateKeyToWif**(`rawPrivateKey`): `string`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:945](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L945)

***

### convertRawPublicKeyToWif()

> **convertRawPublicKeyToWif**(`rawPublicKey`): `string`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:953](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L953)

***

### convertTransactionFromBinaryForm()

> **convertTransactionFromBinaryForm**(`transaction`): [`ApiTransaction`](../type-aliases/ApiTransaction)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1123](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1123)

***

### convertTransactionToBinaryForm()

> **convertTransactionToBinaryForm**(`transaction`, `stripToUnsignedTransaction`?): `string`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:1113](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1113)

***

### createTransactionFromJson()

> **createTransactionFromJson**(`transactionData`): [`ITransaction`](./ITransaction)

Converts Hive API-form transaction in JSON form to our transaction

#### Parameters

##### transactionData

transaction data to be converted

`string` | `object` | [`ApiTransaction`](../type-aliases/ApiTransaction)

#### Returns

[`ITransaction`](./ITransaction)

transaction containing ready to sign transaction (or to convert to protobuf structure using [ITransaction.transaction](./ITransactionBase#transaction) property)

#### Throws

on any Wax API-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:1074](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1074)

***

### createTransactionFromLegacyJson()

> **createTransactionFromLegacyJson**(`transactionData`): [`ITransaction`](./ITransaction)

Converts Hive API-form transaction in legacy JSON form to our transaction

#### Parameters

##### transactionData

transaction data to be converted

`string` | `object` | [`LegacyApiTransaction`](../type-aliases/LegacyApiTransaction)

#### Returns

[`ITransaction`](./ITransaction)

transaction containing ready to sign transaction (or to convert to protobuf structure using [ITransaction.transaction](./ITransactionBase#transaction) property)

#### Throws

on any Wax API-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:1085](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1085)

***

### createTransactionFromProto()

> **createTransactionFromProto**(`protoTransaction`): [`ITransaction`](./ITransaction)

Constructs a new Transaction object with ready protobuf transaction

#### Parameters

##### protoTransaction

[`transaction`](./transaction)

protobuf transaction

#### Returns

[`ITransaction`](./ITransaction)

#### Defined in

[wasm/lib/detailed/interfaces.ts:1063](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1063)

***

### createTransactionWithTaPoS()

> **createTransactionWithTaPoS**(`taposBlockId`, `expirationTime`?): [`ITransaction`](./ITransaction)

Constructs a new Transaction object with given data

#### Parameters

##### taposBlockId

`string`

reference block id (can be head block id) for TaPoS

##### expirationTime?

[`TTimestamp`](../type-aliases/TTimestamp)

expiration time for the transaction. Applies upon the [ITransaction.sign](./ITransactionBase#sign) call or reading [ITransaction.transaction](./ITransactionBase#transaction) property.
                                   Can be either any argument parsable by the Date constructor or relative time in seconds, minutes or hours
                                   (remember maximum expiration time for the transaction in mainnet is 1 hour), e.g.:
                                   `1699550966300` `"2023-11-09T17:29:30.028Z"` `new Date()` `"+10s"` `+30m` `+1h`.
                                   Expiration time will be applied when calling any non-push-related method in [ITransaction](./ITransaction)

#### Returns

[`ITransaction`](./ITransaction)

ready to use transaction interface allowing to fill transaction with its contents like Hive operations

#### Throws

on any Wax API-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:1102](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1102)

***

### ~~decrypt()~~

> **decrypt**(`wallet`, `encrypted`): `string`

Decrypts given data from the encrypted string in `#encrypted` format

#### Parameters

##### wallet

[`ISignatureProvider`](./ISignatureProvider)

Wallet with imported encryption keys

##### encrypted

`string`

Content to be decoded

#### Returns

`string`

Decoded content

#### Deprecated

Use dedicated encryption providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

#### Defined in

[wasm/lib/detailed/interfaces.ts:988](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L988)

***

### delete()

> **delete**(): `void`

Deletes the created wax proto_protocol instance

#### Returns

`void`

#### Throws

on any Wax WASM-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:1129](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L1129)

***

### ~~encrypt()~~

> **encrypt**(`wallet`, `content`, `mainEncryptionKey`, `otherEncryptionKey`?, `nonce`?): `string`

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

`string`

Encrypted content

#### Deprecated

Use dedicated encryption providers, such as:
  - `@hiveio/wax-signers-beekeeper`
  - `@hiveio/wax-signers-metamask`
  - `@hiveio/wax-signers-keychain`
  - `@hiveio/wax-signers-peakvault`

#### Defined in

[wasm/lib/detailed/interfaces.ts:972](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L972)

***

### estimateHbdInterest()

> **estimateHbdInterest**(`accountHdbSeconds`, `hbdBalance`, `lastCompoundingDate`, `now`, `interestRate`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:709](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L709)

***

### estimateHiveCollateral()

> **estimateHiveCollateral**(`currentMedianHistoryBase`, `currentMedianHistoryQuote`, `currentMinHistoryBase`, `currentMinHistoryQuote`, `hbdAmountToGet`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:697](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L697)

***

### extendConfig()

> **extendConfig**(`config`): [`IWaxBaseInterface`](./IWaxBaseInterface)

Extends the current wax base instance with your custom options, creating a copy of the current instance with altered config.

#### Parameters

##### config

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

configuration options to extend

#### Returns

[`IWaxBaseInterface`](./IWaxBaseInterface)

#### Defined in

[wasm/lib/detailed/interfaces.ts:629](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L629)

***

### getAsset()

> **getAsset**(`nai`): [`IHiveAssetData`](./IHiveAssetData)

Retrieves asset amount and symbol from the api data

#### Parameters

##### nai

[`NaiAsset`](./NaiAsset)

API asset

#### Returns

[`IHiveAssetData`](./IHiveAssetData)

asset data

#### Defined in

[wasm/lib/detailed/interfaces.ts:682](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L682)

***

### getPrivateKeyFromPassword()

> **getPrivateKeyFromPassword**(`account`, `role`, `password`): [`IPrivateKeyData`](./IPrivateKeyData)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:927](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L927)

***

### getPublicKeyFromSignature()

> **getPublicKeyFromSignature**(`sigDigest`, `signature`): `string`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:902](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L902)

***

### getVersion()

> **getVersion**(): `string`

Retrieves the bundled package version string

#### Returns

`string`

application version

#### Defined in

[wasm/lib/detailed/interfaces.ts:669](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L669)

***

### ~~hbd()~~

> **hbd**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:833](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L833)

***

### hbdCoins()

> **hbdCoins**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:739](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L739)

***

### hbdSatoshis()

> **hbdSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:784](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L784)

***

### hbdToHive()

> **hbdToHive**(`hbd`, `base`, `quote`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:880](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L880)

***

### ~~hive()~~

> **hive**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:816](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L816)

***

### hiveCoins()

> **hiveCoins**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:724](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L724)

***

### hiveSatoshis()

> **hiveSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:769](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L769)

***

### hiveToHbd()

> **hiveToHbd**(`amount`, `base`, `quote`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:890](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L890)

***

### hpToVests()

> **hpToVests**(`hive`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:870](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L870)

***

### isValidAccountName()

> **isValidAccountName**(`name`): `boolean`

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:640](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L640)

***

### operationBinaryViewMetadata()

> **operationBinaryViewMetadata**(`operation`, `isHf26Serialization`?): [`IBinaryViewOutputData`](./IBinaryViewOutputData)

Retrieves given operation binary view packed "AST" data (in same form as in the block_log)

#### Parameters

##### operation

The operation object which could be either a protobuf operation or operation returned from the Hive Nodes API

[`operation`](./operation) | [`ApiOperation`](./ApiOperation)

##### isHf26Serialization?

`boolean`

A flag indicating if serialization should be done in HF26 form or legacy form (defaults to `true` - hf26 type)

#### Returns

[`IBinaryViewOutputData`](./IBinaryViewOutputData)

binary view metadata

#### Throws

on any Wax WASM-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:662](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L662)

***

### operationGetImpactedAccounts()

> **operationGetImpactedAccounts**(`operation`): `Set`\<`string`\>

Retrieves the set of account names (not authorities!) that are impacted by a given operation.

#### Parameters

##### operation

The operation object which could be either a protobuf operation or operation returned from the Hive Nodes API

[`operation`](./operation) | [`ApiOperation`](./ApiOperation)

#### Returns

`Set`\<`string`\>

A set containing the account names that are impacted by the given operation.

#### Throws

on any Wax WASM-related error

#### Defined in

[wasm/lib/detailed/interfaces.ts:650](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L650)

***

### suggestBrainKey()

> **suggestBrainKey**(): [`IBrainKeyData`](./IBrainKeyData)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:915](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L915)

***

### ~~vests()~~

> **vests**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:850](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L850)

***

### vestsCoins()

> **vestsCoins**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:754](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L754)

***

### vestsSatoshis()

> **vestsSatoshis**(`amount`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:799](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L799)

***

### vestsToHp()

> **vestsToHp**(`vests`, `totalVestingFundHive`, `totalVestingShares`): [`NaiAsset`](./NaiAsset)

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

#### Defined in

[wasm/lib/detailed/interfaces.ts:860](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L860)
