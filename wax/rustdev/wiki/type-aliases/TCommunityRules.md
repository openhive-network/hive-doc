[@hiveio/wax](../globals) / TCommunityRules

# Type Alias: TCommunityRules

> **TCommunityRules**: \{`account`: [`TAccountName`](./TAccountName);`action`: [`FLAG_POST`](../enumerations/ECommunityOperationActions#flag_post) \| [`MUTE_POST`](../enumerations/ECommunityOperationActions#mute_post) \| [`UNMUTE_POST`](../enumerations/ECommunityOperationActions#unmute_post);`notes`: `string`;`permlink`: `string`; \} \| \{`account`: [`TAccountName`](./TAccountName);`action`: [`PIN_POST`](../enumerations/ECommunityOperationActions#pin_post) \| [`UNPIN_POST`](../enumerations/ECommunityOperationActions#unpin_post);`permlink`: `string`; \} \| \{`action`: [`SUBSCRIBE`](../enumerations/ECommunityOperationActions#subscribe) \| [`UNSUBSCRIBE`](../enumerations/ECommunityOperationActions#unsubscribe); \} \| \{`account`: [`TAccountName`](./TAccountName);`action`: [`SET_ROLE`](../enumerations/ECommunityOperationActions#set_role);`role`: [`EAvailableCommunityRoles`](../enumerations/EAvailableCommunityRoles); \} \| \{`account`: [`TAccountName`](./TAccountName);`action`: [`SET_USER_TITLE`](../enumerations/ECommunityOperationActions#set_user_title);`title`: `string`; \} \| \{`action`: [`UPDATE_PROPS`](../enumerations/ECommunityOperationActions#update_props);`props`: `Readonly`\<[`ICommunityProps`](../interfaces/ICommunityProps)\>; \}

## Defined in

[wasm/lib/detailed/hive\_apps\_operations/community.ts:3](https://gitlab.syncad.com/hive/wax/-/blob/dd7802d3411ef1a48993a053b4667ff7b4c56682/ts/wasm/lib/detailed/hive_apps_operations/community.ts#L3)
