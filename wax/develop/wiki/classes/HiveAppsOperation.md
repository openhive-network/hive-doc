[@hiveio/wax](../globals) / HiveAppsOperation

# Abstract Class: HiveAppsOperation\<ChildT, BodyT\>

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:7](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L7)

## Extends

- [`OperationBase`](./OperationBase)

## Extended by

- [`CommunityOperation`](./CommunityOperation)
- [`FollowOperation`](./FollowOperation)
- [`ResourceCreditsOperation`](./ResourceCreditsOperation)

## Type Parameters

### ChildT

`ChildT` *extends* `HiveAppsOperation`\<`any`, `BodyT`\>

### BodyT

`BodyT` *extends* `object` = `object`

## Constructors

### Constructor

> **new HiveAppsOperation**\<`ChildT`, `BodyT`\>(): `HiveAppsOperation`\<`ChildT`, `BodyT`\>

#### Returns

`HiveAppsOperation`\<`ChildT`, `BodyT`\>

#### Inherited from

[`OperationBase`](./OperationBase).[`constructor`](./OperationBase#constructor)

## Properties

### body

> `protected` **body**: `BodyT`[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

***

### id

> `abstract` `protected` `readonly` **id**: `string`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L20)

Id of your custom hive apps operation

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/ad138c1321357120995b72459cde906821a1033a/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths?`): `ChildT`

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

`ChildT`

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

#### Overrides

[`OperationBase`](./OperationBase).[`finalize`](./OperationBase#finalize)
