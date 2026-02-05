[@hiveio/wax](../globals) / YourApiData

# Type Alias: YourApiData\<YourTypes\>

> **YourApiData**\<`YourTypes`\>: `{ readonly [P in keyof YourTypes]: YourTypes[P] extends object ? YourTypes[P] extends { params: infer ParamsType; responseArray: boolean; result: infer ResultType } ? (ParamsType extends undefined ? (...) : (params: ...) => ...) & { endpointUrl: any } & Omit<YourApiData<(...)>, keyof (...)> : YourTypes[P] extends { params: infer ParamsType; result: infer ResultType } ? (...) & { endpointUrl: any } & (...) : YourApiData<(...)> & { endpointUrl: any } : never }` & `object`

**`Internal`**

## Type declaration

### endpointUrl

#### Get Signature

> **get** **endpointUrl**(): `string`

Retrieves the url used for calls to the specified API

##### Returns

`string`

#### Set Signature

> **set** **endpointUrl**(`newUrl`): `void`

New url to set per API. Pass `undefined` to switch back to default endpoint URL specified in the chain configuration ([IWaxOptionsChain.restApiEndpoint](../interfaces/IWaxChainExtendibleOptions#restapiendpoint))

##### Parameters

###### newUrl

`undefined` | `string`

##### Returns

`void`

## Type Parameters

• **YourTypes**

## Defined in

[wasm/lib/detailed/interfaces.ts:1152](https://gitlab.syncad.com/hive/wax/-/blob/8ad2b63c881a2d911b31e0c06383e6fc0fe73d22/ts/wasm/lib/detailed/interfaces.ts#L1152)
