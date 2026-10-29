[@hiveio/wax](../globals) / HiveEndpoint

# Class: HiveEndpoint

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L78)

## Implements

- [`IHiveEndpoint`](../interfaces/IHiveEndpoint)

## Constructors

### Constructor

> **new HiveEndpoint**(`checker`, `id`, `apiCallerId`, `paths`, `endpointUrls`, `caller`): `HiveEndpoint`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:86](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L86)

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

`HiveEndpoint`

## Properties

### apiCallerId

> `readonly` **apiCallerId**: [`EChainApiType`](../enumerations/EChainApiType)

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:89](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L89)

#### Examples

```ts
'json_rpc'
```

```ts
'rest'
```

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`apiCallerId`](../interfaces/IHiveEndpoint#apicallerid)

***

### endpointUrls

> `readonly` **endpointUrls**: `Readonly`\<`Set`\<`string`\>\>

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:91](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L91)

Endpoints that will be checked

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`endpointUrls`](../interfaces/IHiveEndpoint#endpointurls)

***

### id

> `readonly` **id**: `number`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:88](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L88)

Unique identifier for this endpoint
Can be used upon validationerror parsing to properly identify the endpoint

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`id`](../interfaces/IHiveEndpoint#id)

***

### paths

> `readonly` **paths**: `string`[]

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:90](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L90)

#### Examples

```ts
['block_api', 'get_block_header']
```

```ts
['hafbe-api', 'operation-type-counts']
```

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`paths`](../interfaces/IHiveEndpoint#paths)

## Methods

### addEndpointUrl()

> **addEndpointUrl**(`endpointUrl`): `void`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:95](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L95)

Adds new endpoint url to the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to add

#### Returns

`void`

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`addEndpointUrl`](../interfaces/IHiveEndpoint#addendpointurl)

***

### list()

> **list**(): [`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:82](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L82)

Lists sorted endpoint url statuses (latency in descending order)

#### Returns

[`THiveEndpointData`](../type-aliases/THiveEndpointData)[]

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`list`](../interfaces/IHiveEndpoint#list)

***

### performCheck()

> **performCheck**(): `Promise`\<`void`\>

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:108](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L108)

#### Returns

`Promise`\<`void`\>

***

### removeEndpointUrl()

> **removeEndpointUrl**(`endpointUrl`, `clearUnusedEndpointUrlsFromStats?`): `boolean`

Defined in: [wasm/lib/detailed/healthchecker/endpoint.ts:99](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/healthchecker/endpoint.ts#L99)

Removes endpoint url from the list of urls to check

#### Parameters

##### endpointUrl

`string`

url to remove

##### clearUnusedEndpointUrlsFromStats?

`boolean` = `true`

#### Returns

`boolean`

true if endpoint was removed, false if it was not found

#### Implementation of

[`IHiveEndpoint`](../interfaces/IHiveEndpoint).[`removeEndpointUrl`](../interfaces/IHiveEndpoint#removeendpointurl)
