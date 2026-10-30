[@hiveio/workerbee](../globals) / TBlogContentProvided

# Type Alias: TBlogContentProvided\<TAccounts\>

> **TBlogContentProvided**\<`TAccounts`\> = \{ \[K in TAccounts\[number\]\]: IOperationTransactionPair\<comment\>\[\] \| WorkerBeeIterable\<IOperationTransactionPair\<comment\>\> \}

Defined in: [src/chain-observers/providers/blog-content-provider.ts:10](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/chain-observers/providers/blog-content-provider.ts#L10)

## Type Parameters

### TAccounts

`TAccounts` *extends* `TAccountName`[]
