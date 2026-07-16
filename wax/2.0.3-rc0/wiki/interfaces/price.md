[@hiveio/wax](../globals) / price

# Interface: price

Represents quotation of the relative value of asset against another asset.
Similar to 'currency pair' used to determine value of currencies.

For example:
1 EUR / 1.25 USD where:
1 EUR is an asset specified as a base
1.25 USD us an asset specified as a qute

can determine value of EUR against USD.

## Properties

### base

> **base**: `undefined` \| [`asset`](./asset)

#### Param

Represents a value of the price object to be expressed relatively to quote asset.
                      Cannot have amount == 0 if you want to build valid price.

#### Defined in

wasm/lib/proto/price.ts:22

***

### quote

> **quote**: `undefined` \| [`asset`](./asset)

#### Param

represents an relative asset. Cannot have amount == 0, otherwise asertion fail.

#### Defined in

wasm/lib/proto/price.ts:26
