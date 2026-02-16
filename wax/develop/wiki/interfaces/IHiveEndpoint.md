[@hiveio/wax](../globals) / IHiveEndpoint

# Interface: IHiveEndpoint

## Properties

### apiCallerId

> `readonly` **apiCallerId**: [`EChainApiType`](../enumerations/EChainApiType)

#### Examples

```ts
'json_rpc'
```

```ts
'rest'
```

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:17](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L17)

***

### endpointUrls

> `readonly` **endpointUrls**: `Readonly`\<`Set`\<`string`\>\>

Endpoints that will be checked

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L22)

***

### id

> `readonly` **id**: `number`

Unique identifier for this endpoint
Can be used upon validationerror parsing to properly identify the endpoint

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L28)

***

### paths

> `readonly` **paths**: `string`[]

#### Examples

```ts
['block_api', 'get_block_header']
```

```ts
['hafbe-api', 'operation-type-counts']
```

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:11](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L11)

## Methods

### addEndpointUrl()

> **addEndpointUrl**(`endpointUrl`): `void`

Adds new endpoint url to the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to add

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L34)

***

### list()

> **list**(): [`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

Lists sorted endpoint url statuses (latency in descending order)

#### Returns

[`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L46)

***

### removeEndpointUrl()

> **removeEndpointUrl**(`endpointUrl`): `boolean`

Removes endpoint url from the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to remove

#### Returns

`boolean`

true if endpoint was removed, false if it was not found

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:41](https://gitlab.syncad.com/hive/wax/-/blob/742eca65a48eb16152b3c1d1e2208fb91a5718b6/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L41)
