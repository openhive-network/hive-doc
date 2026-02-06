[@hiveio/workerbee](../globals) / WorkerBeeIterable

# Class: WorkerBeeIterable\<T\>

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

• **T**

## Implements

- `Iterable`\<`T`\>

## Constructors

### new WorkerBeeIterable()

> **new WorkerBeeIterable**\<`T`\>(`iterable`): [`WorkerBeeIterable`](./WorkerBeeIterable)\<`T`\>

#### Parameters

##### iterable

`Iterable`\<`T`, `any`, `any`\>

#### Returns

[`WorkerBeeIterable`](./WorkerBeeIterable)\<`T`\>

#### Defined in

[src/types/iterator.ts:18](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/iterator.ts#L18)

## Properties

### iterable

> `protected` `readonly` **iterable**: `Iterable`\<`T`, `any`, `any`\>

#### Defined in

[src/types/iterator.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/iterator.ts#L16)

## Methods

### \[iterator\]()

> **\[iterator\]**(): `Iterator`\<`T`, `any`, `any`\>

#### Returns

`Iterator`\<`T`, `any`, `any`\>

#### Implementation of

`Iterable.[iterator]`

#### Defined in

[src/types/iterator.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/iterator.ts#L22)

***

### forEach()

> **forEach**(`callbackfn`): `void`

#### Parameters

##### callbackfn

(`value`) => `void`

#### Returns

`void`

#### Defined in

[src/types/iterator.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/iterator.ts#L30)

***

### values()

> **values**(): `Iterable`\<`T`, `any`, `any`\>

#### Returns

`Iterable`\<`T`, `any`, `any`\>

#### Defined in

[src/types/iterator.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/1f3f643bda15e565c40fb757d44bfd8511e321cf/src/types/iterator.ts#L26)
