[@hiveio/wax](../globals) / HiveApiTypes

# Type Alias: HiveApiTypes

> **HiveApiTypes** = `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:16](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L16)

## Properties

### account\_by\_key\_api

> **account\_by\_key\_api**: `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L17)

#### get\_key\_references

> **get\_key\_references**: `object`

##### get\_key\_references.params

> **params**: [`GetKeyReferencesRequest`](../interfaces/GetKeyReferencesRequest)

##### get\_key\_references.result

> **result**: [`GetKeyReferencesResponse`](../interfaces/GetKeyReferencesResponse)

***

### block\_api

> **block\_api**: `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:51](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L51)

#### get\_block

> **get\_block**: `object`

##### get\_block.params

> **params**: [`GetBlockRequest`](../interfaces/GetBlockRequest)

##### get\_block.result

> **result**: [`GetBlockResponse`](../interfaces/GetBlockResponse)

#### get\_block\_header

> **get\_block\_header**: `object`

##### get\_block\_header.params

> **params**: [`GetBlockHeaderRequest`](../interfaces/GetBlockHeaderRequest)

##### get\_block\_header.result

> **result**: [`GetBlockHeaderResponse`](../interfaces/GetBlockHeaderResponse)

#### get\_block\_range

> **get\_block\_range**: `object`

##### get\_block\_range.params

> **params**: [`GetBlockRangeRequest`](../interfaces/GetBlockRangeRequest)

##### get\_block\_range.result

> **result**: [`GetBlockRangeResponse`](../interfaces/GetBlockRangeResponse)

***

### database\_api

> **database\_api**: `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:23](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L23)

#### find\_accounts

> **find\_accounts**: `object`

##### find\_accounts.params

> **params**: [`FindAccountsRequest`](../interfaces/FindAccountsRequest)

##### find\_accounts.result

> **result**: [`FindAccountsResponse`](../interfaces/FindAccountsResponse)

#### find\_witnesses

> **find\_witnesses**: `object`

##### find\_witnesses.params

> **params**: [`FindWitnessesRequest`](../interfaces/FindWitnessesRequest)

##### find\_witnesses.result

> **result**: [`FindWitnessesResponse`](../interfaces/FindWitnessesResponse)

#### get\_dynamic\_global\_properties

> **get\_dynamic\_global\_properties**: `object`

##### get\_dynamic\_global\_properties.params

> **params**: [`GetDynamicGlobalPropertiesRequest`](../interfaces/GetDynamicGlobalPropertiesRequest)

##### get\_dynamic\_global\_properties.result

> **result**: [`GetDynamicGlobalPropertiesResponse`](../interfaces/GetDynamicGlobalPropertiesResponse)

#### get\_witness\_schedule

> **get\_witness\_schedule**: `object`

##### get\_witness\_schedule.params

> **params**: [`GetWitnessScheduleRequest`](../interfaces/GetWitnessScheduleRequest)

##### get\_witness\_schedule.result

> **result**: [`GetWitnessScheduleResponse`](../interfaces/GetWitnessScheduleResponse)

#### verify\_authority

> **verify\_authority**: `object`

##### verify\_authority.params

> **params**: [`VerifyAuthorityRequest`](../interfaces/VerifyAuthorityRequest)

##### verify\_authority.result

> **result**: [`VerifyAuthorityResponse`](../interfaces/VerifyAuthorityResponse)

***

### network\_broadcast\_api

> **network\_broadcast\_api**: `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L45)

#### broadcast\_transaction

> **broadcast\_transaction**: `object`

##### broadcast\_transaction.params

> **params**: [`BroadcastTransactionRequest`](../interfaces/BroadcastTransactionRequest)

##### broadcast\_transaction.result

> **result**: [`BroadcastTransactionResponse`](../interfaces/BroadcastTransactionResponse)

***

### rc\_api

> **rc\_api**: `object`

Defined in: [wasm/lib/detailed/chain\_api\_data.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/chain_api_data.ts#L65)

#### find\_rc\_accounts

> **find\_rc\_accounts**: `object`

##### find\_rc\_accounts.params

> **params**: [`FindRcAccountsRequest`](../interfaces/FindRcAccountsRequest)

##### find\_rc\_accounts.result

> **result**: [`FindRcAccountsResponse`](../interfaces/FindRcAccountsResponse)
