[@hiveio/wax](../globals) / ResourceCreditsOperation

# Class: ResourceCreditsOperation

Defined in: [wasm/lib/detailed/hive\_apps\_operations/rc.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L12)

## Extends

- [`HiveAppsOperation`](./HiveAppsOperation)\<`ResourceCreditsOperation`\>

## Constructors

### Constructor

> **new ResourceCreditsOperation**(): `ResourceCreditsOperation`

#### Returns

`ResourceCreditsOperation`

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`constructor`](./HiveAppsOperation#constructor)

## Properties

### body

> `protected` **body**: `object`[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`body`](./HiveAppsOperation#body)

***

### id

> `protected` `readonly` **id**: `"rc"` = `"rc"`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/rc.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L13)

Id of your custom hive apps operation

#### Overrides

[`HiveAppsOperation`](./HiveAppsOperation).[`id`](./HiveAppsOperation#id)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`ops`](./HiveAppsOperation#ops)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths?`): `ResourceCreditsOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

`string` \| `string`[]

required posting authorities (can be an account name)

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

`ResourceCreditsOperation`

itself

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`authorize`](./HiveAppsOperation#authorize)

***

### delegate()

> **delegate**(`workingAccount`, `maxRc`, `delegatee`, ...`otherDelegatees`): `ResourceCreditsOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/rc.ts:27](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L27)

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

`ResourceCreditsOperation`

itself

***

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`finalize`](./HiveAppsOperation#finalize)

***

### removeDelegation()

> **removeDelegation**(`workingAccount`, `delegatee`, ...`otherDelegatees`): `ResourceCreditsOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/rc.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/rc.ts#L53)

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

`ResourceCreditsOperation`

itself
