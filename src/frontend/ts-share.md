# TypeScript

这里暂时记录一些 ts 的学习笔记

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
