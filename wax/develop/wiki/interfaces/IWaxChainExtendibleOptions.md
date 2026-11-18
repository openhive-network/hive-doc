[@hiveio/wax](../globals) / IWaxChainExtendibleOptions

# Interface: IWaxChainExtendibleOptions

Defined in: [wasm/lib/detailed/interfaces.ts:120](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L120)

## Extends

- [`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

## Extended by

- [`IWaxOptionsChain`](./IWaxOptionsChain)

## Properties

### apiEndpoint

> **apiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:127](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L127)

Endpoint for all of the API requests

#### Default

```ts
"https://api.hive.blog/"
```

***

### apiTimeout

> **apiTimeout**: `number`

Defined in: [wasm/lib/detailed/interfaces.ts:155](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L155)

Timeout for all of the API requests in milliseconds.
Set to 0 to disable timeout

#### Default

```ts
2_000
```

***

### chainId

> **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:117](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L117)

Chain id in hex string format

#### Inherited from

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions).[`chainId`](./IWaxBaseExtendibleOptions#chainid)

***

### restApiEndpoint

> **restApiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:135](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L135)

Endpoint for all of the REST API requests

#### Default

```ts
"https://api.syncad.com"
```

***

### waxApiCaller?

> `optional` **waxApiCaller?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:146](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L146)

X-Wax-Api-Caller header value for all requests (both API and REST API).
This header is used to identify the application making requests to the server.
If not set, the X-Wax-Api-Caller header will not be sent with requests.
This setting is global for the entire chain configuration and cannot be overridden per API.

#### Default

```ts
undefined
```
