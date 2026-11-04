# 点亮中国｜微信网页版部署说明

这是可部署的静态网站，地图数据已内置在 index.html 中。

## GitHub Pages 部署
1. 登录 GitHub，新建 Public 仓库，例如 `light-up-china`。
2. 在仓库根目录上传 `index.html` 并提交。
3. 打开 Settings → Pages → Build and deployment。
4. Source 选择 Deploy from a branch，Branch 选择 main / (root)，保存。
5. 等待 Pages 发布，复制页面显示的 HTTPS 网址。
6. 将该网址发到微信，iPhone 点击链接即可在微信浏览器中打开。

注意：HTML 文件直接通过微信作为文件发送，和发送 HTTPS 网页链接是两种不同的打开方式。前者仍可能被文件预览器拦截。

## 游戏说明
- 支持大陆县级行政区划与台湾乡镇市区地图。
- 支持地级市、直辖市和台湾县市的聚合点亮。
- 成功输入后清空文本框；重名排除已点亮选项。
- 地图数据不需要额外的远程请求。
- 进度保存在访问该网站的浏览器 localStorage 中，不跨设备同步。

## 发布前提示
地图数据来源于用户提供的 ChinaGeoJson 与台湾行政边界数据，可能不符合最新行政区划或公开地图审图要求。公开发布前应核查地图审核、版权与数据授权。
