[@hiveio/wax](../globals) / AccountAuthorityUpdateOperation

# Class: AccountAuthorityUpdateOperation

Online operation - it is automatically filled in with the data acquired from the chain API.

The purpose of this operation is to simplify account authority update process by automatic gathering current authority data
from blockchain and then supplementing them by provided action methods. Operation is designed to support different authority categories
(right now is implemented Hive builtin authority).

It is initialized with all of the supported roles for the given account using [AccountAuthorityUpdateOperation.createFor](./AccountAuthorityUpdateOperation#createfor) automatically, so
for example: If you want to add a single key to the active level of the account, you can just add the key, without worrying about your other key authorities.

After initialization, you can use the [AccountAuthorityUpdateOperation.role](./AccountAuthorityUpdateOperation#role) method to retrieve the role instance for the given role level.

## Example

```ts
const operation = await AccountAuthorityUpdateOperation.createFor(myChain, "initminer");

const active = operation.role("active");
active.add(myKey);

const memo = operation.role("memo");
memo.set(myKey);
```

## Extends

- [`OperationBase`](./OperationBase)

## Accessors

### isEffective

#### Get Signature

> **get** **isEffective**(): `boolean`

Checks if the authority has changed since the last update and it is possible to transmit this operation (any changes applied)

##### Returns

`boolean`

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:149](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L149)

## Methods

### enforceOwnerRoleAuthorisation()

> **enforceOwnerRoleAuthorisation**(): `void`

Enforces the requirement for **owner** role authorization when modifying **active** or **posting** roles.

**HF 28** introduces stricter matching between the authority role required by a given operation and the role used to authorize the transaction.
- Since modifying **active** or **posting** roles requires **active** authority at the time of transaction signing, the pre-HF28 behavior — which allowed signing with the **owner** key — will be **disallowed**.  
- This change may pose difficulties for users who have lost their active keys and attempt to use their owner key to set a new one.  
- To address this, the function allows the inclusion — within the `account_update2_operation` generated internally — of elements that enforce the **owner** role requirement, specifically through an ineffective change of the owner authority to the same value currently recorded on-chain.

#### Returns

`void`

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:99](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L99)

***

### finalize()

> **finalize**(`sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Overrides

[`OperationBase`](./OperationBase).[`finalize`](./OperationBase#finalize)

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:161](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L161)

***

### role()

> **role**\<`KRole`\>(`level`): [`TRoleKeyToValueMap`](../type-aliases/TRoleKeyToValueMap)\[`KRole`\]

Returns the role instance for the given role level.

#### Type Parameters

• **KRole** *extends* keyof [`THiveRoles`](../type-aliases/THiveRoles)

#### Parameters

##### level

`KRole`

role level to retrieve

#### Returns

[`TRoleKeyToValueMap`](../type-aliases/TRoleKeyToValueMap)\[`KRole`\]

Role class instance for the given role level

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:111](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L111)

***

### roles()

> **roles**\<`KRoleContainer`\>(`category`): `Iterable`\<[`TRoleContainerKeyToValueMap`](../type-aliases/TRoleContainerKeyToValueMap)\[`KRoleContainer`\], `any`, `any`\>

Returns all of the roles for the given role category.

Note: You can differentiate between different role categories by using the `level` property

#### Type Parameters

• **KRoleContainer** *extends* `"hive"`

#### Parameters

##### category

`KRoleContainer`

role category to retrieve

#### Returns

`Iterable`\<[`TRoleContainerKeyToValueMap`](../type-aliases/TRoleContainerKeyToValueMap)\[`KRoleContainer`\], `any`, `any`\>

Iterable of all roles for the given role category

#### Example

```ts
for(const role of operation.roles("hive"))
  if (role.level === "memo")
    role.set(myKey);
  else
    role.add(myKey);
```

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:137](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L137)

***

### createFor()

> `static` **createFor**(`chain`, `account`): `Promise`\<[`AccountAuthorityUpdateOperation`](./AccountAuthorityUpdateOperation)\>

Creates an instance of AccountAuthorityUpdateOperation with all supported roles pre-initialized for the given account.

#### Parameters

##### chain

[`IHiveChainInterface`](../interfaces/IHiveChainInterface)

chain interface required for online user roles parsing

##### account

`string`

account we will operate on

#### Returns

`Promise`\<[`AccountAuthorityUpdateOperation`](./AccountAuthorityUpdateOperation)\>

initialized account authority update operation

#### Defined in

[wasm/lib/detailed/complex\_operations/account\_update.ts:73](https://gitlab.syncad.com/hive/wax/-/blob/85fd5270526c5a18b82df1989bfd5ab402e6c9b5/ts/wasm/lib/detailed/complex_operations/account_update.ts#L73)
