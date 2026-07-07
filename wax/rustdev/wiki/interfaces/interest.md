[@hiveio/wax](../globals) / interest

# Interface: interest

Related to any operation that modifies HBD liquid or savings balance (including block processing).
Generated when operation modified HBD balance and account received interest payment.
Interest is stored in related balance (liquid when liquid was modified, savings when savings was modified).
Note: since HF25 interest is not calculated nor paid on liquid balance.

## Properties

### interest

> **interest**: `undefined` \| [`asset`](./asset)

#### Param

(HBD) amount of interest paid

#### Defined in

wasm/lib/proto/interest.ts:16

***

### is\_saved\_into\_hbd\_balance

> **is\_saved\_into\_hbd\_balance**: `boolean`

#### Param

true when liquid balance was modified (not happening after HF25)

#### Defined in

wasm/lib/proto/interest.ts:20

***

### owner

> **owner**: `string`

#### Param

user that had his HBD balance modified (receiver of interest)

#### Defined in

wasm/lib/proto/interest.ts:14
