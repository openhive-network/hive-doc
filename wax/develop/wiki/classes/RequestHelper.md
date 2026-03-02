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

[wasm/lib/detailed/util/request\_helper.ts:103](https://gitlab.syncad.com/hive/wax/-/blob/d77f7d9ae3137cbfe5284992334839fb76a6ea96/ts/wasm/lib/detailed/util/request_helper.ts#L103)
