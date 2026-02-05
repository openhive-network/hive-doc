[@hiveio/wax](../globals) / CommunityOperation

# Class: CommunityOperation

## Extends

- [`HiveAppsOperation`](./HiveAppsOperation)\<[`CommunityOperation`](./CommunityOperation)\>

## Constructors

### new CommunityOperation()

> **new CommunityOperation**(): [`CommunityOperation`](./CommunityOperation)

#### Returns

[`CommunityOperation`](./CommunityOperation)

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`constructor`](./HiveAppsOperation#constructors)

## Properties

### body

> `protected` **body**: `object`[] = `[]`

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`body`](./HiveAppsOperation#body)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

***

### id

> `protected` `readonly` **id**: `"community"` = `"community"`

Id of your custom hive apps operation

#### Overrides

[`HiveAppsOperation`](./HiveAppsOperation).[`id`](./HiveAppsOperation#id)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L121)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`ops`](./HiveAppsOperation#ops)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths`?): [`CommunityOperation`](./CommunityOperation)

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

required posting authorities (can be an account name)

`string` | `string`[]

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`authorize`](./HiveAppsOperation#authorize)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

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

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)

***

### flagPost()

> **flagPost**(`community`, `account`, `permlink`, `notes`): [`CommunityOperation`](./CommunityOperation)

Flags post on given community

#### Parameters

##### community

`string`

target community

##### account

`string`

author of the post to flag

##### permlink

`string`

post permlink to flag

##### notes

`string`

notes on the flag

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:144](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L144)

***

### mutePost()

> **mutePost**(`community`, `account`, `permlink`, `notes`): [`CommunityOperation`](./CommunityOperation)

Mutes post on given community

#### Parameters

##### community

`string`

target community

##### account

`string`

author of the post to mute

##### permlink

`string`

post permlink to mute

##### notes

`string`

notes on the mute

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:319](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L319)

***

### pinPost()

> **pinPost**(`community`, `account`, `permlink`): [`CommunityOperation`](./CommunityOperation)

Pins given post on the community page

#### Parameters

##### community

`string`

target community

##### account

`string`

author of the post to pin

##### permlink

`string`

post permlink to pin

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:247](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L247)

***

### setRole()

> **setRole**(`community`, `account`, `role`): [`CommunityOperation`](./CommunityOperation)

Updates the role for a community member

#### Parameters

##### community

`string`

target community

##### account

`string`

community member update the role

##### role

[`EAvailableCommunityRoles`](../enumerations/EAvailableCommunityRoles)

target role to apply to the community member

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:167](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L167)

***

### setUserTitle()

> **setUserTitle**(`community`, `account`, `title`): [`CommunityOperation`](./CommunityOperation)

Sets title on the user

#### Parameters

##### community

`string`

target community

##### account

`string`

account to change the title

##### title

`string`

new account title

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:189](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L189)

***

### subscribe()

> **subscribe**(`community`): [`CommunityOperation`](./CommunityOperation)

Subscribes to given community

#### Parameters

##### community

`string`

target community

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:209](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L209)

***

### unmutePost()

> **unmutePost**(`community`, `account`, `permlink`, `notes`): [`CommunityOperation`](./CommunityOperation)

Unmutes post on given community

#### Parameters

##### community

`string`

target community

##### account

`string`

author of the post to unmute

##### permlink

`string`

post permlink to unmute

##### notes

`string`

notes on the unmute

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:343](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L343)

***

### unpinPost()

> **unpinPost**(`community`, `account`, `permlink`): [`CommunityOperation`](./CommunityOperation)

Unpins given post from the community page

#### Parameters

##### community

`string`

target community

##### account

`string`

author of the post to pin

##### permlink

`string`

post permlink to pin

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:269](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L269)

***

### unsubscribe()

> **unsubscribe**(`community`): [`CommunityOperation`](./CommunityOperation)

Unsubscribes from given community

#### Parameters

##### community

`string`

target community

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:227](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L227)

***

### updateProps()

> **updateProps**(`community`, `props`): [`CommunityOperation`](./CommunityOperation)

Updates props for the given community

#### Parameters

##### community

`string`

target community

##### props

[`ICommunityProps`](../interfaces/ICommunityProps)

community props

#### Returns

[`CommunityOperation`](./CommunityOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:290](https://gitlab.syncad.com/hive/wax/-/blob/a3ee40eb64ee238318a1f50f983c200901c6b4e1/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L290)
