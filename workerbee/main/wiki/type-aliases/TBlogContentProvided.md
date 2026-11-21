[@hiveio/workerbee](../globals) / TBlogContentProvided

# Type Alias: TBlogContentProvided\<TAccounts\>

> **TBlogContentProvided**\<`TAccounts`\> = \{ \[K in TAccounts\[number\]\]: IOperationTransactionPair\<comment\>\[\] \| WorkerBeeIterable\<IOperationTransactionPair\<comment\>\> \}

Defined in: [src/chain-observers/providers/blog-content-provider.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/bc217d4103c521db7966585fc06621a710c6556e/src/chain-observers/providers/blog-content-provider.ts#L10)

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[]
