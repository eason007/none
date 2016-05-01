组件化中台

> ；

# 痛点
  * 数据提取、聚合逻辑一致性\复用；
  * 前端模板一致性\复用
  * 组件与数据的关系

# 解决方法
  1. 数据接口管理平台

  > 数据提取规则、聚合规则、依赖关系

  > 形成个性化数据集复用

  ```
  {
    id : ,
    name : ,
    API : '',
    params : 'key1=val1&key2=$GET.userId&key2=$POST.addTime'
  }
  ```

  1. 前端代码npm仓库
  1. 页面管理配置平台

  > URI路由适配

  > 页面与个性化数据集绑定

  > 页面与页面组件绑定

  ```JSON
  {
    id : ,
    name : ,
    API : '',
    params : 'key1=val1&key2=$GET.userId&key2=$POST.addTime'
  }
  ```