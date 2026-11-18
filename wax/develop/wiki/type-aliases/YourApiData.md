[@hiveio/wax](../globals) / YourApiData

# Type Alias: YourApiData\<YourTypes\>

> **YourApiData**\<`YourTypes`\> = `{ readonly [P in keyof YourTypes]: YourTypes[P] extends object ? YourTypes[P] extends { params: infer ParamsType; responseArray: boolean; result: infer ResultType } ? (ParamsType extends undefined ? (...) : (params: ...) => ...) & { endpointUrl: any } & Omit<YourApiData<(...)>, keyof (...)> : YourTypes[P] extends { params: infer ParamsType; result: infer ResultType } ? (...) & { endpointUrl: any } & (...) : YourApiData<(...)> & { endpointUrl: any } : never }` & `object`

Defined in: [wasm/lib/detailed/interfaces.ts:1160](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L1160)

**`Internal`**

## Type Parameters

### YourTypes

`YourTypes`

## Type Declaration

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

`string` \| `undefined`

##### Returns

`void`
