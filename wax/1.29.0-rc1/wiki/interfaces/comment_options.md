[@hiveio/wax](../globals) / comment\_options

# Interface: comment\_options

The operation comment_options_operation allows to set properties regarding payouts,
rewards or beneficiaries (using {extensions}) for comments.
If the operation: comment_options_operation is done by one of the frontends,
it is usually in the same transaction with the operation: comment_operation.
If a comment has received any votes, only the parameter {percent_hbd} may be changed.

Description https://gitlab.syncad.com/hive/hive/-/blob/develop/doc/devs/operations/19_comment_options.md?ref_type=heads

## Properties

### allow\_curation\_rewards

> **allow\_curation\_rewards**: `boolean`

#### Param

The flag that allows to decide whether the voters for the comment should
                                       receive the curation rewards. Rewards return to the reward fund.
                                       Default value: allow_curation_rewards = true.

#### Defined in

wasm/lib/proto/comment\_options.ts:62

***

### allow\_votes

> **allow\_votes**: `boolean`

#### Param

The flag that allows to decide whether the comment may receive a vote.
                            Default value: allow_votes = true.

#### Defined in

wasm/lib/proto/comment\_options.ts:56

***

### author

> **author**: `string`

#### Param

Account name, the author of the comment.

#### Defined in

wasm/lib/proto/comment\_options.ts:30

***

### extensions

> **extensions**: [`comment_options_extension`](./comment_options_extension)[]

#### Param

It may contain the list of the beneficiaries,
                                                the accounts that should receive the author reward.
                                                The list consists of the account name and the weight of the shares in the author reward.
                                                If the sum of the weights is less than 100%,
                                                the rest of the reward is received by the author.
                                                It should be defined less than 128 accounts.
                                                The allowed range of the weight is from 0 to 10000 (0 – 100%).
                                                The beneficiaries should be listed in alphabetical order, no duplicates.

#### Defined in

wasm/lib/proto/comment\_options.ts:73

***

### max\_accepted\_payout

> **max\_accepted\_payout**: `undefined` \| [`asset`](./asset)

#### Param

The maximum value of payout in HBD.
                                     Default value: max_accepted_payout = asset( 1000000000, HBD_SYMBOL ).
                                     The allowed value should be less than the default value.
                                     If max_accepted_payout = 0, then voters and authors will not receive the payout.

#### Defined in

wasm/lib/proto/comment\_options.ts:38

***

### percent\_hbd

> **percent\_hbd**: `number`

#### Param

By default the author reward is paid 50% HP and 50 % HBD.
                              In some rare situations, instead of HBD, the Hive may be paid.
                              percent_hbd = HIVE_100_PERCENT means that 100 % of HBD part is paid in HBD.
                              A user may decide how many percent of HBD (from 50 %) they wants to receive in the HBD,
                              the rest will be paid out in HP.
                              Default value: percent_hbd = HIVE_100_PERCENT.
                              The allowed value should be less than the default value.
                              This is the only parameter that can be modified after the comment receives any vote.

#### Defined in

wasm/lib/proto/comment\_options.ts:51

***

### permlink

> **permlink**: `string`

#### Defined in

wasm/lib/proto/comment\_options.ts:31
