[@hiveio/wax](../globals) / HiveRoleMemoKeyDefinition

# Class: HiveRoleMemoKeyDefinition

## Extends

- `LevelBase`\<`"memo"`\>

## Constructors

### new HiveRoleMemoKeyDefinition()

> **new HiveRoleMemoKeyDefinition**(): [`HiveRoleMemoKeyDefinition`](./HiveRoleMemoKeyDefinition)

#### Returns

[`HiveRoleMemoKeyDefinition`](./HiveRoleMemoKeyDefinition)

#### Overrides

`LevelBase<"memo">.constructor`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:6](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L6)

## Properties

### level

> **level**: `"memo"`

Role level name. It should be unique and marked `as const` for proper type narrowing
(See: https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-4.html#const-assertions)

#### Inherited from

`LevelBase.level`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/level\_base.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/level_base.ts#L10)

## Accessors

### changed

#### Get Signature

> **get** **changed**(): `boolean`

Checks if the key has changed since the last update.

This check does not rely on previous [set](./HiveRoleMemoKeyDefinition#set) call, but rather on comparison of the public key value.

##### Returns

`boolean`

#### Overrides

`LevelBase.changed`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L40)

***

### isSet

#### Get Signature

> **get** **isSet**(): `boolean`

Checks if the memo key is set to the default value - null public key (`STM1111111111111111111111111111111114T1Anm`)

##### Returns

`boolean`

Either true or false depending on whether the public key is set or not.

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L68)

***

### value

#### Get Signature

> **get** **value**(): `string`

##### Returns

`string`

#### Overrides

`LevelBase.value`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L44)

## Methods

### enforceModifications()

> **enforceModifications**(): `void`

Once called, will mark given role as modified, and effectively push its definition into final operation.

#### Returns

`void`

#### Overrides

`LevelBase.enforceModifications`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:31](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L31)

***

### init()

> **init**(`hiveAddressPrefix`, `publicKey`): `void`

#### Parameters

##### hiveAddressPrefix

`string`

##### publicKey

`string`

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L22)

***

### reset()

> **reset**(): `void`

Resets the level to its initial state.

#### Returns

`void`

#### Overrides

`LevelBase.reset`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L18)

***

### set()

> **set**(`publicKey`): `this`

Sets the provided public key as the account memo key.

#### Parameters

##### publicKey

`string`

Public key to be set as the account memo key

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/81253b5206506b3154ceb85eea73e3fcbd6f30a6/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L54)
