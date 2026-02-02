[@hiveio/wax](../globals) / IWaxChainExtendibleOptions

# Interface: IWaxChainExtendibleOptions

## Extends

- [`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

## Extended by

- [`IWaxOptionsChain`](./IWaxOptionsChain)

## Properties

### apiEndpoint

> **apiEndpoint**: `string`

Endpoint for all of the API requests

#### Default

```ts
"https://api.hive.blog/"
```

#### Defined in

[wasm/lib/detailed/interfaces.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L121)

***

### apiTimeout

> **apiTimeout**: `number`

Timeout for all of the API requests in milliseconds.
Set to 0 to disable timeout

#### Default

```ts
2_000
```

#### Defined in

[wasm/lib/detailed/interfaces.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L149)

***

### chainId

> **chainId**: `string`

Chain id in hex string format

#### Inherited from

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions).[`chainId`](./IWaxBaseExtendibleOptions#chainid)

#### Defined in

[wasm/lib/detailed/interfaces.ts:111](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L111)

***

### restApiEndpoint

> **restApiEndpoint**: `string`

Endpoint for all of the REST API requests

#### Default

```ts
"https://api.syncad.com"
```

#### Defined in

[wasm/lib/detailed/interfaces.ts:129](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L129)

***

### waxApiCaller?

> `optional` **waxApiCaller**: `string`

X-Wax-Api-Caller header value for all requests (both API and REST API).
This header is used to identify the application making requests to the server.
If not set, the X-Wax-Api-Caller header will not be sent with requests.
This setting is global for the entire chain configuration and cannot be overridden per API.

#### Default

```ts
undefined
```

#### Defined in

[wasm/lib/detailed/interfaces.ts:140](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/interfaces.ts#L140)
