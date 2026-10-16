# LibreTV Android App

把你的 LibreTV 网页打包成一个简单的 Android App，全屏 WebView 直接打开。

## 怎么编译出 APK

### 方法：用 GitHub Actions 自动编译（推荐）

1. 把这个项目上传到你的 GitHub 仓库（新建一个空仓库，把所有文件传上去）
2. 等 GitHub Actions 自动跑起来（或者手动点 Actions → Build APK → Run workflow）
3. 编译完后，在 Actions 页面下载 artifact 就是 APK 文件了

### 编译时间

大概 2-3 分钟就能出 APK。

## 怎么安装到 Fire TV Stick

1. Fire TV 上装 Downloader App（亚马逊应用商店搜得到）
2. 把 APK 传到一个可以分享的地方
3. Downloader 输入下载链接，安装

## App 功能

- 全屏显示 LibreTV 网页
- 支持视频播放
- 记住登录密码
- 横屏显示
- 遥控器返回键支持

## 修改网址

如果以后你的 LibreTV 地址变了，改 `app/src/main/java/com/libretv/app/MainActivity.java` 里的 `URL` 变量就行，然后重新 push 到 GitHub 自动编译。
