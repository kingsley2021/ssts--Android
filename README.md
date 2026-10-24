# 随身听书（安卓和ios版）

一个聚合听书工具。程序本身只是播放器，不带任何内容：听书源来自用户导入的**插件**，也可以听自己网盘和手机里的音频。

## 下载

- **安卓版 5.4**：[ssts-v5.4.apk](https://github.com/whykang/ssts--Android/releases/download/v5.4/ssts-v5.4.apk)
- **iOS 版 5.4**（未签名 ipa，需要 iOS 16 及以上）：[ssts-ios-5.4-unsigned.ipa](https://github.com/whykang/ssts--Android/releases/download/v5.4/ssts-ios-5.4-unsigned.ipa)
- **插件包 5.4**（36 个源，安卓和 iOS 通用）：[Sources-v5.4.zip](https://github.com/whykang/ssts--Android/releases/download/v5.4/Sources-v5.4.zip)
- **在线导入插件**：不用下载文件，在“插件”页选择从网址导入，填入下面的地址即可（国内网络可直接访问）

  ```
  https://gitee.com/whykan/ssxz/raw/master/Sources-v5.4.zip
  ```

- 历史版本：[Releases](https://github.com/whykang/ssts--Android/releases)

## 最近更新

**程序（安卓、iOS 5.4）**

- 音量最高 500%：有 100% 到 500% 的快捷档位，小声的音频也能听清
- 摇一摇重新计时：定时中摇一摇手机，重新开始计时并响一声。在定时页面开启，默认关闭
- 跳过静音：自动跳过长时间的停顿和空白。默认关闭，在设置里打开
- 书架新增“书签”一栏，汇总所有书签
- 封面手势：左滑下一集，右滑上一集
- 进度旁显示“第 x / y 集 · 目录”，点一下打开目录
- 进度旁可以直接加入书架，电台也可以
- 移出书架要再确认一次
- 本地文件的发现页分类改为：全部、每个第一层文件夹、其他
- 本地文件打开发现页不再扫描全部子文件夹，文件夹多时也能很快打开
- 本地文件和网盘的文件夹里没有封面图时，按书名到听书源里找封面
- 电子书先从豆瓣读书找封面，找不到再用听书源
- 新增内置源“电子书朗读”：朗读本地的 txt 和 epub 电子书，自动分章节
- 电子书朗读可以选朗读引擎和声音、调语速、试听；除了系统朗读，也可以选微软 Edge 在线朗读（需要联网）
- 设置里新增“后台运行”（安卓）：可以直接打开电池优化和厂商的后台管理设置
- 修复：“最近播放”有时不是从第一条开始显示

**书源（插件包 5.4，共 36 个源）**

- 云听不再内置，移到插件里，并支持 7 天回播
- 新增全球电台：来自 RadioDroid 使用的开放电台库 Radio Browser，可以收听世界各地的电台
- 下载 [Sources-v5.4.zip](https://github.com/whykang/ssts--Android/releases/download/v5.4/Sources-v5.4.zip) 导入即可覆盖旧版本

## 界面预览

| 书架 | 发现 | 播放 | 插件 |
|:---:|:---:|:---:|:---:|
| ![书架](docs/images/library.jpg) | ![发现](docs/images/discover.jpg) | ![播放](docs/images/player.jpg) | ![插件](docs/images/plugins.jpg) |

## 功能

**听书源**

- **插件**：从文件或网址导入 zip 插件包，一个插件可以包含多个源；支持启用、禁用、排序、删除，源的登录和设置，一键测试和调试日志
- **网盘**：内置夸克网盘、百度网盘、阿里云盘、115 网盘和 WebDAV，在设置里开启并登录自己的账号后使用；每个文件夹是一本书，里面的音频是章节，可以指定只看某个目录
- **本地文件**：在设置里选择手机上的一个文件夹，第一层文件夹是分类，里面的文件夹是一本本书；没有封面图时会按书名自动找封面
- **电子书朗读**：朗读手机里的 txt、epub 电子书，可以选朗读引擎、声音和语速
- **广播电台**：插件里有“云听”的全国电台直播（央广频道能回听最近 7 天）和“全球电台”；也可以在设置里添加自己的电台

**找书**

- **发现**：按源浏览分类，一键切换听书源，滚动到底自动加载下一页，封面网格 / 列表两种显示
- **聚合搜索**：多个源同时搜索，结果按源筛选；需要人机验证的源可以在应用内完成验证
- **书架**：收藏的书和最近播放，记住每本书听到哪一集、哪个位置；可以分类
- **云同步**：通过坚果云（WebDAV）在安卓、iOS、Mac 之间同步书架、播放记录、听书进度和书签

**播放**

- 后台播放，通知栏 / 锁屏 / 耳机控制
- 断点续播、自动播放下一集
- 倍速 0.5x – 3x、音量 0 – 500%，每本书记住自己的倍速和音量；可以跳过静音
- 下载到本机离线听，可以按区间下载；播放时自动预缓存后面几集
- 书签：记下某一集的某个位置，可以写备注
- 快进快退（步长可调）
- 定时关闭：本集结束后、播完几集、预设时长或自定义分钟数，结束前音量渐弱，摇一摇重新计时
- 单书跳过片头片尾
- 章节倒序、按标题筛选、定位到上次听到的位置

**界面**

- 浅色、深色、跟随系统
- 7 种主题色

## 插件

这个仓库放的是插件相关的部分：开发文档、示例插件的源码和打好的插件包。

- 📦 [plugins/dist/ShunSources.zip](plugins/dist/ShunSources.zip)：打好的插件包（5.3，34 个听书源），下载后在 App 的“插件”页点 `+` →“从文件导入 zip”

- 📖 [插件开发指南](docs/plugin-development.md)：插件包结构、源的写法、宿主提供的能力、调试和打包
- 🧩 [plugins/ShunSources](plugins/ShunSources)：示例插件的源码，覆盖了文档里提到的大部分写法

插件是一个 zip，里面放一个 `manifest.json` 和若干 JavaScript 脚本，脚本里用 `registerSource({...})` 注册源：

```js
registerSource({
  id: '0f9c0b5c2d7e4c1b9a0e6f3a2b1c4d5e',
  name: '我的站点',
  url: 'https://example.com',

  search: function (keywords, page) {
    var doc = this.host.getHtml('https://example.com/search?q=' + encodeURIComponent(keywords) + '&p=' + page);
    var books = doc.select('.item').map(function (e) {
      return { coverUrl: e.first('img').absUrl('src'), bookUrl: e.first('a').absUrl('href'), title: e.first('h3').text() };
    });
    return { books: books, totalPage: page };
  },

  bookDetail: function (bookUrl) {
    var doc = this.host.getHtml(bookUrl);
    return { episodes: doc.select('#playlist a').map(function (a) { return { title: a.text(), url: a.absUrl('href') }; }) };
  },

  audio: function (episodeUrl) {
    return this.host.getHtml(episodeUrl).first('audio').absUrl('src');
  }
});
```

完整说明见[插件开发指南](docs/plugin-development.md)。

## 说明

本程序只是播放器，不提供任何内容，所有音频都来自插件访问的第三方网站或用户自己的网盘和文件，请支持正版。
插件脚本会在本机访问网络，请只导入你信任的来源提供的插件。
