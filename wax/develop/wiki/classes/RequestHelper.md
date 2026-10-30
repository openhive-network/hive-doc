[@hiveio/wax](../globals) / RequestHelper

# Class: RequestHelper

Defined in: [wasm/lib/detailed/util/request\_helper.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/util/request_helper.ts#L32)

## Constructors

### Constructor

> **new RequestHelper**(): `RequestHelper`

#### Returns

`RequestHelper`

## Methods

### request()

> **request**\<`TResponse`\>(`config`): `Promise`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`TResponse`\>\>

Defined in: [wasm/lib/detailed/util/request\_helper.ts:125](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/util/request_helper.ts#L125)

Requests given resource with timings

#### Type Parameters

##### TResponse

`TResponse` *extends* `string` \| `object` = `string`

#### Parameters

##### config

[`IRequestOptions`](../interfaces/IRequestOptions)

request data

#### Returns

`Promise`\<[`IDetailedResponseData`](../interfaces/IDetailedResponseData)\<`TResponse`\>\>

data for the account retrieval

#### Throws

HTTP Response code is not in range 200-399 (inclusive)

#### Throws

HTTP Response code is in range 200-399 (inclusive), but the response body is not a valid JSON

#### Throws

Request did not complete within the configured timeout

#### Throws

Request was aborted by the user agent

#### Throws

Request failed without receiving a response (e.g. network or CORS error)
