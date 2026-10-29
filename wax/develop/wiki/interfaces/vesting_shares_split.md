[@hiveio/wax](../globals) / vesting\_shares\_split

# Interface: vesting\_shares\_split

Defined in: wasm/lib/proto/vesting\_shares\_split.ts:12

Related to hardfork 1.
Generated for every account with nonzero vesting balance.
Note: due to too small precision of VESTS asset it was increased by 6 digits, meaning all underlying
amounts had to be multiplied by million.s

## Properties

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/vesting\_shares\_split.ts:14

#### Param

**owner**

affected account (source of vesting_shares_before_split and receiver of vesting_shares_after_split)

***

### vesting\_shares\_after\_split

> **vesting\_shares\_after\_split**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/vesting\_shares\_split.ts:20

#### Param

**vesting\_shares\_after\_split**

(VESTS) balance after split

***

### vesting\_shares\_before\_split

> **vesting\_shares\_before\_split**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/vesting\_shares\_split.ts:16

#### Param

**vesting\_shares\_before\_split**

(VESTS) balance before split
