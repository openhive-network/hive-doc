[@hiveio/workerbee](../globals) / TBlogContentProvided

# Type Alias: TBlogContentProvided\<TAccounts\>

> **TBlogContentProvided**\<`TAccounts`\> = \{ \[K in TAccounts\[number\]\]: IOperationTransactionPair\<comment\>\[\] \| WorkerBeeIterable\<IOperationTransactionPair\<comment\>\> \}

Defined in: [src/chain-observers/providers/blog-content-provider.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/chain-observers/providers/blog-content-provider.ts#L10)

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[]
