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

[wasm/lib/detailed/util/request\_helper.ts:103](https://gitlab.syncad.com/hive/wax/-/blob/68ec4e7437e5f2c8b344551ab8912a85d3c584ec/ts/wasm/lib/detailed/util/request_helper.ts#L103)
