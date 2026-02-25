[@hiveio/workerbee](../globals) / WorkerBeeArrayIterable

# Class: WorkerBeeArrayIterable\<T\>

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

• **T**

## Constructors

### new WorkerBeeArrayIterable()

> **new WorkerBeeArrayIterable**\<`T`\>(`array`): [`WorkerBeeArrayIterable`](./WorkerBeeArrayIterable)\<`T`\>

#### Parameters

##### array

`T`[] = `[]`

#### Returns

[`WorkerBeeArrayIterable`](./WorkerBeeArrayIterable)\<`T`\>

#### Overrides

[`WorkerBeeIterable`](./WorkerBeeIterable).[`constructor`](./WorkerBeeIterable#constructors)

#### Defined in

[src/types/iterator.ts:37](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L37)

## Properties

### iterable

> `protected` `readonly` **iterable**: `Iterable`\<`T`, `any`, `any`\>

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`iterable`](./WorkerBeeIterable#iterable)

#### Defined in

[src/types/iterator.ts:16](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L16)

## Methods

### \[iterator\]()

> **\[iterator\]**(): `Iterator`\<`T`, `any`, `any`\>

#### Returns

`Iterator`\<`T`, `any`, `any`\>

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`[iterator]`](WorkerBeeIterable.md#%5Biterator%5D)

#### Defined in

[src/types/iterator.ts:22](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L22)

***

### forEach()

> **forEach**(`callbackfn`): `void`

#### Parameters

##### callbackfn

(`value`) => `void`

#### Returns

`void`

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`forEach`](./WorkerBeeIterable#foreach)

#### Defined in

[src/types/iterator.ts:30](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L30)

***

### push()

> **push**(`value`): `void`

#### Parameters

##### value

`T`

#### Returns

`void`

#### Defined in

[src/types/iterator.ts:41](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L41)

***

### values()

> **values**(): `Iterable`\<`T`, `any`, `any`\>

#### Returns

`Iterable`\<`T`, `any`, `any`\>

#### Inherited from

[`WorkerBeeIterable`](./WorkerBeeIterable).[`values`](./WorkerBeeIterable#values)

#### Defined in

[src/types/iterator.ts:26](https://gitlab.syncad.com/hive/workerbee/-/blob/7c3c23177a79866fc4012a98ce8ff004a399f20c/src/types/iterator.ts#L26)
