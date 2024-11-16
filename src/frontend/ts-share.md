# TypeScript

这里暂时记录一些 TypeScript 的学习笔记

## 可选

```typescript
// 这俩类型唯一区别：Person 是可选的，Person2 是必选的
type Person = {
  name: string
  age?: number
}
type Person2 = {
  name: string
  age: number | undefined
}

const user1: Person = { name: '陈磊', age: 25 } // 合法
const user2: Person = { name: '陈磊', age: undefined } // 合法
```

## TS 内置工具类型

TypeScript 提供了一些内置的工具类型，用于在类型系统中进行常见的类型转换和操作，这些类型都是 TypeScript 语言本身提供的，可以直接使用

### Exclude<UnionType, ExcludedMembers>

xxx

## TS 类型运算符

TypeScript 提供强大的类型运算能力，可以使用各种类型运算符，对已有的类型进行计算，得到新类型
