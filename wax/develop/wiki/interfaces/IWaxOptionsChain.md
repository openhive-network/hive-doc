[@hiveio/wax](../globals) / IWaxOptionsChain

# Interface: IWaxOptionsChain

Defined in: [wasm/lib/detailed/interfaces.ts:182](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L182)

## Extends

- [`IWaxOptions`](./IWaxOptions)
- [`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions)

## Properties

### apiEndpoint

> **apiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L121)

Endpoint for all of the API requests

#### Default

```ts
"https://api.hive.blog/"
```

#### Inherited from

[`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions).[`apiEndpoint`](./IWaxChainExtendibleOptions#apiendpoint)

***

### apiTimeout

> **apiTimeout**: `number`

Defined in: [wasm/lib/detailed/interfaces.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L149)

Timeout for all of the API requests in milliseconds.
Set to 0 to disable timeout

#### Default

```ts
2_000
```

#### Inherited from

[`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions).[`apiTimeout`](./IWaxChainExtendibleOptions#apitimeout)

***

### chainId

> **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:111](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L111)

Chain id in hex string format

#### Inherited from

[`IWaxOptions`](./IWaxOptions).[`chainId`](./IWaxOptions#chainid)

***

### restApiEndpoint

> **restApiEndpoint**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:129](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L129)

Endpoint for all of the REST API requests

#### Default

```ts
"https://api.syncad.com"
```

#### Inherited from

[`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions).[`restApiEndpoint`](./IWaxChainExtendibleOptions#restapiendpoint)

***

### wasmLocation?

> `optional` **wasmLocation?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:170](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L170)

The path to the WASM file. It can be a relative path or an absolute URL
If not specified, the default path is used: "./build_wasm/wax.common.wasm" (may change if bundled)

Note: You can also specify a base64 encoded string of the WASM file to be used directly when inlining

Note: When you don't have your WASM file served from the static directory (such as `/public`),
      or you are bundling / transpiling your code,
      you may need to leverage your bundler's asset importing capabilities, e.g.:

         - For Vite:    `import wasmUrl from './my_wasm_files/wax.common.wasm?url';`
         - For Webpack: `const wasmUrl = new URL("./my_wasm_files/wax.common.wasm", import.meta.url).href;`
      Then pass the imported `wasmUrl` variable to this option.
      For web workers, replace `import.meta.url` with `self.location.href`.

#### Inherited from

[`IWaxOptions`](./IWaxOptions).[`wasmLocation`](./IWaxOptions#wasmlocation)

***

### waxApiCaller?

> `optional` **waxApiCaller?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:140](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/interfaces.ts#L140)

X-Wax-Api-Caller header value for all requests (both API and REST API).
This header is used to identify the application making requests to the server.
If not set, the X-Wax-Api-Caller header will not be sent with requests.
This setting is global for the entire chain configuration and cannot be overridden per API.

#### Default

```ts
undefined
```

#### Inherited from

[`IWaxChainExtendibleOptions`](./IWaxChainExtendibleOptions).[`waxApiCaller`](./IWaxChainExtendibleOptions#waxapicaller)
