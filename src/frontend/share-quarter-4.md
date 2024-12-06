# 第四季度技术分享
xxxxxxxxxx

## GitHub & Github Pages & 自动部署

讲讲 GitHub 是如何自动部署的，比上次深入一点

GitHub Actions 是一个CI/CD（持续集成/持续交付）平台，可以帮助你自动化构建、测试和部署软件。你可以在仓库中创建工作流文件来定义这些自动化过程。

Runner 就是一个自动化的服务或机器人，负责执行你在 GitHub Actions 工作流中定义的任务。它会按照工作流文件中的步骤，自动化地执行构建、测试、部署等操作。

## ts 类型

- 避免定义全局类型(命名空间,接口,类), 以防止类型冲突

```ts
// a.ts
export declare namespace MyTypes {
  interface Data {
    status: number
    data: any
  }
}

// b.ts
import type { MyTypes } from './a'
```