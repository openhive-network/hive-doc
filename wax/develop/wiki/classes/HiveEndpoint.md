[@hiveio/wax](../globals) / HiveEndpoint

# Class: HiveEndpoint

## Implements

- [`IHiveEndpoint`](../interfaces/IHiveEndpoint)

## Constructors

### new HiveEndpoint()

> **new HiveEndpoint**(`checker`, `id`, `apiCallerId`, `paths`, `endpointUrls`, `caller`): [`HiveEndpoint`](./HiveEndpoint)

#### Parameters

##### checker

[`HealthChecker`](./HealthChecker)

##### id

`number`

##### apiCallerId

[`EChainApiType`](../enumerations/EChainApiType)

##### paths

`string`[]

##### endpointUrls

`Readonly`\<`Set`\<`string`\>\>

##### caller

(`apiUrl`) => `Promise`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`any`\>\>

#### Returns

[`HiveEndpoint`](./HiveEndpoint)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L86)

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

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`apiCallerId`](../interfaces/IHiveEndpoint#apicallerid)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:89](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L89)

***

### endpointUrls

> `readonly` **endpointUrls**: `Readonly`\<`Set`\<`string`\>\>

Endpoints that will be checked

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`endpointUrls`](../interfaces/IHiveEndpoint#endpointurls)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:91](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L91)

***

### id

> `readonly` **id**: `number`

Unique identifier for this endpoint
Can be used upon validationerror parsing to properly identify the endpoint

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`id`](../interfaces/IHiveEndpoint#id)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:88](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L88)

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

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`paths`](../interfaces/IHiveEndpoint#paths)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:90](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L90)

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

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`addEndpointUrl`](../interfaces/IHiveEndpoint#addendpointurl)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:95](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L95)

***

### list()

> **list**(): [`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

Lists sorted endpoint url statuses (latency in descending order)

#### Returns

[`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`list`](../interfaces/IHiveEndpoint#list)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:82](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L82)

***

### performCheck()

> **performCheck**(): `Promise`\<`void`\>

#### Returns

`Promise`\<`void`\>

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:108](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L108)

***

### removeEndpointUrl()

> **removeEndpointUrl**(`endpointUrl`, `clearUnusedEndpointUrlsFromStats`): `boolean`

Removes endpoint url from the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to remove

##### clearUnusedEndpointUrlsFromStats

`boolean` = `true`

#### Returns

`boolean`

true if endpoint was removed, false if it was not found

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`removeEndpointUrl`](../interfaces/IHiveEndpoint#removeendpointurl)

#### Defined in

[wasm/lib/detailed/healthchecker/endpoint.ts:99](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L99)
