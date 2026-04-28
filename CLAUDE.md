# 如果你需要编写前端代码的话，请注意以下几点：

## 包安装工具

- 优先使用pnpm

## 框架

- 使用 Vue 3 setup
- 使用 TypeScript
- UI框架使用 Arco Design Vue

## CSS

- 尽量采用Tailwindcss/UnoCSS写法

## 常用工具函数

- 日期时间处理：使用 dayjs
- 工具函数：优先使用 lodash-es 内置 ，而不是自己造轮子
- 事件总线：使用 mitt

## 模块/组件 代码结构

- 每个组件一个文件夹，文件夹内包含组件代码、组件测试代码、组件文档
- 类型定义超过一个要提取到同级的 type.ts 或 interface.ts 文件中
- 善于使用utils目录，将通用的、业务无关的逻辑提取到utils目录中

## 代码风格

- 注重类型，使用 ts，不要使用any
- 做好判空处理
- 考虑代码抽离和复用
- 获取组件实例时，不要使用 ref<InstanceType<typeof PgmEditor>,，改用 useTemplateRef('pgmEditorRef')
- 遵循项目的prettier规范进行代码格式化

## UI还原

- 如果已提供参考图进行UI还原，图中元素很接近Arco组件，优先使用Arco组件

## 代码质量

- 代码逻辑合理，符合业务要求
- 代码架构清晰，注释明确，拓展性强
- 功能考虑周全，交互符合用户直觉

## 注释

- 使用标准的jsDoc注释
- 比较直观的变量、函数（尤其是单个word）无需添加注释
