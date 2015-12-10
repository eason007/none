性能优化关键点

# 服务器
  * gzip
  > gzip_types text/html text/javascript text/css font/ttf font/otf image/svg+xml
  * keep-alive
  * chunk
  > bigpipe
  * 统一http header
  * 缓存有效期

# 文档
  * html大小
  * css置顶
  * js置底

# 图片
  * jpeg有损压缩
  * jpeg无损压缩
  * png压缩
  * gif大小限制
  * 单文件大小限制

# 请求
  * 静态资源独立域名
  * 异步请求非身份验证，独立域名
  * 图片资源多域名散列
  * 单个类型请求数限制

# 代码
  * 延迟加载
  * 懒加载
  * 异步加载

# 网络
  * CDN
  * BGP
  * LVS

# 指标
  * 首包
  * waiting
  * 白屏
  * 首屏
  * 首屏字节数
  * window.load
  * 总下载字节数
  * 基础文档字节数
  * DNS 解析
  * 200/304/404统计