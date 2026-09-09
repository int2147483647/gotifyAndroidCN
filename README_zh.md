# Gotify Android [![Build Status][github-action-badge]][github-action] [![FOSSA Status][fossa-badge]][fossa] [![latest release version][release-badge]][release] [![F-Droid][fdroid-badge]][fdroid]

<img align="right" src="app.gif" width="250" />

Gotify Android 连接到 [gotify/server](https://github.com/gotify/server)，并在收到新消息时显示推送通知。

## 功能特性

* 收到新消息时显示推送通知
* 查看和删除消息

## 安装

下载 APK 或通过 F-Droid / Google Play 获取应用。

[<img src="https://play.google.com/intl/en_gb/badges/images/generic/en_badge_web_generic.png" alt="Get it on Google Play" width="150" />][playstore]
[<img src="https://fdroid.gitlab.io/artwork/badge/get-it-on.png" alt="Get it on F-Droid" width="150"/>][fdroid]
[<img src="download-badge.png" alt="Get it on F-Droid" width="150"/>][release]

Google Play 和 Google Play 徽标是 Google LLC 的商标。

### 禁用电池优化

默认情况下，Android 会终止长时间运行的应用以节省电量。启用电池优化后，Gotify 将被终止，您将无法收到任何通知。

以下是禁用 Gotify 电池优化的方法：

* 打开"设置"
* 搜索"电池优化"
* 找到"Gotify"并禁用电池优化

另请参阅 https://dontkillmyapp.com，了解各手机制造商禁用电池优化的具体说明。

### 最小化 Gotify 前台通知

*仅适用于 Android 8 及以上版本*

显示连接状态的前台通知可以手动最小化以减少干扰：

* 打开 设置 -> 应用 -> Gotify
* 点击 通知
* 点击 `Gotify 前台通知`
* 切换"最小化"选项 / 选择不同的"行为"或"重要性"（取决于您的 Android 版本）
* 重启 Gotify

## 消息优先级

| 通知方式 | Gotify 优先级 |
| - | - |
| 无通知 | 0 |
| 通知栏图标 | 1 - 3 |
| 通知栏图标 + 声音 | 4 - 7 |
| 通知栏图标 + 声音 + 振动 | 8 - 10 |

## 构建

使用 Java 17 并执行以下命令来构建 APK。

```bash
$ ./gradlew build
```

## 更新客户端

* 运行 `./gradlew openApiGenerate`
* 提交更改

## 版本管理
我们使用 [SemVer](http://semver.org/) 进行版本管理。有关可用版本，请参阅[此仓库的标签](https://github.com/gotify/android/tags)。

## 许可证
本项目基于 MIT 许可证 - 详情请参阅 [LICENSE](LICENSE) 文件

 [github-action-badge]: https://github.com/gotify/android/workflows/Build/badge.svg
 [github-action]: https://github.com/gotify/android/actions?query=workflow%3ABuild
 [playstore]: https://play.google.com/store/apps/details?id=com.github.gotify
 [fdroid-badge]: https://img.shields.io/f-droid/v/com.github.gotify.svg
 [fdroid]: https://f-droid.org/de/packages/com.github.gotify/
 [fossa-badge]: https://app.fossa.io/api/projects/git%2Bgithub.com%2Fgotify%2Fandroid.svg?type=shield
 [fossa]: https://app.fossa.io/projects/git%2Bgithub.com%2Fgotify%2Fandroid
 [release-badge]: https://img.shields.io/github/release/gotify/android.svg
 [release]: https://github.com/gotify/android/releases/latest
