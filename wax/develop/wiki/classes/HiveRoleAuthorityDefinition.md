[@hiveio/wax](../globals) / HiveRoleAuthorityDefinition

# Class: HiveRoleAuthorityDefinition\<TRole\>

## Extends

- `LevelBase`\<`TRole`\>

## Type Parameters

• **TRole** *extends* `string`

## Constructors

### new HiveRoleAuthorityDefinition()

> **new HiveRoleAuthorityDefinition**\<`TRole`\>(`role`, `ensureCanUpdate`): [`HiveRoleAuthorityDefinition`](./HiveRoleAuthorityDefinition)\<`TRole`\>

#### Parameters

##### role

`TRole`

##### ensureCanUpdate

(`level`) => `void`

#### Returns

[`HiveRoleAuthorityDefinition`](./HiveRoleAuthorityDefinition)\<`TRole`\>

#### Overrides

`LevelBase<TRole>.constructor`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:9](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L9)

## Properties

### level

> **level**: `TRole`

Role level name. It should be unique and marked `as const` for proper type narrowing
(See: https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-4.html#const-assertions)

#### Inherited from

`LevelBase.level`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/level\_base.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/level_base.ts#L10)

## Accessors

### changed

#### Get Signature

> **get** **changed**(): `boolean`

Checks if the authority has changed since the last update.

This check does not rely on previous [add](./HiveRoleAuthorityDefinition#add), [remove](./HiveRoleAuthorityDefinition#remove) etc. calls, but rather on deep comparison of the authority object.

##### Returns

`boolean`

#### Overrides

`LevelBase.changed`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:39](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L39)

***

### isNullAuthority

#### Get Signature

> **get** **isNullAuthority**(): `boolean`

Checks if the currently selected role is null - everyone can access your account - no account nor key authorities.

##### Returns

`boolean`

Either true or false depending on whether the authority is null or not.

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:218](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L218)

***

### value

#### Get Signature

> **get** **value**(): `Readonly`\<[`authority`](../interfaces/authority)\>

##### Returns

`Readonly`\<[`authority`](../interfaces/authority)\>

#### Overrides

`LevelBase.value`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:73](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L73)

## Methods

### add()

> **add**(`accountOrKey`, `weight`?): `this`

Adds an account or key to the currently selected role with specified weight.
If the account or key already exists, its weight is updated.

#### Parameters

##### accountOrKey

`string`

Account or key to be added to the currently selected role.

##### weight?

`number` = `1`

Account or key weight in the authority. Default is 1.

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:122](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L122)

***

### addToRole()

> `protected` **addToRole**(`accountOrKey`, `weight`): `void`

#### Parameters

##### accountOrKey

`string`

##### weight

`number`

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:77](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L77)

***

### clear()

> **clear**(): `this`

Clears the currently selected role making it null authority. See [isNullAuthority](./HiveRoleAuthorityDefinition#isnullauthority) method.

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:203](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L203)

***

### enforceModifications()

> **enforceModifications**(): `void`

Once called, will mark given role as modified, and effectively push its definition into final operation.

#### Returns

`void`

#### Overrides

`LevelBase.enforceModifications`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L30)

***

### ensureValidAccountOrKey()

> `protected` **ensureValidAccountOrKey**(`accountOrKey`): `void`

#### Parameters

##### accountOrKey

`string`

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:99](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L99)

***

### getTuple()

> `protected` **getTuple**(`accountOrKey`): `void` \| [`string`, `number`]

#### Parameters

##### accountOrKey

`string`

#### Returns

`void` \| [`string`, `number`]

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:104](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L104)

***

### has()

> **has**(`accountOrKey`, `weight`?): `boolean`

Checks if the account or key is present in the currently selected role.

#### Parameters

##### accountOrKey

`string`

Account or key to be checked.

##### weight?

`number`

Account or key weight in the authority. If provided, the weight is checked as well.

#### Returns

`boolean`

Either true or false depending on whether the account or key is present in the currently selected role.

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:173](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L173)

***

### init()

> **init**(`maxAccountNameLength`, `hiveAddressPrefix`, `authority`): `void`

#### Parameters

##### maxAccountNameLength

`number`

##### hiveAddressPrefix

`string`

##### authority

[`authority`](../interfaces/authority)

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L66)

***

### remove()

> **remove**(`accountOrKey`): `this`

Removes given account or key from the currently selected role.
Does nothing if the account or key is not present.

#### Parameters

##### accountOrKey

`string`

Account or key to be removed from the currently selected role.

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:158](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L158)

***

### removeFromRole()

> `protected` **removeFromRole**(`accountOrKey`): `void`

#### Parameters

##### accountOrKey

`string`

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:87](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L87)

***

### replace()

> **replace**(`accountOrKey`, `weight`, `newKeyOrAccount`): `this`

Replaces the account or key with a new one in the currently selected role or changes the weight of the existing account or key.

#### Parameters

##### accountOrKey

`string`

Account or key to be added to the currently selected role.

##### weight

`number`

Account or key weight in the authority.

##### newKeyOrAccount

`string` = `accountOrKey`

Account or key to replace the old one. If not provided, the account or key is not replaced, but weight is changed.

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:138](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L138)

***

### reset()

> **reset**(): `void`

Resets the level to its initial state.

#### Returns

`void`

#### Overrides

`LevelBase.reset`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L26)

***

### setTreshold()

> **setTreshold**(`treshold`?): `this`

Sets weight threshold for the currently selected role.

#### Parameters

##### treshold?

`number` = `1`

weight threshold for the currently selected role. Defaults to 1.

#### Returns

`this`

itself

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:190](https://gitlab.syncad.com/hive/wax/-/blob/00bfff44d29ba8c012da43e0172222eab09f77bd/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L190)
