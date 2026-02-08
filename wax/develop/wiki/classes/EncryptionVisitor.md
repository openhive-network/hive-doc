[@hiveio/wax](../globals) / EncryptionVisitor

# Class: EncryptionVisitor

## Extends

- [`OperationVisitor`](./OperationVisitor)

## Constructors

### new EncryptionVisitor()

> **new EncryptionVisitor**(`encryptionType`, `cryptographicFunction`): [`EncryptionVisitor`](./EncryptionVisitor)

#### Parameters

##### encryptionType

[`EEncryptionType`](../enumerations/EEncryptionType)

##### cryptographicFunction

[`TEncryptFn`](../type-aliases/TEncryptFn)

#### Returns

[`EncryptionVisitor`](./EncryptionVisitor)

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`constructor`](./OperationVisitor#constructors)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:12](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L12)

## Methods

### accept()

> `readonly` **accept**(`op`): [`NoOverride`](../type-aliases/NoOverride) & `void`

You should not override this method

#### Parameters

##### op

[`operation`](../interfaces/operation)

#### Returns

[`NoOverride`](../type-aliases/NoOverride) & `void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`accept`](./OperationVisitor#accept)

#### Defined in

[wasm/lib/detailed/visitor.ts:26](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L26)

***

### account\_create\_operation()?

> `optional` **account\_create\_operation**(`op`): `void`

#### Parameters

##### op

[`account_create`](../interfaces/account_create)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_create_operation`](./OperationVisitor#account_create_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:42](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L42)

***

### account\_create\_with\_delegation\_operation()?

> `optional` **account\_create\_with\_delegation\_operation**(`op`): `void`

#### Parameters

##### op

[`account_create_with_delegation`](../interfaces/account_create_with_delegation)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_create_with_delegation_operation`](./OperationVisitor#account_create_with_delegation_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:71](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L71)

***

### account\_update\_operation()?

> `optional` **account\_update\_operation**(`op`): `void`

#### Parameters

##### op

[`account_update`](../interfaces/account_update)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_update_operation`](./OperationVisitor#account_update_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:43](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L43)

***

### account\_update2\_operation()?

> `optional` **account\_update2\_operation**(`op`): `void`

#### Parameters

##### op

[`account_update2`](../interfaces/account_update2)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_update2_operation`](./OperationVisitor#account_update2_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:73](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L73)

***

### account\_witness\_proxy\_operation()?

> `optional` **account\_witness\_proxy\_operation**(`op`): `void`

#### Parameters

##### op

[`account_witness_proxy`](../interfaces/account_witness_proxy)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_witness_proxy_operation`](./OperationVisitor#account_witness_proxy_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:46](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L46)

***

### account\_witness\_vote\_operation()?

> `optional` **account\_witness\_vote\_operation**(`op`): `void`

#### Parameters

##### op

[`account_witness_vote`](../interfaces/account_witness_vote)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`account_witness_vote_operation`](./OperationVisitor#account_witness_vote_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:45](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L45)

***

### cancel\_transfer\_from\_savings\_operation()?

> `optional` **cancel\_transfer\_from\_savings\_operation**(`op`): `void`

#### Parameters

##### op

[`cancel_transfer_from_savings`](../interfaces/cancel_transfer_from_savings)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`cancel_transfer_from_savings_operation`](./OperationVisitor#cancel_transfer_from_savings_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:67](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L67)

***

### change\_recovery\_account\_operation()?

> `optional` **change\_recovery\_account\_operation**(`op`): `void`

#### Parameters

##### op

[`change_recovery_account`](../interfaces/change_recovery_account)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`change_recovery_account_operation`](./OperationVisitor#change_recovery_account_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:59](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L59)

***

### claim\_account\_operation()?

> `optional` **claim\_account\_operation**(`op`): `void`

#### Parameters

##### op

[`claim_account`](../interfaces/claim_account)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`claim_account_operation`](./OperationVisitor#claim_account_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:55](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L55)

***

### claim\_reward\_balance\_operation()?

> `optional` **claim\_reward\_balance\_operation**(`op`): `void`

#### Parameters

##### op

[`claim_reward_balance`](../interfaces/claim_reward_balance)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`claim_reward_balance_operation`](./OperationVisitor#claim_reward_balance_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:69](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L69)

***

### collateralized\_convert\_operation()?

> `optional` **collateralized\_convert\_operation**(`op`): `void`

#### Parameters

##### op

[`collateralized_convert`](../interfaces/collateralized_convert)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`collateralized_convert_operation`](./OperationVisitor#collateralized_convert_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:78](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L78)

***

### comment\_operation()

> **comment\_operation**(`op`): `void`

#### Parameters

##### op

[`comment`](../interfaces/comment)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`comment_operation`](./OperationVisitor#comment_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:18](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L18)

***

### comment\_options\_operation()?

> `optional` **comment\_options\_operation**(`op`): `void`

#### Parameters

##### op

[`comment_options`](../interfaces/comment_options)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`comment_options_operation`](./OperationVisitor#comment_options_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:52](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L52)

***

### convert\_operation()?

> `optional` **convert\_operation**(`op`): `void`

#### Parameters

##### op

[`convert`](../interfaces/convert)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`convert_operation`](./OperationVisitor#convert_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:41](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L41)

***

### create\_claimed\_account\_operation()?

> `optional` **create\_claimed\_account\_operation**(`op`): `void`

#### Parameters

##### op

[`create_claimed_account`](../interfaces/create_claimed_account)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`create_claimed_account_operation`](./OperationVisitor#create_claimed_account_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:56](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L56)

***

### create\_proposal\_operation()?

> `optional` **create\_proposal\_operation**(`op`): `void`

#### Parameters

##### op

[`create_proposal`](../interfaces/create_proposal)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`create_proposal_operation`](./OperationVisitor#create_proposal_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:74](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L74)

***

### custom\_json\_operation()

> **custom\_json\_operation**(`op`): `void`

#### Parameters

##### op

[`custom_json`](../interfaces/custom_json)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`custom_json_operation`](./OperationVisitor#custom_json_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:28](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L28)

***

### custom\_operation()?

> `optional` **custom\_operation**(`op`): `void`

#### Parameters

##### op

[`custom`](../interfaces/custom)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`custom_operation`](./OperationVisitor#custom_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:48](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L48)

***

### decline\_voting\_rights\_operation()?

> `optional` **decline\_voting\_rights\_operation**(`op`): `void`

#### Parameters

##### op

[`decline_voting_rights`](../interfaces/decline_voting_rights)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`decline_voting_rights_operation`](./OperationVisitor#decline_voting_rights_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:68](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L68)

***

### delegate\_vesting\_shares\_operation()?

> `optional` **delegate\_vesting\_shares\_operation**(`op`): `void`

#### Parameters

##### op

[`delegate_vesting_shares`](../interfaces/delegate_vesting_shares)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`delegate_vesting_shares_operation`](./OperationVisitor#delegate_vesting_shares_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:70](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L70)

***

### delete\_comment\_operation()?

> `optional` **delete\_comment\_operation**(`op`): `void`

#### Parameters

##### op

[`delete_comment`](../interfaces/delete_comment)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`delete_comment_operation`](./OperationVisitor#delete_comment_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:50](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L50)

***

### escrow\_approve\_operation()?

> `optional` **escrow\_approve\_operation**(`op`): `void`

#### Parameters

##### op

[`escrow_approve`](../interfaces/escrow_approve)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`escrow_approve_operation`](./OperationVisitor#escrow_approve_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:64](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L64)

***

### escrow\_dispute\_operation()?

> `optional` **escrow\_dispute\_operation**(`op`): `void`

#### Parameters

##### op

[`escrow_dispute`](../interfaces/escrow_dispute)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`escrow_dispute_operation`](./OperationVisitor#escrow_dispute_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:61](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L61)

***

### escrow\_release\_operation()?

> `optional` **escrow\_release\_operation**(`op`): `void`

#### Parameters

##### op

[`escrow_release`](../interfaces/escrow_release)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`escrow_release_operation`](./OperationVisitor#escrow_release_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:62](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L62)

***

### escrow\_transfer\_operation()?

> `optional` **escrow\_transfer\_operation**(`op`): `void`

#### Parameters

##### op

[`escrow_transfer`](../interfaces/escrow_transfer)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`escrow_transfer_operation`](./OperationVisitor#escrow_transfer_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:60](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L60)

***

### feed\_publish\_operation()?

> `optional` **feed\_publish\_operation**(`op`): `void`

#### Parameters

##### op

[`feed_publish`](../interfaces/feed_publish)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`feed_publish_operation`](./OperationVisitor#feed_publish_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:40](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L40)

***

### limit\_order\_cancel\_operation()?

> `optional` **limit\_order\_cancel\_operation**(`op`): `void`

#### Parameters

##### op

[`limit_order_cancel`](../interfaces/limit_order_cancel)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`limit_order_cancel_operation`](./OperationVisitor#limit_order_cancel_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:39](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L39)

***

### limit\_order\_create\_operation()?

> `optional` **limit\_order\_create\_operation**(`op`): `void`

#### Parameters

##### op

[`limit_order_create`](../interfaces/limit_order_create)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`limit_order_create_operation`](./OperationVisitor#limit_order_create_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:38](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L38)

***

### limit\_order\_create2\_operation()?

> `optional` **limit\_order\_create2\_operation**(`op`): `void`

#### Parameters

##### op

[`limit_order_create2`](../interfaces/limit_order_create2)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`limit_order_create2_operation`](./OperationVisitor#limit_order_create2_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:54](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L54)

***

### pow\_operation()?

> `optional` **pow\_operation**(`op`): `void`

#### Parameters

##### op

[`pow`](../interfaces/pow)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`pow_operation`](./OperationVisitor#pow_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:47](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L47)

***

### pow2\_operation()?

> `optional` **pow2\_operation**(`op`): `void`

#### Parameters

##### op

[`pow2`](../interfaces/pow2)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`pow2_operation`](./OperationVisitor#pow2_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:63](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L63)

***

### recover\_account\_operation()?

> `optional` **recover\_account\_operation**(`op`): `void`

#### Parameters

##### op

[`recover_account`](../interfaces/recover_account)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`recover_account_operation`](./OperationVisitor#recover_account_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:58](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L58)

***

### recurrent\_transfer\_operation()

> **recurrent\_transfer\_operation**(`op`): `void`

#### Parameters

##### op

[`recurrent_transfer`](../interfaces/recurrent_transfer)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`recurrent_transfer_operation`](./OperationVisitor#recurrent_transfer_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:47](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L47)

***

### remove\_proposal\_operation()?

> `optional` **remove\_proposal\_operation**(`op`): `void`

#### Parameters

##### op

[`remove_proposal`](../interfaces/remove_proposal)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`remove_proposal_operation`](./OperationVisitor#remove_proposal_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:76](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L76)

***

### request\_account\_recovery\_operation()?

> `optional` **request\_account\_recovery\_operation**(`op`): `void`

#### Parameters

##### op

[`request_account_recovery`](../interfaces/request_account_recovery)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`request_account_recovery_operation`](./OperationVisitor#request_account_recovery_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:57](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L57)

***

### set\_withdraw\_vesting\_route\_operation()?

> `optional` **set\_withdraw\_vesting\_route\_operation**(`op`): `void`

#### Parameters

##### op

[`set_withdraw_vesting_route`](../interfaces/set_withdraw_vesting_route)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`set_withdraw_vesting_route_operation`](./OperationVisitor#set_withdraw_vesting_route_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:53](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L53)

***

### transfer\_from\_savings\_operation()

> **transfer\_from\_savings\_operation**(`op`): `void`

#### Parameters

##### op

[`transfer_from_savings`](../interfaces/transfer_from_savings)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`transfer_from_savings_operation`](./OperationVisitor#transfer_from_savings_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:43](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L43)

***

### transfer\_operation()

> **transfer\_operation**(`op`): `void`

#### Parameters

##### op

[`transfer`](../interfaces/transfer)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`transfer_operation`](./OperationVisitor#transfer_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:22](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L22)

***

### transfer\_to\_savings\_operation()

> **transfer\_to\_savings\_operation**(`op`): `void`

#### Parameters

##### op

[`transfer_to_savings`](../interfaces/transfer_to_savings)

#### Returns

`void`

#### Overrides

[`OperationVisitor`](./OperationVisitor).[`transfer_to_savings_operation`](./OperationVisitor#transfer_to_savings_operation)

#### Defined in

[wasm/lib/detailed/encryption\_visitor.ts:39](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/encryption_visitor.ts#L39)

***

### transfer\_to\_vesting\_operation()?

> `optional` **transfer\_to\_vesting\_operation**(`op`): `void`

#### Parameters

##### op

[`transfer_to_vesting`](../interfaces/transfer_to_vesting)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`transfer_to_vesting_operation`](./OperationVisitor#transfer_to_vesting_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:36](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L36)

***

### update\_proposal\_operation()?

> `optional` **update\_proposal\_operation**(`op`): `void`

#### Parameters

##### op

[`update_proposal`](../interfaces/update_proposal)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`update_proposal_operation`](./OperationVisitor#update_proposal_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:77](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L77)

***

### update\_proposal\_votes\_operation()?

> `optional` **update\_proposal\_votes\_operation**(`op`): `void`

#### Parameters

##### op

[`update_proposal_votes`](../interfaces/update_proposal_votes)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`update_proposal_votes_operation`](./OperationVisitor#update_proposal_votes_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:75](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L75)

***

### vote\_operation()?

> `optional` **vote\_operation**(`op`): `void`

#### Parameters

##### op

[`vote`](../interfaces/vote)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`vote_operation`](./OperationVisitor#vote_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:33](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L33)

***

### withdraw\_vesting\_operation()?

> `optional` **withdraw\_vesting\_operation**(`op`): `void`

#### Parameters

##### op

[`withdraw_vesting`](../interfaces/withdraw_vesting)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`withdraw_vesting_operation`](./OperationVisitor#withdraw_vesting_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:37](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L37)

***

### witness\_block\_approve\_operation()?

> `optional` **witness\_block\_approve\_operation**(`op`): `void`

#### Parameters

##### op

[`witness_block_approve`](../interfaces/witness_block_approve)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`witness_block_approve_operation`](./OperationVisitor#witness_block_approve_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:49](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L49)

***

### witness\_set\_properties\_operation()?

> `optional` **witness\_set\_properties\_operation**(`op`): `void`

#### Parameters

##### op

[`witness_set_properties`](../interfaces/witness_set_properties)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`witness_set_properties_operation`](./OperationVisitor#witness_set_properties_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:72](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L72)

***

### witness\_update\_operation()?

> `optional` **witness\_update\_operation**(`op`): `void`

#### Parameters

##### op

[`witness_update`](../interfaces/witness_update)

#### Returns

`void`

#### Inherited from

[`OperationVisitor`](./OperationVisitor).[`witness_update_operation`](./OperationVisitor#witness_update_operation)

#### Defined in

[wasm/lib/detailed/visitor.ts:44](https://gitlab.syncad.com/hive/wax/-/blob/118cc41b9e3c5cabf1f0bf5691d038b26cace2f3/ts/wasm/lib/detailed/visitor.ts#L44)
