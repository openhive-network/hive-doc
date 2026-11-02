[@hiveio/workerbee](../globals) / TBlogContentProvided

# Type Alias: TBlogContentProvided\<TAccounts\>

> **TBlogContentProvided**\<`TAccounts`\> = \{ \[K in TAccounts\[number\]\]: IOperationTransactionPair\<comment\>\[\] \| WorkerBeeIterable\<IOperationTransactionPair\<comment\>\> \}

Defined in: [src/chain-observers/providers/blog-content-provider.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/5d935b802bf63dd6ae9d7911b398e4cc3b84e819/src/chain-observers/providers/blog-content-provider.ts#L10)

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[]
