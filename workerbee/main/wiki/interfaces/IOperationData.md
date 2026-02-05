[@hiveio/workerbee](../globals) / IOperationData

# Interface: IOperationData

## Extends

- [`IOperationBaseData`](./IOperationBaseData)

## Properties

### operations

> **operations**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`operation`\>, `any`, `any`\>

#### Inherited from

[`IOperationBaseData`](./IOperationBaseData).[`operations`](./IOperationBaseData#operations)

#### Defined in

[src/chain-observers/classifiers/operation-classifier.ts:11](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/operation-classifier.ts#L11)

***

### operationsPerType

> **operationsPerType**: `object`

#### account\_create\_operation?

> `optional` **account\_create\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_create`\>, `any`, `any`\>

#### account\_create\_with\_delegation\_operation?

> `optional` **account\_create\_with\_delegation\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_create_with_delegation`\>, `any`, `any`\>

#### account\_created\_operation?

> `optional` **account\_created\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_created`\>, `any`, `any`\>

#### account\_update\_operation?

> `optional` **account\_update\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_update`\>, `any`, `any`\>

#### account\_update2\_operation?

> `optional` **account\_update2\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_update2`\>, `any`, `any`\>

#### account\_witness\_proxy\_operation?

> `optional` **account\_witness\_proxy\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_witness_proxy`\>, `any`, `any`\>

#### account\_witness\_vote\_operation?

> `optional` **account\_witness\_vote\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`account_witness_vote`\>, `any`, `any`\>

#### author\_reward\_operation?

> `optional` **author\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`author_reward`\>, `any`, `any`\>

#### cancel\_transfer\_from\_savings\_operation?

> `optional` **cancel\_transfer\_from\_savings\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`cancel_transfer_from_savings`\>, `any`, `any`\>

#### change\_recovery\_account\_operation?

> `optional` **change\_recovery\_account\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`change_recovery_account`\>, `any`, `any`\>

#### changed\_recovery\_account\_operation?

> `optional` **changed\_recovery\_account\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`changed_recovery_account`\>, `any`, `any`\>

#### claim\_account\_operation?

> `optional` **claim\_account\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`claim_account`\>, `any`, `any`\>

#### claim\_reward\_balance\_operation?

> `optional` **claim\_reward\_balance\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`claim_reward_balance`\>, `any`, `any`\>

#### clear\_null\_account\_balance\_operation?

> `optional` **clear\_null\_account\_balance\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`clear_null_account_balance`\>, `any`, `any`\>

#### collateralized\_convert\_immediate\_conversion\_operation?

> `optional` **collateralized\_convert\_immediate\_conversion\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`collateralized_convert_immediate_conversion`\>, `any`, `any`\>

#### collateralized\_convert\_operation?

> `optional` **collateralized\_convert\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`collateralized_convert`\>, `any`, `any`\>

#### comment\_benefactor\_reward\_operation?

> `optional` **comment\_benefactor\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`comment_benefactor_reward`\>, `any`, `any`\>

#### comment\_operation?

> `optional` **comment\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`comment`\>, `any`, `any`\>

#### comment\_options\_operation?

> `optional` **comment\_options\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`comment_options`\>, `any`, `any`\>

#### comment\_payout\_update\_operation?

> `optional` **comment\_payout\_update\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`comment_payout_update`\>, `any`, `any`\>

#### comment\_reward\_operation?

> `optional` **comment\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`comment_reward`\>, `any`, `any`\>

#### consolidate\_treasury\_balance\_operation?

> `optional` **consolidate\_treasury\_balance\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`consolidate_treasury_balance`\>, `any`, `any`\>

#### convert\_operation?

> `optional` **convert\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`convert`\>, `any`, `any`\>

#### create\_claimed\_account\_operation?

> `optional` **create\_claimed\_account\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`create_claimed_account`\>, `any`, `any`\>

#### create\_proposal\_operation?

> `optional` **create\_proposal\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`create_proposal`\>, `any`, `any`\>

#### curation\_reward\_operation?

> `optional` **curation\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`curation_reward`\>, `any`, `any`\>

#### custom\_json\_operation?

> `optional` **custom\_json\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`custom_json`\>, `any`, `any`\>

#### custom\_operation?

> `optional` **custom\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`custom`\>, `any`, `any`\>

#### decline\_voting\_rights\_operation?

> `optional` **decline\_voting\_rights\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`decline_voting_rights`\>, `any`, `any`\>

#### declined\_voting\_rights\_operation?

> `optional` **declined\_voting\_rights\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`declined_voting_rights`\>, `any`, `any`\>

#### delayed\_voting\_operation?

> `optional` **delayed\_voting\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`delayed_voting`\>, `any`, `any`\>

#### delegate\_vesting\_shares\_operation?

> `optional` **delegate\_vesting\_shares\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`delegate_vesting_shares`\>, `any`, `any`\>

#### delete\_comment\_operation?

> `optional` **delete\_comment\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`delete_comment`\>, `any`, `any`\>

#### dhf\_conversion\_operation?

> `optional` **dhf\_conversion\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`dhf_conversion`\>, `any`, `any`\>

#### dhf\_funding\_operation?

> `optional` **dhf\_funding\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`dhf_funding`\>, `any`, `any`\>

#### effective\_comment\_vote\_operation?

> `optional` **effective\_comment\_vote\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`effective_comment_vote`\>, `any`, `any`\>

#### escrow\_approve\_operation?

> `optional` **escrow\_approve\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_approve`\>, `any`, `any`\>

#### escrow\_approved\_operation?

> `optional` **escrow\_approved\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_approved`\>, `any`, `any`\>

#### escrow\_dispute\_operation?

> `optional` **escrow\_dispute\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_dispute`\>, `any`, `any`\>

#### escrow\_rejected\_operation?

> `optional` **escrow\_rejected\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_rejected`\>, `any`, `any`\>

#### escrow\_release\_operation?

> `optional` **escrow\_release\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_release`\>, `any`, `any`\>

#### escrow\_transfer\_operation?

> `optional` **escrow\_transfer\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`escrow_transfer`\>, `any`, `any`\>

#### expired\_account\_notification\_operation?

> `optional` **expired\_account\_notification\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`expired_account_notification`\>, `any`, `any`\>

#### failed\_recurrent\_transfer\_operation?

> `optional` **failed\_recurrent\_transfer\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`failed_recurrent_transfer`\>, `any`, `any`\>

#### feed\_publish\_operation?

> `optional` **feed\_publish\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`feed_publish`\>, `any`, `any`\>

#### fill\_collateralized\_convert\_request\_operation?

> `optional` **fill\_collateralized\_convert\_request\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_collateralized_convert_request`\>, `any`, `any`\>

#### fill\_convert\_request\_operation?

> `optional` **fill\_convert\_request\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_convert_request`\>, `any`, `any`\>

Virtual operations:

#### fill\_order\_operation?

> `optional` **fill\_order\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_order`\>, `any`, `any`\>

#### fill\_recurrent\_transfer\_operation?

> `optional` **fill\_recurrent\_transfer\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_recurrent_transfer`\>, `any`, `any`\>

#### fill\_transfer\_from\_savings\_operation?

> `optional` **fill\_transfer\_from\_savings\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_transfer_from_savings`\>, `any`, `any`\>

#### fill\_vesting\_withdraw\_operation?

> `optional` **fill\_vesting\_withdraw\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`fill_vesting_withdraw`\>, `any`, `any`\>

#### hardfork\_hive\_operation?

> `optional` **hardfork\_hive\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`hardfork_hive`\>, `any`, `any`\>

#### hardfork\_hive\_restore\_operation?

> `optional` **hardfork\_hive\_restore\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`hardfork_hive_restore`\>, `any`, `any`\>

#### hardfork\_operation?

> `optional` **hardfork\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`hardfork`\>, `any`, `any`\>

#### ineffective\_delete\_comment\_operation?

> `optional` **ineffective\_delete\_comment\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`ineffective_delete_comment`\>, `any`, `any`\>

#### interest\_operation?

> `optional` **interest\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`interest`\>, `any`, `any`\>

#### limit\_order\_cancel\_operation?

> `optional` **limit\_order\_cancel\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`limit_order_cancel`\>, `any`, `any`\>

#### limit\_order\_cancelled\_operation?

> `optional` **limit\_order\_cancelled\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`limit_order_cancelled`\>, `any`, `any`\>

#### limit\_order\_create\_operation?

> `optional` **limit\_order\_create\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`limit_order_create`\>, `any`, `any`\>

#### limit\_order\_create2\_operation?

> `optional` **limit\_order\_create2\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`limit_order_create2`\>, `any`, `any`\>

#### liquidity\_reward\_operation?

> `optional` **liquidity\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`liquidity_reward`\>, `any`, `any`\>

#### pow\_operation?

> `optional` **pow\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`pow`\>, `any`, `any`\>

#### pow\_reward\_operation?

> `optional` **pow\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`pow_reward`\>, `any`, `any`\>

#### pow2\_operation?

> `optional` **pow2\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`pow2`\>, `any`, `any`\>

#### producer\_missed\_operation?

> `optional` **producer\_missed\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`producer_missed`\>, `any`, `any`\>

#### producer\_reward\_operation?

> `optional` **producer\_reward\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`producer_reward`\>, `any`, `any`\>

#### proposal\_fee\_operation?

> `optional` **proposal\_fee\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`proposal_fee`\>, `any`, `any`\>

#### proposal\_pay\_operation?

> `optional` **proposal\_pay\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`proposal_pay`\>, `any`, `any`\>

#### proxy\_cleared\_operation?

> `optional` **proxy\_cleared\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`proxy_cleared`\>, `any`, `any`\>

#### recover\_account\_operation?

> `optional` **recover\_account\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`recover_account`\>, `any`, `any`\>

#### recurrent\_transfer\_operation?

> `optional` **recurrent\_transfer\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`recurrent_transfer`\>, `any`, `any`\>

#### remove\_proposal\_operation?

> `optional` **remove\_proposal\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`remove_proposal`\>, `any`, `any`\>

#### request\_account\_recovery\_operation?

> `optional` **request\_account\_recovery\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`request_account_recovery`\>, `any`, `any`\>

#### return\_vesting\_delegation\_operation?

> `optional` **return\_vesting\_delegation\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`return_vesting_delegation`\>, `any`, `any`\>

#### set\_withdraw\_vesting\_route\_operation?

> `optional` **set\_withdraw\_vesting\_route\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`set_withdraw_vesting_route`\>, `any`, `any`\>

#### shutdown\_witness\_operation?

> `optional` **shutdown\_witness\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`shutdown_witness`\>, `any`, `any`\>

#### system\_warning\_operation?

> `optional` **system\_warning\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`system_warning`\>, `any`, `any`\>

#### transfer\_from\_savings\_operation?

> `optional` **transfer\_from\_savings\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`transfer_from_savings`\>, `any`, `any`\>

#### transfer\_operation?

> `optional` **transfer\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`transfer`\>, `any`, `any`\>

#### transfer\_to\_savings\_operation?

> `optional` **transfer\_to\_savings\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`transfer_to_savings`\>, `any`, `any`\>

#### transfer\_to\_vesting\_completed\_operation?

> `optional` **transfer\_to\_vesting\_completed\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`transfer_to_vesting_completed`\>, `any`, `any`\>

#### transfer\_to\_vesting\_operation?

> `optional` **transfer\_to\_vesting\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`transfer_to_vesting`\>, `any`, `any`\>

#### update\_proposal\_operation?

> `optional` **update\_proposal\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`update_proposal`\>, `any`, `any`\>

#### update\_proposal\_votes\_operation?

> `optional` **update\_proposal\_votes\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`update_proposal_votes`\>, `any`, `any`\>

#### vesting\_shares\_split\_operation?

> `optional` **vesting\_shares\_split\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`vesting_shares_split`\>, `any`, `any`\>

#### vote\_operation?

> `optional` **vote\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`vote`\>, `any`, `any`\>

#### withdraw\_vesting\_operation?

> `optional` **withdraw\_vesting\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`withdraw_vesting`\>, `any`, `any`\>

#### witness\_block\_approve\_operation?

> `optional` **witness\_block\_approve\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`witness_block_approve`\>, `any`, `any`\>

#### witness\_set\_properties\_operation?

> `optional` **witness\_set\_properties\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`witness_set_properties`\>, `any`, `any`\>

#### witness\_update\_operation?

> `optional` **witness\_update\_operation**: `Iterable`\<[`IOperationTransactionPair`](./IOperationTransactionPair)\<`witness_update`\>, `any`, `any`\>

#### Defined in

[src/chain-observers/classifiers/operation-classifier.ts:15](https://gitlab.syncad.com/hive/workerbee/-/blob/a9c18a70c8fa630b34e00ffd5c64e7e0814c726d/src/chain-observers/classifiers/operation-classifier.ts#L15)
