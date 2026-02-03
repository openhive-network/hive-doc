[@hiveio/wax](../globals) / ResourceCreditsOperation

# Class: ResourceCreditsOperation

## Extends

- [`HiveAppsOperation`](./HiveAppsOperation)\<[`ResourceCreditsOperation`](./ResourceCreditsOperation)\>

## Constructors

### new ResourceCreditsOperation()

> **new ResourceCreditsOperation**(): [`ResourceCreditsOperation`](./ResourceCreditsOperation)

#### Returns

[`ResourceCreditsOperation`](./ResourceCreditsOperation)

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`constructor`](./HiveAppsOperation#constructors)

## Properties

### body

> `protected` **body**: `object`[] = `[]`

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`body`](./HiveAppsOperation#body)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

***

### id

> `protected` `readonly` **id**: `"rc"` = `"rc"`

Id of your custom hive apps operation

#### Overrides

[`HiveAppsOperation`](./HiveAppsOperation).[`id`](./HiveAppsOperation#id)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/rc.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L13)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`ops`](./HiveAppsOperation#ops)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths`?): [`ResourceCreditsOperation`](./ResourceCreditsOperation)

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

required posting authorities (can be an account name)

`string` | `string`[]

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

[`ResourceCreditsOperation`](./ResourceCreditsOperation)

itself

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`authorize`](./HiveAppsOperation#authorize)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

***

### delegate()

> **delegate**(`workingAccount`, `maxRc`, `delegatee`, ...`otherDelegatees`): [`ResourceCreditsOperation`](./ResourceCreditsOperation)

Delegates resource credits to given account(s)

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               Also it will be the account which delegates resource credits (aka from)

##### maxRc

[`TNaiAssetConvertible`](../type-aliases/TNaiAssetConvertible)

maximum resource credits delegated (must pe non-negative value)

##### delegatee

`string`

target account to delegate. Remember you cannot delegate to yourself!

##### otherDelegatees

...`string`[]

optional list of other target accounts to delegate.
                                        In the standard node configuration there may be 100 delegatees at most.

#### Returns

[`ResourceCreditsOperation`](./ResourceCreditsOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/rc.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L27)

***

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`finalize`](./HiveAppsOperation#finalize)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)

***

### removeDelegation()

> **removeDelegation**(`workingAccount`, `delegatee`, ...`otherDelegatees`): [`ResourceCreditsOperation`](./ResourceCreditsOperation)

Removes resource credits delegation from given account(s)

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               Also it will be the account which delegated resource credits in the past (aka from)

##### delegatee

`string`

target account to remove the delegation from.

##### otherDelegatees

...`string`[]

optional list of other target accounts to remove the delegation from.

#### Returns

[`ResourceCreditsOperation`](./ResourceCreditsOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/rc.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/71b6f108be21d1700323d3d4958dc29cb6099ac3/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L53)
