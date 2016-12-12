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
      name : '',
      API : '',
      params : 'key1=val1&key2=$GET.userId&key2=$POST.addTime',
      filter : {                      //过滤器
        addTime : date('Y-m-d'),      //源字段上应用函数
        is3RD : saleType(11,12,13),   //根据源字段形成新字段
        saleModel : case 
      }
    }
    ```
      >> 缓存的定义???

  1. 前端代码npm仓库
  1. 页面管理配置平台

    > URI路由适配

    > 页面与个性化数据集绑定

    > 页面与组件绑定

    ```
    {
      router : '[controller].[model]',//路由定义
      dataSet : [{                    //页面的数据集定义
        id : 73,                      //数据集id
        name : 'brand'                //变量名
      }, {
        id : 88,                      //数据集id
        name : '',                    //变量名
        request : ['brand']           //依赖变量
      }],
      rowSet : [{                     //组件定义

      }]
    }
    ```