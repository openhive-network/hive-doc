[@hiveio/wax](../globals) / IWaxOptions

# Interface: IWaxOptions

Defined in: [wasm/lib/detailed/interfaces.ts:152](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L152)

## Extends

- [`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions)

## Extended by

- [`IWaxOptionsChain`](./IWaxOptionsChain)

## Properties

### chainId

> **chainId**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:111](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L111)

Chain id in hex string format

#### Inherited from

[`IWaxBaseExtendibleOptions`](./IWaxBaseExtendibleOptions).[`chainId`](./IWaxBaseExtendibleOptions#chainid)

***

### wasmLocation?

> `optional` **wasmLocation?**: `string`

Defined in: [wasm/lib/detailed/interfaces.ts:170](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/interfaces.ts#L170)

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
