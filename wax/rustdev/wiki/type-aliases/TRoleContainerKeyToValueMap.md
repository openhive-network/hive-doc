[@hiveio/wax](../globals) / TRoleContainerKeyToValueMap

# Type Alias: TRoleContainerKeyToValueMap

> **TRoleContainerKeyToValueMap**: \{ \[C in InstanceType\<typeof AuthorityRoleCategories\[number\]\> as C\["category"\]\]: \{ \[K in keyof C\["authorities"\]\]: Omit\<C\["authorities"\]\[K\], "init" \| "enforceModifications"\> \}\[keyof C\["authorities"\]\] \}

## Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/01139ad1e8636f968fe3751f59b69c3a0bb4bb0c/ts/wasm/lib/detailed/complex_operations/account_update.ts#L29)
