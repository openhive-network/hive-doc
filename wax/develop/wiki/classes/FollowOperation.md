[@hiveio/wax](../globals) / FollowOperation

# Class: FollowOperation

## Extends

- [`HiveAppsOperation`](./HiveAppsOperation)\<[`FollowOperation`](./FollowOperation)\>

## Constructors

### new FollowOperation()

> **new FollowOperation**(): [`FollowOperation`](./FollowOperation)

#### Returns

[`FollowOperation`](./FollowOperation)

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`constructor`](./HiveAppsOperation#constructors)

## Properties

### body

> `protected` **body**: `object`[] = `[]`

Object bodies to stringify in the final hive apps operation form - <i>Stage</i>

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`body`](./HiveAppsOperation#body)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:13](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L13)

***

### id

> `protected` `readonly` **id**: `"follow"` = `"follow"`

Id of your custom hive apps operation

#### Overrides

[`HiveAppsOperation`](./HiveAppsOperation).[`id`](./HiveAppsOperation#id)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L50)

***

### ops

> `protected` **ops**: [`operation`](../interfaces/operation)[] = `[]`

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`ops`](./HiveAppsOperation#ops)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L22)

## Methods

### authorize()

> **authorize**(`requiredPostingAuths`, `requiredAuths`?): [`FollowOperation`](./FollowOperation)

Authorizes the currently staged hive apps operation, commits it to saved body and clears the stage

#### Parameters

##### requiredPostingAuths

required posting authorities (can be an account name)

`string` | `string`[]

##### requiredAuths?

`string`[] = `[]`

required authorities (defaults to the empty array)

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Inherited from

[`HiveAppsOperation`](./HiveAppsOperation).[`authorize`](./HiveAppsOperation#authorize)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:32](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L32)

***

### blacklistBlog()

> **blacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to blacklist given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be blacklisted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:150](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L150)

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

[wasm/lib/detailed/hive\_apps\_operations/factory.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/factory.ts#L59)

***

### followBlacklistBlog()

> **followBlacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to follow blacklist of given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to follow blacklisted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:178](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L178)

***

### followBlog()

> **followBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to follow specified list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               Also it will be the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be followed

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:80](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L80)

***

### followMutedBlog()

> **followMutedBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to follow muted of given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to follow muted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:234](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L234)

***

### muteBlog()

> **muteBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to mute given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be muted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:108](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L108)

***

### reblog()

> **reblog**(`workingAccount`, `author`, `permlink`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to reblog specified post.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               Also it will be the account which reblogs given post (aka account)

##### author

`string`

account name of the author of the given post

##### permlink

`string`

permlink of the given post

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:303](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L303)

***

### resetAllBlog()

> **resetAllBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to reset all lists of given blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to reset the lists

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:262](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L262)

***

### resetBlacklistBlog()

> **resetBlacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to reset blacklist list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to reset the blacklist list

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:136](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L136)

***

### resetBlogList()

> **resetBlogList**(`action`, `workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to push operation to remove all matching entries between workingAccount (follower) and specified following blog accounts.
Scope of clear operation can be specfied by action parameter to point only blog, mute or both entries.

#### Parameters

##### action

[`EFollowBlogAction`](../enumerations/EFollowBlogAction)

determines scope of entries removal

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/otherBlogs parameters (aka follower)

##### blog

`string`

the blog account to be muted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:276](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L276)

***

### resetFollowBlacklistBlog()

> **resetFollowBlacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to reset follow blacklist list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to reset the follow blacklist list

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:164](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L164)

***

### resetFollowMutedBlog()

> **resetFollowMutedBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to reset follow blacklist list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to reset the follow blacklist list

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:220](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L220)

***

### unblacklistBlog()

> **unblacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to unblacklist given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be unblacklisted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:192](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L192)

***

### unfollowBlacklistBlog()

> **unfollowBlacklistBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to unfollow blacklist of given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to unfollow blacklisted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:206](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L206)

***

### unfollowBlog()

> **unfollowBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Unfollows / unmutes given blog

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               Also it will be the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be unfollowed

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:94](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L94)

***

### unfollowMutedBlog()

> **unfollowMutedBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Allows to generate operation to unfollow muted of given list of blog accounts.

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to unfollow muted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:248](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L248)

***

### unmuteBlog()

> **unmuteBlog**(`workingAccount`, `blog`, ...`otherBlogs`): [`FollowOperation`](./FollowOperation)

Unfollows / unmutes given blog

#### Parameters

##### workingAccount

`string`

The account which has to authorize transaction.
                               This is the account which follows the ones specified by the blog/other_blogs parameters (aka follower)

##### blog

`string`

the blog account to be unmuted

##### otherBlogs

...`string`[]

optional list of other blog accounts to be concatenated and build single list

#### Returns

[`FollowOperation`](./FollowOperation)

itself

#### Defined in

[wasm/lib/detailed/hive\_apps\_operations/follow.ts:122](https://gitlab.syncad.com/hive/wax/-/blob/a42fdb500bc14c06485fccd0dc833631ac25faef/ts/wasm/lib/detailed/hive_apps_operations/follow.ts#L122)
