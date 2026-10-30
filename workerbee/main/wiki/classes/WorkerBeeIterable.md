[@hiveio/workerbee](../globals) / WorkerBeeIterable

# Class: WorkerBeeIterable\<T\>

Defined in: [src/types/iterator.ts:15](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L15)

Container that can be iterated over the elements of the collection.

## Examples

```typescript
for (const { transaction } of data.whaleOperations)
  console.log(`Got transaction: #${transaction.id}`);
```

```typescript
data.whaleOperations.forEach(({ transaction }) => console.log(`Got transaction: #${transaction.id}`)));
```

## Extended by

- [`WorkerBeeArrayIterable`](./WorkerBeeArrayIterable)

## Type Parameters

### T

`T`

## Implements

- `Iterable`\<`T`\>

## Constructors

### Constructor

> **new WorkerBeeIterable**\<`T`\>(`iterable`): `WorkerBeeIterable`\<`T`\>

Defined in: [src/types/iterator.ts:18](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L18)

#### Parameters

##### iterable

`Iterable`\<`T`\>

#### Returns

`WorkerBeeIterable`\<`T`\>

## Properties

### iterable

> `protected` `readonly` **iterable**: `Iterable`\<`T`\>

Defined in: [src/types/iterator.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L16)

## Methods

### \[iterator\]()

> **\[iterator\]**(): `Iterator`\<`T`\>

Defined in: [src/types/iterator.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L22)

#### Returns

`Iterator`\<`T`\>

#### Implementation of

`Iterable.[iterator]`

***

### forEach()

> **forEach**(`callbackfn`): `void`

Defined in: [src/types/iterator.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L30)

#### Parameters

##### callbackfn

(`value`) => `void`

#### Returns

`void`

***

### values()

> **values**(): `Iterable`\<`T`\>

Defined in: [src/types/iterator.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/3982dd8b488b220b2d8116d78e4de2feb40b2434/src/types/iterator.ts#L26)

#### Returns

`Iterable`\<`T`\>
