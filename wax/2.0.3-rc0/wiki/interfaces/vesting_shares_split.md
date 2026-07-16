[@hiveio/wax](../globals) / vesting\_shares\_split

# Interface: vesting\_shares\_split

Related to hardfork 1.
Generated for every account with nonzero vesting balance.
Note: due to too small precision of VESTS asset it was increased by 6 digits, meaning all underlying
amounts had to be multiplied by million.s

## Properties

### owner

> **owner**: `string`

#### Param

affected account (source of vesting_shares_before_split and receiver of vesting_shares_after_split)

#### Defined in

wasm/lib/proto/vesting\_shares\_split.ts:14

***

### vesting\_shares\_after\_split

> **vesting\_shares\_after\_split**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) balance after split

#### Defined in

wasm/lib/proto/vesting\_shares\_split.ts:20

***

### vesting\_shares\_before\_split

> **vesting\_shares\_before\_split**: `undefined` \| [`asset`](./asset)

#### Param

(VESTS) balance before split

#### Defined in

wasm/lib/proto/vesting\_shares\_split.ts:16
