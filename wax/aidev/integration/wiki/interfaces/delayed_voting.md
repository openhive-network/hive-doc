[@hiveio/wax](../globals) / delayed\_voting

# Interface: delayed\_voting

Related to transfer_to_vesting_operation.
Generated during block processing every time part of fairly fresh VESTS becomes active part of governance vote for the account.
Note: after account receives new VESTS there is a grace period before those VESTS are accounted for when
it comes to governance vote power. This vop is generated at the end of that period.

## Properties

### voter

> **voter**: `string`

#### Param

account with fairly fresh VESTS

#### Defined in

wasm/lib/proto/delayed\_voting.ts:13

***

### votes

> **votes**: `string`

#### Param

(VESTS satoshi) new governance vote power that just activated for voter

#### Defined in

wasm/lib/proto/delayed\_voting.ts:15
