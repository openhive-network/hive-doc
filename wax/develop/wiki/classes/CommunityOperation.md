[@hiveio/wax](../globals) / CommunityOperation

# Class: CommunityOperation

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:120](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L120)

## Extends

- [`HiveAppsOperation`](./HiveAppsOperation)\<`CommunityOperation`\>

## Constructors

### Constructor

> **new CommunityOperation**(): `CommunityOperation`

#### Returns

`CommunityOperation`

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`constructor`](./HiveAppsOperation#constructor)

## Properties

### body

> `protected` **body**: `object`[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`body`](./HiveAppsOperation#body)

***

### id

> `protected` `readonly` **id**: `"community"` = `"community"`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:121](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L121)

Id of your custom hive apps operation

#### Overrides

[`HiveAppsOperation`](./HiveAppsOperation).[`id`](./HiveAppsOperation#id)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`ops`](./HiveAppsOperation#ops)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths?`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

`string` \| `string`[]

required posting authorities (can be an account name)

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

`CommunityOperation`

itself

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`authorize`](./HiveAppsOperation#authorize)

***

### finalize()

> **finalize**(`_sink`): `Iterable`\<[`operation`](../interfaces/operation)\>

Defined in: [wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)

**`Internal`**

#### Parameters

##### \_sink

[`IOperationSink`](../interfaces/IOperationSink)

#### Returns

`Iterable`\<[`operation`](../interfaces/operation)\>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`finalize`](./HiveAppsOperation#finalize)

***

### flagPost()

> **flagPost**(`community`, `account`, `permlink`, `notes`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:144](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L144)

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

`CommunityOperation`

itself

***

### mutePost()

> **mutePost**(`community`, `account`, `permlink`, `notes`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:319](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L319)

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

`CommunityOperation`

itself

***

### pinPost()

> **pinPost**(`community`, `account`, `permlink`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:247](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L247)

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

`CommunityOperation`

itself

***

### setRole()

> **setRole**(`community`, `account`, `role`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:167](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L167)

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

`CommunityOperation`

itself

***

### setUserTitle()

> **setUserTitle**(`community`, `account`, `title`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:189](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L189)

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

`CommunityOperation`

itself

***

### subscribe()

> **subscribe**(`community`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:209](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L209)

Subscribes to given community

#### Parameters

##### community

`string`

target community

#### Returns

`CommunityOperation`

itself

***

### unmutePost()

> **unmutePost**(`community`, `account`, `permlink`, `notes`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:343](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L343)

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

`CommunityOperation`

itself

***

### unpinPost()

> **unpinPost**(`community`, `account`, `permlink`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:269](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L269)

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

`CommunityOperation`

itself

***

### unsubscribe()

> **unsubscribe**(`community`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:227](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L227)

Unsubscribes from given community

#### Parameters

##### community

`string`

target community

#### Returns

`CommunityOperation`

itself

***

### updateProps()

> **updateProps**(`community`, `props`): `CommunityOperation`

Defined in: [wasm/lib/detailed/hive\_apps\_operations/community.ts:290](https://gitlab.syncad.com/hive/wax/-/blob/41dd38f2e2e1da6af90684938b2e4bef0bd93939/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L290)

Updates props for the given community

#### Parameters

##### community

`string`

target community

##### props

[`ICommunityProps`](../interfaces/ICommunityProps)

community props

#### Returns

`CommunityOperation`

itself
