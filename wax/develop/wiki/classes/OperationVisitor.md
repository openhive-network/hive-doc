[@hiveio/wax](../globals) / OperationVisitor

# Class: OperationVisitor\<R\>

Defined in: [wasm/lib/detailed/visitor.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L22)

## Extended by

- [`EncryptionVisitor`](./EncryptionVisitor)

## Type Parameters

### R

`R` = `void`

## Implements

- [`TOperationVisitor`](../type-aliases/TOperationVisitor)\<`R`\>

## Constructors

### Constructor

> **new OperationVisitor**\<`R`\>(): `OperationVisitor`\<`R`\>

#### Returns

`OperationVisitor`\<`R`\>

## Methods

### accept()

> `readonly` **accept**(`op`): [`NoOverride`](../type-aliases/NoOverride) & `void` \| `R`

Defined in: [wasm/lib/detailed/visitor.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L26)

You should not override this method

#### Parameters

##### op

[`operation`](../interfaces/operation)

#### Returns

[`NoOverride`](../type-aliases/NoOverride) & `void` \| `R`

***

### account\_create\_operation()?

> `optional` **account\_create\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:42](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L42)

#### Parameters

##### op

[`account_create`](../interfaces/account_create)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_create_operation`](../interfaces/operation#account_create_operation)

***

### account\_create\_with\_delegation\_operation()?

> `optional` **account\_create\_with\_delegation\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:71](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L71)

#### Parameters

##### op

[`account_create_with_delegation`](../interfaces/account_create_with_delegation)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_create_with_delegation_operation`](../interfaces/operation#account_create_with_delegation_operation)

***

### account\_update\_operation()?

> `optional` **account\_update\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:43](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L43)

#### Parameters

##### op

[`account_update`](../interfaces/account_update)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_update_operation`](../interfaces/operation#account_update_operation)

***

### account\_update2\_operation()?

> `optional` **account\_update2\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:73](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L73)

#### Parameters

##### op

[`account_update2`](../interfaces/account_update2)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_update2_operation`](../interfaces/operation#account_update2_operation)

***

### account\_witness\_proxy\_operation()?

> `optional` **account\_witness\_proxy\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L46)

#### Parameters

##### op

[`account_witness_proxy`](../interfaces/account_witness_proxy)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_witness_proxy_operation`](../interfaces/operation#account_witness_proxy_operation)

***

### account\_witness\_vote\_operation()?

> `optional` **account\_witness\_vote\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L45)

#### Parameters

##### op

[`account_witness_vote`](../interfaces/account_witness_vote)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`account_witness_vote_operation`](../interfaces/operation#account_witness_vote_operation)

***

### cancel\_transfer\_from\_savings\_operation()?

> `optional` **cancel\_transfer\_from\_savings\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:67](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L67)

#### Parameters

##### op

[`cancel_transfer_from_savings`](../interfaces/cancel_transfer_from_savings)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`cancel_transfer_from_savings_operation`](../interfaces/operation#cancel_transfer_from_savings_operation)

***

### change\_recovery\_account\_operation()?

> `optional` **change\_recovery\_account\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L59)

#### Parameters

##### op

[`change_recovery_account`](../interfaces/change_recovery_account)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`change_recovery_account_operation`](../interfaces/operation#change_recovery_account_operation)

***

### claim\_account\_operation()?

> `optional` **claim\_account\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:55](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L55)

#### Parameters

##### op

[`claim_account`](../interfaces/claim_account)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`claim_account_operation`](../interfaces/operation#claim_account_operation)

***

### claim\_reward\_balance\_operation()?

> `optional` **claim\_reward\_balance\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:69](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L69)

#### Parameters

##### op

[`claim_reward_balance`](../interfaces/claim_reward_balance)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`claim_reward_balance_operation`](../interfaces/operation#claim_reward_balance_operation)

***

### collateralized\_convert\_operation()?

> `optional` **collateralized\_convert\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L78)

#### Parameters

##### op

[`collateralized_convert`](../interfaces/collateralized_convert)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`collateralized_convert_operation`](../interfaces/operation#collateralized_convert_operation)

***

### comment\_operation()?

> `optional` **comment\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:34](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L34)

#### Parameters

##### op

[`comment`](../interfaces/comment)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`comment_operation`](../interfaces/operation#comment_operation)

***

### comment\_options\_operation()?

> `optional` **comment\_options\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:52](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L52)

#### Parameters

##### op

[`comment_options`](../interfaces/comment_options)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`comment_options_operation`](../interfaces/operation#comment_options_operation)

***

### convert\_operation()?

> `optional` **convert\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:41](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L41)

#### Parameters

##### op

[`convert`](../interfaces/convert)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`convert_operation`](../interfaces/operation#convert_operation)

***

### create\_claimed\_account\_operation()?

> `optional` **create\_claimed\_account\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:56](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L56)

#### Parameters

##### op

[`create_claimed_account`](../interfaces/create_claimed_account)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`create_claimed_account_operation`](../interfaces/operation#create_claimed_account_operation)

***

### create\_proposal\_operation()?

> `optional` **create\_proposal\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:74](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L74)

#### Parameters

##### op

[`create_proposal`](../interfaces/create_proposal)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`create_proposal_operation`](../interfaces/operation#create_proposal_operation)

***

### custom\_json\_operation()?

> `optional` **custom\_json\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:51](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L51)

#### Parameters

##### op

[`custom_json`](../interfaces/custom_json)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`custom_json_operation`](../interfaces/operation#custom_json_operation)

***

### custom\_operation()?

> `optional` **custom\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:48](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L48)

#### Parameters

##### op

[`custom`](../interfaces/custom)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`custom_operation`](../interfaces/operation#custom_operation)

***

### decline\_voting\_rights\_operation()?

> `optional` **decline\_voting\_rights\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L68)

#### Parameters

##### op

[`decline_voting_rights`](../interfaces/decline_voting_rights)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`decline_voting_rights_operation`](../interfaces/operation#decline_voting_rights_operation)

***

### delegate\_vesting\_shares\_operation()?

> `optional` **delegate\_vesting\_shares\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:70](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L70)

#### Parameters

##### op

[`delegate_vesting_shares`](../interfaces/delegate_vesting_shares)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`delegate_vesting_shares_operation`](../interfaces/operation#delegate_vesting_shares_operation)

***

### delete\_comment\_operation()?

> `optional` **delete\_comment\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L50)

#### Parameters

##### op

[`delete_comment`](../interfaces/delete_comment)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`delete_comment_operation`](../interfaces/operation#delete_comment_operation)

***

### escrow\_approve\_operation()?

> `optional` **escrow\_approve\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L64)

#### Parameters

##### op

[`escrow_approve`](../interfaces/escrow_approve)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`escrow_approve_operation`](../interfaces/operation#escrow_approve_operation)

***

### escrow\_dispute\_operation()?

> `optional` **escrow\_dispute\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:61](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L61)

#### Parameters

##### op

[`escrow_dispute`](../interfaces/escrow_dispute)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`escrow_dispute_operation`](../interfaces/operation#escrow_dispute_operation)

***

### escrow\_release\_operation()?

> `optional` **escrow\_release\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:62](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L62)

#### Parameters

##### op

[`escrow_release`](../interfaces/escrow_release)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`escrow_release_operation`](../interfaces/operation#escrow_release_operation)

***

### escrow\_transfer\_operation()?

> `optional` **escrow\_transfer\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:60](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L60)

#### Parameters

##### op

[`escrow_transfer`](../interfaces/escrow_transfer)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`escrow_transfer_operation`](../interfaces/operation#escrow_transfer_operation)

***

### feed\_publish\_operation()?

> `optional` **feed\_publish\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L40)

#### Parameters

##### op

[`feed_publish`](../interfaces/feed_publish)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`feed_publish_operation`](../interfaces/operation#feed_publish_operation)

***

### limit\_order\_cancel\_operation()?

> `optional` **limit\_order\_cancel\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:39](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L39)

#### Parameters

##### op

[`limit_order_cancel`](../interfaces/limit_order_cancel)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`limit_order_cancel_operation`](../interfaces/operation#limit_order_cancel_operation)

***

### limit\_order\_create\_operation()?

> `optional` **limit\_order\_create\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L38)

#### Parameters

##### op

[`limit_order_create`](../interfaces/limit_order_create)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`limit_order_create_operation`](../interfaces/operation#limit_order_create_operation)

***

### limit\_order\_create2\_operation()?

> `optional` **limit\_order\_create2\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L54)

#### Parameters

##### op

[`limit_order_create2`](../interfaces/limit_order_create2)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`limit_order_create2_operation`](../interfaces/operation#limit_order_create2_operation)

***

### pow\_operation()?

> `optional` **pow\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:47](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L47)

#### Parameters

##### op

[`pow`](../interfaces/pow)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`pow_operation`](../interfaces/operation#pow_operation)

***

### pow2\_operation()?

> `optional` **pow2\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:63](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L63)

#### Parameters

##### op

[`pow2`](../interfaces/pow2)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`pow2_operation`](../interfaces/operation#pow2_operation)

***

### recover\_account\_operation()?

> `optional` **recover\_account\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:58](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L58)

#### Parameters

##### op

[`recover_account`](../interfaces/recover_account)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`recover_account_operation`](../interfaces/operation#recover_account_operation)

***

### recurrent\_transfer\_operation()?

> `optional` **recurrent\_transfer\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:79](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L79)

#### Parameters

##### op

[`recurrent_transfer`](../interfaces/recurrent_transfer)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`recurrent_transfer_operation`](../interfaces/operation#recurrent_transfer_operation)

***

### remove\_proposal\_operation()?

> `optional` **remove\_proposal\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L76)

#### Parameters

##### op

[`remove_proposal`](../interfaces/remove_proposal)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`remove_proposal_operation`](../interfaces/operation#remove_proposal_operation)

***

### request\_account\_recovery\_operation()?

> `optional` **request\_account\_recovery\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:57](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L57)

#### Parameters

##### op

[`request_account_recovery`](../interfaces/request_account_recovery)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`request_account_recovery_operation`](../interfaces/operation#request_account_recovery_operation)

***

### set\_withdraw\_vesting\_route\_operation()?

> `optional` **set\_withdraw\_vesting\_route\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L53)

#### Parameters

##### op

[`set_withdraw_vesting_route`](../interfaces/set_withdraw_vesting_route)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`set_withdraw_vesting_route_operation`](../interfaces/operation#set_withdraw_vesting_route_operation)

***

### transfer\_from\_savings\_operation()?

> `optional` **transfer\_from\_savings\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:66](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L66)

#### Parameters

##### op

[`transfer_from_savings`](../interfaces/transfer_from_savings)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`transfer_from_savings_operation`](../interfaces/operation#transfer_from_savings_operation)

***

### transfer\_operation()?

> `optional` **transfer\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:35](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L35)

#### Parameters

##### op

[`transfer`](../interfaces/transfer)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`transfer_operation`](../interfaces/operation#transfer_operation)

***

### transfer\_to\_savings\_operation()?

> `optional` **transfer\_to\_savings\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:65](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L65)

#### Parameters

##### op

[`transfer_to_savings`](../interfaces/transfer_to_savings)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`transfer_to_savings_operation`](../interfaces/operation#transfer_to_savings_operation)

***

### transfer\_to\_vesting\_operation()?

> `optional` **transfer\_to\_vesting\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L36)

#### Parameters

##### op

[`transfer_to_vesting`](../interfaces/transfer_to_vesting)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`transfer_to_vesting_operation`](../interfaces/operation#transfer_to_vesting_operation)

***

### update\_proposal\_operation()?

> `optional` **update\_proposal\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:77](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L77)

#### Parameters

##### op

[`update_proposal`](../interfaces/update_proposal)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`update_proposal_operation`](../interfaces/operation#update_proposal_operation)

***

### update\_proposal\_votes\_operation()?

> `optional` **update\_proposal\_votes\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:75](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L75)

#### Parameters

##### op

[`update_proposal_votes`](../interfaces/update_proposal_votes)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`update_proposal_votes_operation`](../interfaces/operation#update_proposal_votes_operation)

***

### vote\_operation()?

> `optional` **vote\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L33)

#### Parameters

##### op

[`vote`](../interfaces/vote)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`vote_operation`](../interfaces/operation#vote_operation)

***

### withdraw\_vesting\_operation()?

> `optional` **withdraw\_vesting\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L37)

#### Parameters

##### op

[`withdraw_vesting`](../interfaces/withdraw_vesting)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`withdraw_vesting_operation`](../interfaces/operation#withdraw_vesting_operation)

***

### witness\_block\_approve\_operation()?

> `optional` **witness\_block\_approve\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:49](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L49)

#### Parameters

##### op

[`witness_block_approve`](../interfaces/witness_block_approve)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`witness_block_approve_operation`](../interfaces/operation#witness_block_approve_operation)

***

### witness\_set\_properties\_operation()?

> `optional` **witness\_set\_properties\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L72)

#### Parameters

##### op

[`witness_set_properties`](../interfaces/witness_set_properties)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`witness_set_properties_operation`](../interfaces/operation#witness_set_properties_operation)

***

### witness\_update\_operation()?

> `optional` **witness\_update\_operation**(`op`): `R`

Defined in: [wasm/lib/detailed/visitor.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/3d827177c4112afa560e8adbccbf055964c990b2/ts/wasm/lib/detailed/visitor.ts#L44)

#### Parameters

##### op

[`witness_update`](../interfaces/witness_update)

#### Returns

`R`

#### Implementation of

[`operation`](../interfaces/operation).[`witness_update_operation`](../interfaces/operation#witness_update_operation)
