# TechGuide 插件分发库

卫月第三方插件仓库，供用户在 **设置 → 第三方插件仓库** 添加链接安装 TechGuide。

## 插件仓库 URL

```
https://gitee.com/baofengz/tech-guide-repo/raw/main/pluginmaster.json
```

## 目录说明

| 路径 | 说明 |
|------|------|
| `pluginmaster.json` | 插件索引（由 TechGuide Release 构建自动生成） |
| `release/TechGuide/latest.zip` | 安装包（由 TechGuide Release 构建自动生成） |

## 维护者发版

源码在 `F:\FFIX\FFXIVWY\TechGuide`。Release 编译后会自动写入本仓库：

```cmd
F:\FFIX\FFXIVWY\TechGuide\build-release.cmd
```

确认文件后手动推送：

```cmd
cd /d F:\FFIX\FFXIVWY\tech-guide-repo
git add .
git commit -m "release 1.0.0.0"
git push origin main
```
