---
jsApi: true
title: "[I] StringTemplate"

---
## Extends

- [`BaseType`](BaseType.md)

## Properties

| Property | Type | Description | Inheritance |
| :------ | :------ | :------ | :------ |
| `instantiationParameters`? | [`Type`](../type-aliases/Type.md)[] | - | [`BaseType`](BaseType.md).`instantiationParameters` |
| `isFinished` | `boolean` | Reflect if a type has been finished(Decorators have been called).<br />There is multiple reasons a type might not be finished:<br />- a template declaration will not<br />- a template instance that argument that are still template parameters<br />- a template instance that is only partially instantiated(like a templated operation inside a templated interface) | [`BaseType`](BaseType.md).`isFinished` |
| `kind` | `"StringTemplate"` | - | [`BaseType`](BaseType.md).`kind` |
| `node` | [`StringTemplateExpressionNode`](StringTemplateExpressionNode.md) | - | [`BaseType`](BaseType.md).`node` |
| `projectionBase`? | [`Type`](../type-aliases/Type.md) | - | [`BaseType`](BaseType.md).`projectionBase` |
| `projectionSource`? | [`Type`](../type-aliases/Type.md) | - | [`BaseType`](BaseType.md).`projectionSource` |
| `projector`? | [`Projector`](Projector.md) | - | [`BaseType`](BaseType.md).`projector` |
| `spans` | [`StringTemplateSpan`](../type-aliases/StringTemplateSpan.md)[] | - | - |

## Accessors

### projections

```ts
get projections(): ProjectionStatementNode[]
```

#### Returns

[`ProjectionStatementNode`](ProjectionStatementNode.md)[]

## Methods

### projectionsByName()

```ts
projectionsByName(name): ProjectionStatementNode[]
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `name` | `string` |

#### Returns

[`ProjectionStatementNode`](ProjectionStatementNode.md)[]

#### Inherited from

[`BaseType`](BaseType.md).[`projectionsByName`](BaseType.md#projectionsbyname)
