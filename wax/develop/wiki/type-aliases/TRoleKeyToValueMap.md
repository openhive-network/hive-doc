[@hiveio/wax](../globals) / TRoleKeyToValueMap

# Type Alias: TRoleKeyToValueMap

> **TRoleKeyToValueMap** = \{ \[K in keyof TRolesStruct\]: Omit\<TRolesStruct\[K\], "init" \| "enforceModifications"\> \}

Defined in: [wasm/lib/detailed/complex\_operations/account\_update.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/account_update.ts#L25)
