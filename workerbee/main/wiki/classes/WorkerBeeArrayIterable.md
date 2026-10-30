[@hiveio/workerbee](../globals) / WorkerBeeArrayIterable

# Class: WorkerBeeArrayIterable\<T\>

Defined in: [src/types/iterator.ts:36](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L36)

Container that can be iterated over the elements of the collection.

## Examples

```typescript
for (const { transaction } of data.whaleOperations)
  console.log(`Got transaction: #${transaction.id}`);
```

```typescript
data.whaleOperations.forEach(({ transaction }) => console.log(`Got transaction: #${transaction.id}`)));
```

## Extends

- [`WorkerBeeIterable`](./WorkerBeeIterable)\<`T`\>

## Type Parameters

### T

`T`

## Constructors

### Constructor

> **new WorkerBeeArrayIterable**\<`T`\>(`array?`): `WorkerBeeArrayIterable`\<`T`\>

Defined in: [src/types/iterator.ts:37](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L37)

#### Parameters

##### array?

`T`[] = `[]`

#### Returns

`WorkerBeeArrayIterable`\<`T`\>

#### Overrides

[`WorkerBeeIterable`](./WorkerBeeIterable).[`constructor`](./WorkerBeeIterable#constructor)

## Properties

### iterable

> `protected` `readonly` **iterable**: `Iterable`\<`T`\>

Defined in: [src/types/iterator.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L16)

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`iterable`](./WorkerBeeIterable#iterable)

## Methods

### \[iterator\]()

> **\[iterator\]**(): `Iterator`\<`T`\>

Defined in: [src/types/iterator.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L22)

#### Returns

`Iterator`\<`T`\>

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`[iterator]`](WorkerBeeIterable.md#iterator)

***

### forEach()

> **forEach**(`callbackfn`): `void`

Defined in: [src/types/iterator.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L30)

#### Parameters

##### callbackfn

(`value`) => `void`

#### Returns

`void`

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`forEach`](./WorkerBeeIterable#foreach)

***

### push()

> **push**(`value`): `void`

Defined in: [src/types/iterator.ts:41](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L41)

#### Parameters

##### value

`T`

#### Returns

`void`

***

### values()

> **values**(): `Iterable`\<`T`\>

Defined in: [src/types/iterator.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/14ef337aed6fb39de20f05f5efe0a62254b4a09f/src/types/iterator.ts#L26)

#### Returns

`Iterable`\<`T`\>

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`values`](./WorkerBeeIterable#values)
