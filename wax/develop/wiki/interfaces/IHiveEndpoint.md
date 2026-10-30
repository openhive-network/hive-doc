[@hiveio/wax](../globals) / IHiveEndpoint

# Interface: IHiveEndpoint

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:6](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L6)

## Properties

### apiCallerId

> `readonly` **apiCallerId**: [`EChainApiType`](../enumerations/EChainApiType)

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L17)

#### Examples

```ts
'json_rpc'
```

```ts
'rest'
```

***

### endpointUrls

> `readonly` **endpointUrls**: `Readonly`\<`Set`\<`string`\>\>

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L22)

Endpoints that will be checked

***

### id

> `readonly` **id**: `number`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L28)

Unique identifier for this endpoint
Can be used upon validationerror parsing to properly identify the endpoint

***

### paths

> `readonly` **paths**: `string`[]

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L11)

#### Examples

```ts
['block_api', 'get_block_header']
```

```ts
['hafbe-api', 'operation-type-counts']
```

## Methods

### addEndpointUrl()

> **addEndpointUrl**(`endpointUrl`): `void`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L34)

Adds new endpoint url to the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to add

#### Returns

`void`

***

### list()

> **list**(): [`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L46)

Lists sorted endpoint url statuses (latency in descending order)

#### Returns

[`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

***

### removeEndpointUrl()

> **removeEndpointUrl**(`endpointUrl`): `boolean`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:41](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L41)

Removes endpoint url from the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to remove

#### Returns

`boolean`

true if endpoint was removed, false if it was not found
