[@hiveio/wax](../globals) / HiveRoleAuthorityDefinition

# Interface: HiveRoleAuthorityDefinition\<TRole\>

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:8](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L8)

## Extends

- `LevelBase`\<`TRole`\>

## Type Parameters

### TRole

`TRole` *extends* `string`

## Properties

### level

> **level**: `TRole`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/level\_base.ts:10](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/level_base.ts#L10)

Role level name. It should be unique and marked `as const` for proper type narrowing
(See: https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-4.html#const-assertions)

#### Inherited from

`LevelBase.level`

## Accessors

### changed

#### Get Signature

> **get** **changed**(): `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:39](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L39)

Checks if the authority has changed since the last update.

This check does not rely on previous [add](./#add), [remove](./#remove) etc. calls, but rather on deep comparison of the authority object.

##### Returns

`boolean`

#### Overrides

`LevelBase.changed`

***

### isNullAuthority

#### Get Signature

> **get** **isNullAuthority**(): `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:218](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L218)

Checks if the currently selected role is null - everyone can access your account - no account nor key authorities.

##### Returns

`boolean`

Either true or false depending on whether the authority is null or not.

***

### value

#### Get Signature

> **get** **value**(): `Readonly`\<[`authority`](./authority)\>

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:73](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L73)

##### Returns

`Readonly`\<[`authority`](./authority)\>

#### Overrides

`LevelBase.value`

## Methods

### add()

> **add**(`accountOrKey`, `weight?`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:122](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L122)

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

***

### addToRole()

> `protected` **addToRole**(`accountOrKey`, `weight`): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:77](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L77)

#### Parameters

##### accountOrKey

`string`

##### weight

`number`

#### Returns

`void`

***

### clear()

> **clear**(): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:203](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L203)

Clears the currently selected role making it null authority. See [isNullAuthority](./#isnullauthority) method.

#### Returns

`this`

itself

***

### enforceModifications()

> **enforceModifications**(): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:30](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L30)

Once called, will mark given role as modified, and effectively push its definition into final operation.

#### Returns

`void`

#### Overrides

`LevelBase.enforceModifications`

***

### ensureValidAccountOrKey()

> `protected` **ensureValidAccountOrKey**(`accountOrKey`): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:99](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L99)

#### Parameters

##### accountOrKey

`string`

#### Returns

`void`

***

### getTuple()

> `protected` **getTuple**(`accountOrKey`): `void` \| \[`string`, `number`\]

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:104](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L104)

#### Parameters

##### accountOrKey

`string`

#### Returns

`void` \| \[`string`, `number`\]

***

### has()

> **has**(`accountOrKey`, `weight?`): `boolean`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:173](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L173)

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

***

### init()

> **init**(`maxAccountNameLength`, `hiveAddressPrefix`, `authority`): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L66)

#### Parameters

##### maxAccountNameLength

`number`

##### hiveAddressPrefix

`string`

##### authority

[`authority`](./authority)

#### Returns

`void`

***

### remove()

> **remove**(`accountOrKey`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:158](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L158)

Removes given account or key from the currently selected role.
Does nothing if the account or key is not present.

#### Parameters

##### accountOrKey

`string`

Account or key to be removed from the currently selected role.

#### Returns

`this`

itself

***

### removeFromRole()

> `protected` **removeFromRole**(`accountOrKey`): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:87](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L87)

#### Parameters

##### accountOrKey

`string`

#### Returns

`void`

***

### replace()

> **replace**(`accountOrKey`, `weight`, `newKeyOrAccount?`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:138](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L138)

Replaces the account or key with a new one in the currently selected role or changes the weight of the existing account or key.

#### Parameters

##### accountOrKey

`string`

Account or key to be added to the currently selected role.

##### weight

`number`

Account or key weight in the authority.

##### newKeyOrAccount?

`string` = `accountOrKey`

Account or key to replace the old one. If not provided, the account or key is not replaced, but weight is changed.

#### Returns

`this`

itself

***

### reset()

> **reset**(): `void`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L26)

Resets the level to its initial state.

#### Returns

`void`

#### Overrides

`LevelBase.reset`

***

### setTreshold()

> **setTreshold**(`treshold?`): `this`

Defined in: [wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/hive\_role\_authority\_definition.ts:190](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/hive_role_authority_definition.ts#L190)

Sets weight threshold for the currently selected role.

#### Parameters

##### treshold?

`number` = `1`

weight threshold for the currently selected role. Defaults to 1.

#### Returns

`this`

itself
