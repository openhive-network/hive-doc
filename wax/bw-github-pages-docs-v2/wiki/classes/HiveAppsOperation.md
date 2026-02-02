[@hiveio/wax](../globals) / HiveAppsOperation

# Class: `abstract` HiveAppsOperation\<ChildT, BodyT\>

## Extends

- [`OperationBase`](./OperationBase)

## Extended by

- [`CommunityOperation`](./CommunityOperation)
- [`FollowOperation`](./FollowOperation)
- [`ResourceCreditsOperation`](./ResourceCreditsOperation)

## Type Parameters

• **ChildT** *extends* [`HiveAppsOperation`](./HiveAppsOperation)\<`any`, `BodyT`\>

• **BodyT** *extends* `object` = `object`

## Constructors

### new HiveAppsOperation()

> **new HiveAppsOperation**\<`ChildT`, `BodyT`\>(): [`HiveAppsOperation`](./HiveAppsOperation)\<`ChildT`, `BodyT`\>

#### Returns

[`HiveAppsOperation`](./HiveAppsOperation)\<`ChildT`, `BodyT`\>

#### Inherited from

[`OperationBase`](./OperationBase).[`constructor`](./OperationBase#constructors)

## Properties

### body

> `protected` **body**: `BodyT`[] = `[]`

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

***

### id

> `abstract` `protected` `readonly` **id**: `string`

Id of your custom hive apps operation

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:20](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L20)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths`?): `ChildT`

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

required posting authorities (can be an account name)

`string` | `string`[]

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

`ChildT`

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

***

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation), `any`, `any`\>

#### Overrides

[`OperationBase`](./OperationBase).[`finalize`](./OperationBase#finalize)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/2765bf30e974bf76e09d2574c0ad71106b64f92b/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)
