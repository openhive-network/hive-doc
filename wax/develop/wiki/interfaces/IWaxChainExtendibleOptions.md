[@hiveio/wax](../globals) / IWaxChainExtendibleOptions

# Interface: IWaxChainExtendibleOptions

Defined in: [wasm/lib/detailed/interfaces.ts:114](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L114)

## Extends

- [`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

## Extended by

- [`IWaxOptionsChain`](./IWaxOptionsChain)

## Properties

### apiEndpoint

> **apiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L121)

Endpoint for all of the API requests

#### Default

```ts
"https://api.hive.blog/"
```

***

### apiTimeout

> **apiTimeout**: `number`

Defined in: [wasm/lib/detailed/interfaces.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L149)

Timeout for all of the API requests in milliseconds.
Set to 0 to disable timeout

#### Default

```ts
2_000
```

***

### chainId

> **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:111](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L111)

Chain id in hex string format

#### Inherited from

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions).[`chainId`](./IWaxBaseExtendibleOptions#chainid)

***

### restApiEndpoint

> **restApiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:129](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L129)

Endpoint for all of the REST API requests

#### Default

```ts
"https://api.syncad.com"
```

***

### waxApiCaller?

> `optional` **waxApiCaller?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:140](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/interfaces.ts#L140)

X-Wax-Api-Caller header value for all requests (both API and REST API).
This header is used to identify the application making requests to the server.
If not set, the X-Wax-Api-Caller header will not be sent with requests.
This setting is global for the entire chain configuration and cannot be overridden per API.

#### Default

```ts
undefined
```
