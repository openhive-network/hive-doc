[@hiveio/wax](../globals) / hardfork\_hive

# Interface: hardfork\_hive

Related to hardfork 23 (HIVE inception hardfork).
Generated for every account that did not receive HIVE airdrop.

## Properties

### account

> **account**: `string`

#### Param

account excluded from airdrop (source of amounts for airdrop)

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:12

***

### hbd\_transferred

> **hbd\_transferred**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) part of airdrop to treasury (sourced from various HBD balances on account)

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:18

***

### hive\_transferred

> **hive\_transferred**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) part of airdrop to treasury (sourced from various HIVE balances on account)

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:22

***

### other\_affected\_accounts

> **other\_affected\_accounts**: `string`[]

#### Param

delegatees that lost delegations from account - filled before pre notification

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:16

***

### total\_hive\_from\_vests

> **total\_hive\_from\_vests**: `undefined` \| [`asset`](./asset)

#### Param

(HIVE) part of airdrop to treasury (sourced from conversion of vests_converted)

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:30

***

### treasury

> **treasury**: `string`

#### Param

treasury that received airdrop instead of account (receiver of funds)

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:14

***

### vests\_converted

> **vests\_converted**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) sum of all sources of VESTS on account

#### Defined in

wasm/lib/proto/hardfork\_hive.ts:26
