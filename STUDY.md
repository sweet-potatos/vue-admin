## 关于不同版本的Vue
### vue.js 与 vue.runtime.xxx.js的区别
```
  (1).vue.js是完整版的Vue，包括：核心功能+模板解析器
  (2).vue.runtime.xxx.js是运行版的Vue，只有核心功能，没有模板解析器
```

### 不能使用template配置项的原因
> 因为vue.runtime.xxx.js，没有模板解析器，所以不能使用template配置项，需要使用render函数接收到的createElement函数去指定具体内容


## vue.config.js配置文件
> 使用 vue inspect > output.js 可以查看Vue脚手架的默认配置
> 使用vue.config.js可以对脚手架进行个性化定制，详情见文档：https://cli.vuejs.org/zh/


## ref属性
```
  1.被用来给元素或子组件注册引用信息(id的替代者)
  2.应用在html标签上获取的是真实的DOM元素，应用在组件标签上是组件实例对象(vc)
  3.使用方式:
    打标识: <h1 ref="xxx">...</h1> 或 <School ref="xxx" />
    获取: this.$ref.xxx
```