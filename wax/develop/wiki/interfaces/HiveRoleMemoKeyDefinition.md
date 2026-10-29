[@hiveio/wax](../globals) / HiveRoleMemoKeyDefinition

# Interface: HiveRoleMemoKeyDefinition

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:5](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L5)

## Extends

- `LevelBase`\<`"memo"`\>

## Properties

### level

> **level**: `"memo"`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/level\_base.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/level_base.ts#L10)

Role level name. It should be unique and marked `as const` for proper type narrowing
(See: https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-4.html#const-assertions)

#### Inherited from

`LevelBase.level`

## Accessors

### changed

#### Get Signature

> **get** **changed**(): `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L40)

Checks if the key has changed since the last update.

This check does not rely on previous [set](./#set) call, but rather on comparison of the public key value.

##### Returns

`boolean`

#### Overrides

`LevelBase.changed`

***

### isSet

#### Get Signature

> **get** **isSet**(): `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L68)

Checks if the memo key is set to the default value - null public key (`STM1111111111111111111111111111111114T1Anm`)

##### Returns

`boolean`

Either true or false depending on whether the public key is set or not.

***

### value

#### Get Signature

> **get** **value**(): `string`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L44)

##### Returns

`string`

#### Overrides

`LevelBase.value`

## Methods

### enforceModifications()

> **enforceModifications**(): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:31](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L31)

Once called, will mark given role as modified, and effectively push its definition into final operation.

#### Returns

`void`

#### Overrides

`LevelBase.enforceModifications`

***

### init()

> **init**(`hiveAddressPrefix`, `publicKey`): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L22)

#### Parameters

##### hiveAddressPrefix

`string`

##### publicKey

`string`

#### Returns

`void`

***

### reset()

> **reset**(): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L18)

Resets the level to its initial state.

#### Returns

`void`

#### Overrides

`LevelBase.reset`

***

### set()

> **set**(`publicKey`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_memo\_key.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_memo_key.ts#L54)

Sets the provided public key as the account memo key.

#### Parameters

##### publicKey

`string`

Public key to be set as the account memo key

#### Returns

`this`

itself
