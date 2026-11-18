[@hiveio/wax](../globals) / TDelegableHpAccountData

# Type Alias: TDelegableHpAccountData

> **TDelegableHpAccountData** = `Pick`\<[`ApiAccount`](../interfaces/ApiAccount), `"vesting_shares"` \| `"delegated_vesting_shares"` \| `"received_vesting_shares"` \| `"vesting_withdraw_rate"` \| `"next_vesting_withdrawal"` \| `"withdrawn"` \| `"to_withdraw"` \| `"voting_manabar"` \| `"downvote_manabar"`\>

Defined in: [wasm/lib/detailed/interfaces.ts:101](https://gitlab.syncad.com/hive/wax/-/blob/a16d25496931bf7989e7fb881def9b373fa78a3a/ts/wasm/lib/detailed/interfaces.ts#L101)

Account properties (as returned by the find_accounts API call) required to calculate the delegable HP
