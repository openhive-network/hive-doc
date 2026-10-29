[@hiveio/wax](../globals) / hardfork\_hive

# Interface: hardfork\_hive

Defined in: wasm/lib/proto/hardfork\_hive.ts:10

Related to hardfork 23 (HIVE inception hardfork).
Generated for every account that did not receive HIVE airdrop.

## Properties

### account

> **account**: `string`

Defined in: wasm/lib/proto/hardfork\_hive.ts:12

#### Param

**account**

account excluded from airdrop (source of amounts for airdrop)

***

### hbd\_transferred

> **hbd\_transferred**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive.ts:18

#### Param

**hbd\_transferred**

(HBD) part of airdrop to treasury (sourced from various HBD balances on account)

***

### hive\_transferred

> **hive\_transferred**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive.ts:22

#### Param

**hive\_transferred**

(HIVE) part of airdrop to treasury (sourced from various HIVE balances on account)

***

### other\_affected\_accounts

> **other\_affected\_accounts**: `string`[]

Defined in: wasm/lib/proto/hardfork\_hive.ts:16

#### Param

**other\_affected\_accounts**

delegatees that lost delegations from account - filled before pre notification

***

### total\_hive\_from\_vests

> **total\_hive\_from\_vests**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive.ts:30

#### Param

**total\_hive\_from\_vests**

(HIVE) part of airdrop to treasury (sourced from conversion of vests_converted)

***

### treasury

> **treasury**: `string`

Defined in: wasm/lib/proto/hardfork\_hive.ts:14

#### Param

**treasury**

treasury that received airdrop instead of account (receiver of funds)

***

### vests\_converted

> **vests\_converted**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/hardfork\_hive.ts:26

#### Param

**vests\_converted**

(VESTS) sum of all sources of VESTS on account
