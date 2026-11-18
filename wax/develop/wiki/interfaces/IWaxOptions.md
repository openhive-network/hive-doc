[@hiveio/wax](../globals) / IWaxOptions

# Interface: IWaxOptions

Defined in: [wasm/lib/detailed/interfaces.ts:158](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L158)

## Extends

- [`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

## Extended by

- [`IWaxOptionsChain`](./IWaxOptionsChain)

## Properties

### chainId

> **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:117](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L117)

Chain id in hex string format

#### Inherited from

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions).[`chainId`](./IWaxBaseExtendibleOptions#chainid)

***

### enableLogs?

> `optional` **enableLogs?**: `boolean`

Defined in: [wasm/lib/detailed/interfaces.ts:185](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L185)

Whether the WASM module may write its logs (e.g. the hive protocol `ilog` / `wlog` / `elog` messages) to the console.
Set to false to silence all of the WASM module output.

#### Default

```ts
true
```

***

### wasmLocation?

> `optional` **wasmLocation?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:176](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L176)

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
