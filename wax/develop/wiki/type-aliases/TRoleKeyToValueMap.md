[@hiveio/wax](../globals) / TRoleKeyToValueMap

# Type Alias: TRoleKeyToValueMap

> **TRoleKeyToValueMap** = \{ \[K in keyof TRolesStruct\]: Omit\<TRolesStruct\[K\], "init" \| "enforceModifications"\> \}

Defined in: [wasm/lib/detailed/complex\_operations/account\_update.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/1a91d054cf9d01385db4d6224262f77abf1c86b2/ts/wasm/lib/detailed/complex_operations/account_update.ts#L25)
