[@hiveio/wax](../globals) / TRoleContainerKeyToValueMap

# Type Alias: TRoleContainerKeyToValueMap

> **TRoleContainerKeyToValueMap**: \{ \[C in InstanceType\<typeof AuthorityRoleCategories\[number\]\> as C\["category"\]\]: \{ \[K in keyof C\["authorities"\]\]: Omit\<C\["authorities"\]\[K\], "init" \| "enforceModifications"\> \}\[keyof C\["authorities"\]\] \}

## Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:29](https://gitlab.syncad.com/hive/wax/-/blob/b151b63067d7ad83f36191a944e9354f16f88e6d/ts/wasm/lib/detailed/complex_operations/account_update.ts#L29)
