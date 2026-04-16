[@hiveio/wax](../globals) / account\_create

# Interface: account\_create

A new account may be created only by an existing account.
The account that creates a new account pays a fee.
The fee amount is set by the witnesses.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/09_account_create.md?ref_type=heads&plain=0&blame=1#2-parameters

## Properties

### active

> **active**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/account\_create.ts:32

***

### creator

> **creator**: `string`

#### Param

An account that creates a new account.

#### Defined in

wasm/lib/proto/account\_create.ts:20

***

### fee

> **fee**: `undefined` \| [`asset`](./asset)

#### Param

Paid by creator. The witnesses decide the amount of the fee. Now, it is 3 HIVE.

#### Defined in

wasm/lib/proto/account\_create.ts:16

***

### json\_metadata

> **json\_metadata**: `string`

#### Param

#### Defined in

wasm/lib/proto/account\_create.ts:42

***

### memo\_key

> **memo\_key**: `string`

#### Param

Not authority, public memo key.

#### Defined in

wasm/lib/proto/account\_create.ts:40

***

### new\_account\_name

> **new\_account\_name**: `string`

#### Param

Valid account name may consist of many parts separated by a dot,
                                 total may have up to 16 characters, parts have to start from a letter,
                                 may be followed by numbers, or '-'.

#### Defined in

wasm/lib/proto/account\_create.ts:26

***

### owner

> **owner**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/account\_create.ts:28

***

### posting

> **posting**: `undefined` \| [`authority`](./authority)

#### Param

#### Defined in

wasm/lib/proto/account\_create.ts:36
