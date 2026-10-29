[@hiveio/wax](../globals) / create\_claimed\_account

# Interface: create\_claimed\_account

Defined in: wasm/lib/proto/create\_claimed\_account.ts:14

The operation create_claimed_account_operation may be used by the user who has the token.
Pending claimed accounts (see claim_account_operation).
After executing the operation create_claimed_account_operation, a new account is created.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/23_create_claimed_account.md?ref_type=heads

## Properties

### active

> **active**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:29

#### Param

**active**

***

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:16

#### Param

**creator**

An account who create a new account.

***

### extensions

> **extensions**: [`future_extensions`](./future_extensions)[]

Defined in: wasm/lib/proto/create\_claimed\_account.ts:41

#### Param

**extensions**

Not currently used.

***

### json\_metadata

> **json\_metadata**: `string`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:39

#### Param

**json\_metadata**

Json string.

***

### memo\_key

> **memo\_key**: `string`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:37

#### Param

**memo\_key**

***

### new\_account\_name

> **new\_account\_name**: `string`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:23

#### Param

**new\_account\_name**

Account name.
                                   Valid account name may consist of many parts separated by a dot,
                                   total may have up to 16 characters, parts have to start from a letter,
                                   may be followed by numbers, or "-".

***

### owner

> **owner**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:25

#### Param

**owner**

***

### posting

> **posting**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/create\_claimed\_account.ts:33

#### Param

**posting**
