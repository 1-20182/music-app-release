# 悠音流音乐播放器软件

一款专注于「沉浸式纯播放体验」的 Android 本地音乐播放器,聚合网易/QQ/酷狗多源曲库,内置一起听、鸣潮彩蛋视频背景、睡眠定时、均衡器等实用功能,全程无广告、无外部服务器依赖。

## 主要功能

- 多源曲库聚合:网易/QQ/酷狗三大平台一站搜索,支持跨源匹配同曲版本与音质对比
- 沉浸视频背景:播放界面全线采用视频背景,鸣潮原声曲目自动切换专属风景视频
- 远程一起听:支持主从设备(手机为主,平板为客)通过 Supabase 实时或局域网同步听歌
- 睡眠定时:渐弱关闭、预设时长、播完本曲多种策略,基于 AlarmManager 精准触发
- 音质均衡器:多频段调节、低音增强、环绕声
- 歌词体验:实时歌词、歌词卡生成分享、歌词焦点模式
- 听歌热力图:按日历可视化你的听歌习惯
- 跨源匹配:当前歌曲在其他平台搜索同曲版本,自动优选可用源
- 网易云登录:手机/二维码/Cookie 多种方式,同步歌单与收藏
- 响应式布局:竖屏/横屏自适应,configChanges 避免旋转重建

## 下载

前往 [GitHub Releases](https://github.com/1-20182/music-app-release/releases) 下载最新版 APK,直接安装即可。

> **国内用户镜像**：GitHub 访问不便时,可前往 [GitCode 发行仓库](https://gitcode.com/c3317812824/music-app-release/releases) 下载,已同步 v1.0.0 / v1.5.0 / v1.7.5 / v1.9.4 全部正式发行版本。

> Debug 版使用固定签名,可与历史版本覆盖安装,无需卸载数据。

## 系统要求

- Android 8.0 (API 26) 及以上
- 建议预留 200MB 存储空间(含视频背景素材)

## 权限说明

| 权限 | 用途 |
|------|------|
| INTERNET | 在线曲库搜索与流媒体播放 |
| ACCESS_NETWORK_STATE | 网络状态检测,优化请求策略 |
| WAKE_LOCK | 播放期间保持 CPU 唤醒 |
| FOREGROUND_SERVICE | 后台音乐播放 |
| POST_NOTIFICATIONS (Android 13+) | 播放控制通知 |
| SCHEDULE_EXACT_ALARM (Android 12+) | 睡眠定时精准触发 |
| RECORD_AUDIO | 均衡器音频采集(可选) |
| READ/WRITE_EXTERNAL_STORAGE | 本地音乐读取与缓存(低版本) |

## 反馈

使用中遇到问题或想提新功能建议,请在 [Issues](https://github.com/1-20182/music-app-release/issues) 提交,附上设备型号、Android 版本、复现步骤与日志(如有)。

## 说明

本项目为发行版下载仓库,仅提供成品 APK。源代码与开发讨论请前往开发仓库。
