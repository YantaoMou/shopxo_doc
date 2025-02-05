## URL生成

创建于 2021-08-01 / 最近更新于 2021-08-01 / 6319

字体： \[默认\] \[大\] \[更大\]

### 生成 URL 方法

| 方法名称 | 描述 |
| --- | --- |
| PluginsHomeUrl | 前端 URL 生成方法 |
| PluginsAdminUrl | 后端 URL 生成方法 |

### 生成 URL 参数

| 参数名称 | 描述 |
| --- | --- |
| $plugins\_name | 应用唯一标记名称 |
| $plugins\_control | 应用控制器 |
| $plugins\_action | 应用方法 |
| $params | 参数(一维数组) |

### 实例

> 生成前端首页 **PluginsHomeUrl('test\_plugins', 'index', 'index')**
> 
> 生成后端首页 **PluginsAdminUrl('coupon', 'test\_plugins', 'index', \['test'=>'hello'\])**