[@hiveio/wax](../globals) / RequestHelper

# Class: RequestHelper

## Constructors

### new RequestHelper()

> **new RequestHelper**(): [`RequestHelper`](./RequestHelper)

#### Returns

[`RequestHelper`](./RequestHelper)

## Methods

### request()

> **request**\<`TResponse`\>(`config`): `Promise`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`TResponse`\>\>

Requests given resource with timings

#### Type Parameters

• **TResponse** *extends* `string` \| `object` = `string`

#### Parameters

##### config

[`IRequestOptions`](../interfaces/IRequestOptions)

request data

#### Returns

`Promise`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`TResponse`\>\>

data for the account retrieval

#### Throws

HTTP Response code is not in range 200-399 (inclusive)

#### Defined in

[wasm/lib/detailed/util/request\_helper.ts:103](https://gitlab.syncad.com/hive/wax/-/blob/e25b8c8d97e816ce4f4ff46288ec990cab9c8b9f/ts/wasm/lib/detailed/util/request_helper.ts#L103)
