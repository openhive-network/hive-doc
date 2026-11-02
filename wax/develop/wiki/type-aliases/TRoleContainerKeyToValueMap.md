[@hiveio/wax](../globals) / TRoleContainerKeyToValueMap

# Type Alias: TRoleContainerKeyToValueMap

> **TRoleContainerKeyToValueMap** = \{ \[C in InstanceType\<typeof AuthorityRoleCategories\[number\]\> as C\["category"\]\]: \{ \[K in keyof C\["authorities"\]\]: Omit\<C\["authorities"\]\[K\], "init" \| "enforceModifications"\> \}\[keyof C\["authorities"\]\] \}

Defined in: [wasm/lib/detailed/complex\_operations/account\_update.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/b01b7edf441b2e4ae66d53ccdeaa3b4aec519fbb/ts/wasm/lib/detailed/complex_operations/account_update.ts#L29)
