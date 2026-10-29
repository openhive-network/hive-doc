[@hiveio/wax](../globals) / account\_create

# Interface: account\_create

Defined in: wasm/lib/proto/account\_create.ts:14

A new account may be created only by an existing account.
The account that creates a new account pays a fee.
The fee amount is set by the witnesses.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/09_account_create.md?ref_type=heads&plain=0&blame=1#2-parameters

## Properties

### active

> **active**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/account\_create.ts:32

#### Param

**active**

***

### creator

> **creator**: `string`

Defined in: wasm/lib/proto/account\_create.ts:20

#### Param

**creator**

An account that creates a new account.

***

### fee

> **fee**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/account\_create.ts:16

#### Param

**fee**

Paid by creator. The witnesses decide the amount of the fee. Now, it is 3 HIVE.

***

### json\_metadata

> **json\_metadata**: `string`

Defined in: wasm/lib/proto/account\_create.ts:42

#### Param

**json\_metadata**

***

### memo\_key

> **memo\_key**: `string`

Defined in: wasm/lib/proto/account\_create.ts:40

#### Param

**memo\_key**

Not authority, public memo key.

***

### new\_account\_name

> **new\_account\_name**: `string`

Defined in: wasm/lib/proto/account\_create.ts:26

#### Param

**new\_account\_name**

Valid account name may consist of many parts separated by a dot,
                                 total may have up to 16 characters, parts have to start from a letter,
                                 may be followed by numbers, or '-'.

***

### owner

> **owner**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/account\_create.ts:28

#### Param

**owner**

***

### posting

> **posting**: [`authority`](./authority) \| `undefined`

Defined in: wasm/lib/proto/account\_create.ts:36

#### Param

**posting**
