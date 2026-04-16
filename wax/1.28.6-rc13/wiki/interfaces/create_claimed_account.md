[@hiveio/wax](../globals) / create\_claimed\_account

# Interface: create\_claimed\_account

The operation create_claimed_account_operation may be used by the user who has the token.
Pending claimed accounts (see claim_account_operation).
After executing the operation create_claimed_account_operation, a new account is created.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/23_create_claimed_account.md?ref_type=heads

## Properties

### active

> **active**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:29

***

### creator

> **creator**: `string`

#### Param

An account who create a new account.

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:16

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

#### Param

Not currently used.

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:41

***

### json\_metadata

> **json\_metadata**: `string`

#### Param

Json string.

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:39

***

### memo\_key

> **memo\_key**: `string`

#### Param

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:37

***

### new\_account\_name

> **new\_account\_name**: `string`

#### Param

Account name.
                                   Valid account name may consist of many parts separated by a dot,
                                   total may have up to 16 characters, parts have to start from a letter,
                                   may be followed by numbers, or “-“.

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:23

***

### owner

> **owner**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:25

***

### posting

> **posting**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/create\_claimed\_account.ts:33
