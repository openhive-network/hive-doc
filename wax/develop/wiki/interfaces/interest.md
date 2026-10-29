[@hiveio/wax](../globals) / interest

# Interface: interest

Defined in: wasm/lib/proto/interest.ts:12

Related to any operation that modifies HBD liquid or savings balance (including block processing).
Generated when operation modified HBD balance and account received interest payment.
Interest is stored in related balance (liquid when liquid was modified, savings when savings was modified).
Note: since HF25 interest is not calculated nor paid on liquid balance.

## Properties

### interest

> **interest**: [`asset`](./asset) \| `undefined`

Defined in: wasm/lib/proto/interest.ts:16

#### Param

**interest**

(HBD) amount of interest paid

***

### is\_saved\_into\_hbd\_balance

> **is\_saved\_into\_hbd\_balance**: `boolean`

Defined in: wasm/lib/proto/interest.ts:20

#### Param

**is\_saved\_into\_hbd\_balance**

true when liquid balance was modified (not happening after HF25)

***

### owner

> **owner**: `string`

Defined in: wasm/lib/proto/interest.ts:14

#### Param

**owner**

user that had his HBD balance modified (receiver of interest)
