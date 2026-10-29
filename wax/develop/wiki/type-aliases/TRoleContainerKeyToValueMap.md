[@hiveio/wax](../globals) / TRoleContainerKeyToValueMap

# Type Alias: TRoleContainerKeyToValueMap

> **TRoleContainerKeyToValueMap** = \{ \[C in InstanceType\<typeof AuthorityRoleCategories\[number\]\> as C\["category"\]\]: \{ \[K in keyof C\["authorities"\]\]: Omit\<C\["authorities"\]\[K\], "init" \| "enforceModifications"\> \}\[keyof C\["authorities"\]\] \}

Defined in: [wasm/lib/detailed/complex\_operations/account\_update.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/account_update.ts#L29)
