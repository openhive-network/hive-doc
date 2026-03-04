[@hiveio/wax](../globals) / legacy\_chain\_properties

# Interface: legacy\_chain\_properties

Witnesses must vote on how to set certain chain properties to ensure a smooth
and well functioning network.  Any time owner is in the active set of witnesses these
properties will be used to control the blockchain configuration.

## Properties

### account\_creation\_fee

> **account\_creation\_fee**: `undefined` \| [`asset`](./asset)

#### Param

This fee, paid in HIVE, is converted into VESTS for the new account.
                                      Accounts without vesting shares cannot earn usage rations and therefore are powerless.
                                      This minimum fee requires all accounts to have some kind of commitment
                                      to the network that includes the ability to vote and make transactions.

#### Defined in

wasm/lib/proto/legacy\_chain\_properties.ts:18

***

### hbd\_interest\_rate

> **hbd\_interest\_rate**: `number`

#### Param

#### Defined in

wasm/lib/proto/legacy\_chain\_properties.ts:24

***

### maximum\_block\_size

> **maximum\_block\_size**: `number`

#### Param

This witnesses vote for the maximum_block_size which is used by the network to tune rate limiting and capacity.

#### Defined in

wasm/lib/proto/legacy\_chain\_properties.ts:22
