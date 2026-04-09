# 如果你需要编写前端代码的话，请注意以下几点：

## 框架

- 使用 Vue 3 setup
- 使用 TypeScript
- UI框架使用 Arco Design Vue

## CSS
- 尽量采用UnoCSS写法
- 相同样式可以抽离为同一个.class

## 文件结构
- 每个组件一个文件夹，文件夹内包含组件代码、组件测试代码、组件文档
- 类型定义超过一个要提取到同级的 type.ts 或 interface.ts 文件中

## 代码风格
- 注重类型，使用 ts，不要使用any
- 做好判空处理
- 考虑代码抽离和复用
- 获取组件实例时，不要使用 ref<InstanceType<typeof PgmEditor>,，改用 useTemplateRef('pgmEditorRef')

## 代码质量
- 代码逻辑合理，符合业务要求
- 代码架构清晰，注释明确，拓展性强
- 功能可用，交互符合用户直觉

## 注释
- 使用 "/** 简述 */" 为js/ts 变量编写注释
- 使用 "/** 
   * 简述
   */" 为js/ts 函数编写注释
- 需要 展开描述的注释，在 @description 中展示描述
- 比较直观的变量、函数（尤其是单个word）无需添加注释