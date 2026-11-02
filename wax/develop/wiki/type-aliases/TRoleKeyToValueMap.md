[@hiveio/wax](../globals) / TRoleKeyToValueMap

# Type Alias: TRoleKeyToValueMap

> **TRoleKeyToValueMap** = \{ \[K in keyof TRolesStruct\]: Omit\<TRolesStruct\[K\], "init" \| "enforceModifications"\> \}

Defined in: [wasm/lib/detailed/complex\_operations/account\_update.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/complex_operations/account_update.ts#L25)
