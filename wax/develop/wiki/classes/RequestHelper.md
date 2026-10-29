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

#### Throws

HTTP Response code is in range 200-399 (inclusive), but the response body is not a valid JSON

#### Throws

Request did not complete within the configured timeout

#### Throws

Request was aborted by the user agent

#### Throws

Request failed without receiving a response (e.g. network or CORS error)

#### Defined in

[wasm/lib/detailed/util/request\_helper.ts:125](https://gitlab.syncad.com/hive/wax/-/blob/3722012494e8b95cad34795ca4735863e6a7742f/ts/wasm/lib/detailed/util/request_helper.ts#L125)
