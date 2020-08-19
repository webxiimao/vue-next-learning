#### 对比vue2

- 类型检查 Flow => Typescript

> TypeScript提供了更好的类型检查，能支持复杂的类型推导；由于源码就使用 TypeScript 编写，也省去了单独维护 d.ts 文件的麻烦

- 性能优化

  - 源码体积优化

  > 1.移除一些冷门的 feature（比如 filter、inline-template 等）
  >
  > 2.引入 tree-shaking 的技术，减少打包体积

  - 优化数据劫持

    1. Object.defineProperty => Proxy

    > 由于 Vue.js 无法判断你在运行时到底会访问到哪个属性，所以对于这样一个嵌套层级较深的对象，如果要劫持它内部深层次的对象变化，就需要递归遍历这个对象，执行 Object.defineProperty 把每一层对象数据都变成响应式的。

- 编译优化
  
  - 只diff动态节点

#### vue3 组件渲染

- 创建vnode -> 渲染vnode -> 创建dom

> 创建vnode  生成vnode 
>
> 渲染vnode patch方法
>
> 创建dom hostCreateElement...

- diff

#### vue3 reactive库



