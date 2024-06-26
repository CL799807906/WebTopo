## WEB组态
基于若依框架的web组态 
物联云组态地址：http://81.68.197.219:10071/index   github 123456
## 功能清单
| 功能 | 状态 | 
| -  | -: | 
| 面板标尺 | 完成 |
| 拖曳添加组件 | 完成 |
| 位置移动-鼠标 | 完成 |
| 位置移动-方向键 | 完成 |
| 位置移动-批量 | 完成 |
| 拖动位置磁性吸附 | 未完成 |
| 尺寸锚点（8个） | 完成 |
| 旋转锚点 | 完成 |
| 选中效果 | 完成 |
| 层叠控制 | 完成 |
| 面板比例缩放 | 完成 |
| CTRL+C/V复制黏贴 | 完成 |
| CTRL+A多选 | 完成 |
| 鼠标框选 | 完成 |
| DELETE删除（支持删除多个） | 完成 |
| 样式配置（文字、大小、位置、边框、颜色、旋转） | 完成 |
| 组件继承体系 | 完成 |
| DOM组件（文字、图片） | 完成 |
| canvas组件（圆形、三角形、矩形、线条、箭头线条） | 完成 |
| 折线箭头 | 部分完成 |
| echarts组件 | 完成 |
| SVG组件 | 完成 |
| 组件同步/异步数据加载 | 完成 |
| 通讯机制-事件总线 | 完成 |
| 通讯机制-VUEX | 完成 |
| 事件总线-WebSocket | 完成 |
| 事件总线-MQTT | 完成 |
| VUEX-WebSocket | 完成 |
| VUEX-MQTT | 完成 |


## 高级功能
| 功能 | 状态 | 
| -  | -: | 
| 批量编辑属性 | 完成 |
| 对齐工具 | 完成 |
| 撤销和恢复 | 有限支持 |
| 容器组件 | 完成 |
| 动画 | 完成 |

## 撤销和恢复支持操作列表
| 命令码 | 操作 | 撤销 | 恢复 | 
| -  | -  | -  | -: | 
| add | 新增 | 支持 | 支持|
| del | 删除 | 支持 | 支持|
| move | 移动 | 支持 | 支持|
| select | 选择 | 完成 | 完成|
| -- | 反选 | 完成 | 完成|
| resize | 形变 | 完成 | 完成|
| copy-add | 多项复制 | 完成 | 完成|
| -- | 属性修改 | 完成 | 完成|
| lock | 选择 | 完成 | 完成|

## 如何拓展控件
1. 定义数据文件（参见 \src\components\topo\data-toolbox下的json文件）
2. 新增控件，根据数据文件的数据自己实现显示方式（在\src\components\topo\control下新增控件，继承组件，可参考其他组件实现方式，整个思想就是利用第一步的数据绘制dom节点或canvas图像）
3. 注册控件到工具栏（在TopoToolbox.vue中）
4. 注册控件（在TopoBase.vue中）

## 构建命令参考
npm install --registry=https://registry.npmmirror.com
```
### Compiles and hot-reloads for development
```
npm run dev
```
### Compiles and minifies for production
```
npm run build
```

## 运行截图
![image](https://github.com/CL799807906/WebTopo/assets/26914642/2fcea729-2d62-4e14-953a-f839d00192fd)


