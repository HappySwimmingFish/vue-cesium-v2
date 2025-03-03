# 更新日志

## 2.4.2 - 20230105

- 修复 Cesium 版本号比较错误导致量算报错的问题。

## 2.4.1 - 20221105

- `vc-viewer` 组件通过 `viewerCreator` 自定义初始化异常问题。

## 2.4.0 - 20220922

- 修复全局引入火星库失败的问题。
- 修复引入dc-sdk用cdn地址引入失败的问题。
- 优化组件加载速度。

## 2.3.15 - 20220903

- czml 数据源组件 czml 属性支持传数组。
- 修复 Cesium 1.97 版本去掉 Cesium.Uri 导致天地图组件不正常的问题。

## 2.3.14 - 20220810

- 修复组件在重载时为清空导致淹没分析卡顿的问题。
- 淹没分析改为 vue3 版本的逻辑。

## 2.3.13 - 20220809

- 修复高版本 Cesium 内部 API 变更导致计算面积错误的问题。

## 2.3.12 - 20220803

- 兼容 Cesium 1.96 版本。
- 引入 mars3d 方式改变。

## 2.3.11 - 2022-06-06

- 量算绘制的点默认保持在最上层。
- 全球视角下绘制面显示异常问题修复。
- vc-viewer 组件提供 viewerCreator 属性，传入 viewer 的构造方法，用于加载非标准的第三方 Cesium 库。

## 2.3.10 - 2022-05-19

- 去掉个别还在用 when 的逻辑。
- 资源换为 unpkg.com 的。

## 2.3.9 - 2022-05-14

- 修复高德、百度、腾讯地图组件最大层级参数错误问题。

## 2.3.8 - 2021-05-10

- 修复 vc-primitive-tileset 组件在 Cesium 1.92+ 版本报错问题。

## 2.3.7 - 2021-05-06

- 去掉调试输出。

## 2.3.6 - 2021-05-06

- 增加天地图地形组件 `vc-provider-terrain-tianditu`.
- 导航组件经纬度范围支持配置。
- 调整百度地图组件参数。
- 同步 VcPolygon 组件。

## 2.3.5 - 2021-04-06

- 兼容 Cesium 最新版本。
- 增加 `vc-provider-imagery-tencent` 和 `vc-provider-imagery-amap` 组件。
- 组件事件支持短横线写法。

## 2.3.4 - 2021-02-21

- 兼容最新版本 dc-sdk。

## 2.3.3 - 2021-02-16

- 修复 `vc-map-overview` 在 2D 模式不正常问题。

## 2.3.2 - 2021-01-13

- 修复 `vc-viewer` 组件如果没有监听 `ready` 事件导致子组件无法正常加载的问题。

## 2.3.1 - 2021-12-23

- 替换 heatmapjs 源。
- 修复 `vc-provider-imagery-baidumap` 组件 `projectionTransforms` prop 写错问题。

## 2.3.0 - 2021-12-17

- 用 pnpm 替换 pnpm

## 2.2.12 - 2021-12-16

- 修复量算组件在超图平台上不能拾取到 S3M 模型上的问题（上个版本没完全修复 - -）。

## 2.2.11 - 2021-12-16

- 修复量算组件在超图平台上不能拾取到 S3M 模型上的问题。

## 2.2.10 - 2021-11-30

- 修复 `vc-viewer` timeline 时间格式化不正确的问题。

## 2.2.9 - 2021-11-20

- 添加对火星科技 mars3d 和 数字视觉 dc-sdk 支持。

## 2.2.8 - 2021-10-20

- 修复 `vc-overview-map` 组件修改 `url` 参数不起作用的问题。

## 2.2.7 - 2021-09-09

- 兼容 Cesium 1.85 版本
- 计算相关的椭球体参数不固定为 WGS84 了，从 scene.globe 取（补充上个版本没改完的）

## 2.2.6 - 2021-08-11

- 计算相关的椭球体参数不固定为 WGS84 了，从 scene.globe 取

## 2.2.5 - 2021-06-30

- 修复超图平台移除图层时崩溃的问题。

## 2.2.4 - 2021-06-28

- GeoJSON 数据源 mouserover, mouseout 异常修复。

## 2.2.3 - 2021-05-28

- 参考 3.0 版本优化组件生命周期逻辑。
- 扩展的一些组件支持动态响应更新。

## 2.2.2 - 2021-04-25

- 解决绘制工具编辑时图标不显示的问题。

## 2.2.1 - 2021-03-27

- 解决 umd 打包 coordtransform 引用问题。
- `vc-heatmap` 组件支持用 `breaks` 和 `colors` 属性确定颜色方案。

## 2.2.0 - 2021-01-30

### 修改

- 绘制组件增加编辑功能。
- [`vc-primitive-model`](https://zouyaoji.top/vue-cesium/#/zh/primitive/vc-primitive-model)和[`vc-primitive-tileset`](https://zouyaoji.top/vue-cesium/#/zh/primitive/vc-primitive-tileset) 组件同步官方属性。

## 2.1.9 - 2021-01-10

### 修改

- 常用属性支持传 `Array`。
- 实体属性支持传 `Function`。
- 修复生产环境组件移除异常问题。 [#92](https://github.com/zouyaoji/vue-cesium/issues/92)
- [`vc-ripple-circle-double`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-ripple-circle-double), [`vc-circle-roatating-double`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-circle-roatating-double) 解决设置高度异常问题。

### 修改

- `vc-viewer` camera 属性更新与绑定不一致的问题。

## 2.1.8 - 2021-01-04

### 增加

- [`vc-provider-imagery-baidumap`](https://zouyaoji.top/vue-cesium/#/zh/imageryLayer/vc-provider-imagery-baidumap) 加载百度瓦片地图服务。

### 修改

- 影像 provider 增加属性 `projectionTransforms`，用于瓦片的投影变换。
- `vc-collection-primitive-xxx`, `vc-datasource-xxx` 的集合属性增加动态修改支持。 如[`vc-collection-primitive-billboard`](https://zouyaoji.top/vue-cesium/#/zh/primitives/vc-collection-primitive-billboard)。
- `vc-navigation` 解决二维模式下位置坐标异常问题。
- 实体、图元、几何体等可拾取的对象组件事件优化，并增加 `moveout`、`moveover`、`clickout` 事件响应。
- `vc-viewer` 增加 `cesiumReady` 事件，当 CesiumJS 加载成功时触发。

## 2.1.7 - 2020-12-01

### 修改

- 解决 `umd` 模式下鹰眼组件不正常的问题。
- 解决 [#87](https://github.com/zouyaoji/vue-cesium/issues/87) 提到的按需引入的问题。
- [`vc-datasource-geojson`](https://zouyaoji.top/vue-cesium/#/zh/datasource/vc-datasource-geojson) 等数据源组件都支持通过 `entities` 属性添加实体集合。
- 实体组件 [`vc-entity`](https://zouyaoji.top/vue-cesium/#/zh/entity/vc-entity), 图元组件 [`vc-primitive`](https://zouyaoji.top/vue-cesium/#/zh/primitive/vc-primitive), 图元集合组件 ['vc-collection-primitive'](https://zouyaoji.top/vue-cesium/#/zh/primitives/vc-collection-primitive) 增加响应鼠标点击事件。
- [`vc-layer-imagery`](https://zouyaoji.top/vue-cesium/#/zh/imageryLayer/vc-layer-imagery]) 影像图层组件新增一个属性 `sortOrder` 维护图层相对顺序。
- [`vc-measure-distance`, `vc-measure-area`, `vc-measure-height`](https://zouyaoji.top/vue-cesium/#/zh/tool/vc-measuring) 量算工具支持触摸屏操作。

## 2.1.6 - 2020-08-15

### 增加

- [`vc-overlay-html`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-overlay-html) HTML 元素组件。
- [`vc-overlay-html`](https://zouyaoji.top/vue-cesium/#/zh/control/vc-map-overview) 鹰眼地图组件。

## 2.1.5 - 2020-08-01

### 增加

- [`vc-scan-circle`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-scan-circle) 圆形扫描效果组件。
- [`vc-scan-radar`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-scan-radar) 雷达扫描效果组件。
- [`vc-ripple-circle-double`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-ripple-circle-double) 双圆涟漪效果组件。
- [`vc-shine-ellipse`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-shine-ellipse) 闪圆效果组件。
- [`vc-shine-point`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-shine-point) 闪点效果组件。
- [`vc-trail-polyline`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-trail-polyline) 流动线效果组件。
- [`vc-trail-wall`](https://zouyaoji.top/vue-cesium/#/zh/extend/vc-trail-polyline) 流动墙效果组件。
- [`vc-provider-imagery-style-mapbox`](https://zouyaoji.top/vue-cesium/#/zh/imageryLayer/vc-provider-imagery-style-mapbox) 加载 mapbox 自定义地图服务。
- 支持引入 cesiumlab 的 earthsdk (1.4.17+).

## 2.1.4 - 2020-05-26

### 修改

- 量算和绘制组件 activeEvt 事件的触发顺序调整。
- 量算和绘制组件中绘制的面改为双面。
- 量算距离和量算面积组件解决距离单位 km 时数值不正确问题。
- `vc-navigation` 全屏模式下位置不正确的问题。

## 2.1.3 - 2020-05-14

### 修改

- `vc-viewer` 增加 removeCesiumScript 属性，确定`vc-viewer`在销毁时是否移除 CesiumJS 标签。fixed: #58
- `vc-navigation` 解决单页面添加多个`vc-viewer` 初始化不正常的问题。增加相机高度。增加 heading, pitch, roll 属性。

## 2.1.2 - 2020-05-13

### 增加

- `vc-navigation` 增加 legendChanged 事件，方便获取导航罗盘当前计算的比例尺。
- `vc-navigation` 增加 geolocation 事件，定位成功时返回定位结果。
- `vc-navigation` 鉴于国内谷歌浏览器定位被墙，增加高德定位 API 选项。
- `vc-viewer` 增加转发 viewr.infoBox.viewModel 的 `cameraClicked` 和 `closeClicked` 事件。

### 修改

- 量算工具和绘制工具支持贴地选项。
- `vc-datasource-custom` 解决名称获取异常问题。
- `vc-handler-draw-polygon` 和 `vc-handler-draw-polyline` 增加贴地选项 `clampToGround`。
- `vc-handler-draw-polygon` 的 `polygonColor` 改为 `polygonMaterial`，方便自定义绘制材质。

## 2.1.1 - 2020-05-05

### 修改

- `vc-viewer` 增加 timeline 时间本地化选项。
- `vc-datasource-custom` 可添加批量实体。
- `vc-entity` position 属性可以传 Function，相当于是 callback。

## 2.1.0 - 2020-04-22

### 增加

- `vc-graphics-tileset` 组件，对应 `Cesium3DTilesetGraphics`

### 修改

- 绘制组件 `drawEvt` 事件增加鼠标左键点击反馈。
- 量算组件 `measureEvt` 事件增加鼠标左键点击反馈。
- 量算组件增加 `movingEvt` 事件反馈鼠标所在屏幕坐标。
- `vc-primitive-3dtileset` 组件名称改为 `vc-primitive-tileset`（参考官方的实体命名，两者保持一致）。
- 优化导航控件。

## 2.0.9 - 2020-04-20

### 修改

- 量算组件和绘制组件互斥。
- `vc-handler-draw-polyline`组件可以定义绘制的线型。
- 绘制和量算的点可通过 `depthTest` 属性觉得是否参与深度检测。（默认不参与，即点、线不被地形和模型裁切，会一直显示）
- 加载超图平台客户端绘制的线被遮挡问题修复。

## 2.0.6 - 2020-03-17

### 增加

- 增加粒子系统组件 `vc-primitive-particle` 。
- 增加克里金色斑图组件 `vc-kriging-map`

### 修改

- `vc-navigation` 缩放控件的 `defaultResetView` 属性初始化时会覆盖 `vc-viewer` 的 `camera` 属性，增加一个属性 `overrideCamera` 来控制是否覆盖，默认是否。

## 2.0.5 - 2020-01-07

### 修改

- `vc-measure-distance` 组件增加一个属性 `arcType`, `0` 代表量算时绘制的空间直线, `1` 代表绘制的是测地线。
- 修复 [#48](https://github.com/zouyaoji/vue-cesium/issues/48).

### 2.0.4 - 2019-12-28

### 增加

- `vc-navigation` 组件增加一个定位按钮. 用的是浏览器定位 API `navigator.geolocation`, 谷歌浏览器被墙了，可能没效果， Firefox 和 Edge 测试工作正常。

### 修改

- 数据源聚合事件。
- 数据源属性合并成一个对象。
- `vc-provider-imagery-tianditu`组件域名换了.

## 2.0.3 - 2019-12-23

### 增加

- 国际化语言。 `Vue.use(VueCesium, {cesiumPath: cesiumPath, accessToken: accessToken, lang: lang})` 默认加载中文。
- `vc-navigation` 增加一个打印控件。

### 修改

- css 名称统一。
- 面积量算结果修正，用海伦公式计算表面积。
- 距离量算结果修正，之前简单的用了 `Cartesian3.distance` 计算的是两点之间的直线距离，忽略了地球曲率，并不合理，改为计算`测地距离(GeodesicDistance)`。

## 2.0.2 - 2019-12-19

### 增加

- `vc-navigation-sm` 超图罗盘样式组件。
- `vc-stage-process-post` 后期处理组件。
- `vc-collection-stage-process-post` 后期处理集合组件。
- `vc-provider-imagery-tiledcache` 组件，加载 TiledCache 瓦片。

### 修改

- `vc-navigation` 样式修改了，增加了位置信息。
- `vc-analysis-flood` -> `vc-analytics-flood`

## 2.0.1 - 2019-12-09

### 修改

- 各组件加载放在 Created 生命周期，方便通过获取`createdPromise`对象进行相关逻辑操作。
- 量算组件增加选项，指定测量线和文字标签是否始终显示。

### 增加

- `vc-provider-imagery-supermap` 加载超图 iServer 影像服务。
- `vc-provider-imagery-tianditu` 加载天地图 WMTS 影像服务。
- `vc-handler-draw-point` 绘制点组件。
- `vc-handler-draw-polyline` 绘制线组件。
- `vc-handler-draw-polygon` 绘制面组件。
- `vc-geometry-xxx` 补充几何体对象组件。
  - `vc-geometry-outline-box`: `BoxOutlineGeometry`,
  - `vc-geometry-circle`: `CircleGeometry`,
  - `vc-geometry-outline-circle`: `CircleOutlineGeometry`,
  - `vc-geometry-polygon-coplanar`: `CoplanarPolygonGeometry`,
  - `vc-geometry-outline-polygon-coplanar`: `CoplanarPolygonOutlineGeometry`,
  - `vc-geometry-corridor`: `CorridorGeometry`,
  - `vc-geometry-outline-corridor`: `CorridorOutlineGeometry`,
  - `vc-geometry-cylinder`: `CylinderGeometry`,
  - `vc-geometry-outline-cylinder`: `CylinderOutlineGeometry`,
  - `vc-geometry-ellipse`: `EllipseGeometry`,
  - `vc-geometry-outline-ellipse`: `EllipseOutlineGeometry`,
  - `vc-geometry-ellipsoid`: `EllipsoidGeometry`,
  - `vc-geometry-outline-ellipsoid`: `EllipsoidOutlineGeometry`,
  - `vc-geometry-frustum`: `FrustumGeometry`,
  - `vc-geometry-outline-frustum`: `FrustumOutlineGeometry`,
  - `vc-geometry-polyline-ground`: `GroundPolylineGeometry`,
  - `vc-geometry-plane`: `PlaneGeometry`,
  - `vc-geometry-outline-plane`: `PlaneOutlineGeometry`,
  - `vc-geometry-polygon`: `PolygonGeometry`,
  - `vc-geometry-outline-polygon`: `PolygonOutlineGeometry`,
  - `vc-geometry-polyline`: `PolylineGeometry`,
  - `vc-geometry-polyline-volume`: `PolylineVolumeGeometry`,
  - `vc-geometry-outline-polyline-volume`: `PolylineVolumeOutlineGeometry`,
  - `vc-geometry-rectangle`: `RectangleGeometry`,
  - `vc-geometry-outline-rectangle`: `RectangleOutlineGeometry`,
  - `vc-geometry-polyline-simple`: `SimplePolylineGeometry`,
  - `vc-geometry-sphere`: `SphereGeometry`,
  - `vc-geometry-outline-sphere`: `SphereOutlineGeometry`,
  - `vc-geometry-wall`: `WallGeometry`,
  - `vc-geometry-outline-wall`: `WallOutlineGeometry`

## 2.0.0 - 2019-12-02

### 增加

- `vc-provider-imagery-supermap` 加载超图 iServer 影像服务。
- `vc-provider-imagery-tianditu` 加载天地图 WMTS 影像服务。
- 支持 CDN 引用注册。

## 2.0.0-beta.3 - 2019-11-26

### 修改

- `@babel/runtime-corejs2` 依赖不正确。
- `vc-viewer` 组件有些部件位置异常。
- `vc-provider-imagery-wmts` 组件支持设置天地图服务 token。
- `vc-navigation` 组件样式文件打包。

## 2.0.0-beta.0 - 2019-11-20

这个版本将做了较大的更新，精简了代码，优化了组件加载速度，更优雅的支持局部引入，重新规范了组件命名，请谨慎升级，最新组件名称参考[在线文档](https://zouyaoji.top/vue-cesium/#/)。

### 修改

- 组件打包的 babel 环境升级到 7+ 版本。参考[Babel 中文网](https://www.babeljs.cn/docs/)、[Babel7 学习笔记](https://segmentfault.com/a/1190000017162255)。
- 组件打包方式改为用 rollup 打包。
- 组件加载、卸载方式改为异步，Vue 侦听器改为代码动态创建。
- 组件命名重新规范，根据 Vue 推荐的[风格指南](https://cn.vuejs.org/v2/style-guide/)。
- 组件在线文档规范。

## 1.0.6 - 2019-11-19

### 修改

- fixed [#27](https://github.com/zouyaoji/vue-cesium/issues/27)。

## 1.0.5 - 2019-11-01

V2 版本会做较大更新，我会尽量将此版本现有功能维护到稳定再更新下一个版本。

### 修改

- 解决 1.60+ 版本面绘制问题。
