[@hiveio/wax](../globals) / HiveAccountCategory

# Class: HiveAccountCategory

## Extends

- `RoleCategoryBase`\<[`THiveRoles`](../type-aliases/THiveRoles)\>

## Constructors

### new HiveAccountCategory()

> **new HiveAccountCategory**(): [`HiveAccountCategory`](./HiveAccountCategory)

#### Returns

[`HiveAccountCategory`](./HiveAccountCategory)

#### Inherited from

`RoleCategoryBase<THiveRoles>.constructor`

## Properties

### authorities

> **authorities**: `Readonly`\<[`THiveRoles`](../type-aliases/THiveRoles)\>

#### Inherited from

`RoleCategoryBase.authorities`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/role\_category\_base.ts:15](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/complex_operations/role_classes/role_category_base.ts#L15)

***

### category

> **category**: `"hive"`

Category name. It should be unique and marked `as const` for proper type narrowing
(See: https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-4.html#const-assertions)

#### Overrides

`RoleCategoryBase.category`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/index.ts:23](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/index.ts#L23)

## Accessors

### changed

#### Get Signature

> **get** **changed**(): `boolean`

Indicates if any of the authority levels has changed since the last update.

##### Returns

`boolean`

#### Overrides

`RoleCategoryBase.changed`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/index.ts:25](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/index.ts#L25)

## Methods

### finalize()

> **finalize**(`_sink`): [`operation`](../interfaces/operation)[]

This function should return an array of operations that will modify the user account roles.

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

[`operation`](../interfaces/operation)[]

#### Overrides

`RoleCategoryBase.finalize`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/index.ts:104](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/index.ts#L104)

***

### init()

> **init**(`chain`, `account`): `Promise`\<`void`\>

This function is responsible for gathering authority types for the given account.
It should return an object with keys as role names and values as authority objects.
Keys you return will have an impact on the role types supported by the account authority update operation

#### Parameters

##### chain

[`IHiveChainInterface`](../interfaces/IHiveChainInterface)

##### account

`string`

#### Returns

`Promise`\<`void`\>

#### Overrides

`RoleCategoryBase.init`

#### Defined in

[wasm/lib/detailed/complex\_operations/role\_classes/categories/hive\_authority/index.ts:31](https://gitlab.syncad.com/hive/wax/-/blob/7356a732487b770e0eb1c04e8b68d7224bfd392e/ts/wasm/lib/detailed/complex_operations/role_classes/categories/hive_authority/index.ts#L31)
