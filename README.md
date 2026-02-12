# Mod仓库

这个仓库用于维护移动版尖塔模组启动器的在线模组中的模组列表。

## 如何添加新模组

1. 把新模组的文件放到 `mods/` 目录。
2. 打开 `manifest.json`，依葫芦画瓢新增一个模组条目。
3. 如果该模组需要在启动器里显示提示，去 `mod_notifications.json` 增加提示。

### manifest.json 示例

```json
"ExampleMod": {
"url": "mods/ExampleMod.jar",
"steamId": "",
"info": {
"modid": "examplemod",
"name": "Example Mod",
"author_list": [
"AuthorName"
],
"description": "这里写模组简介",
"version": "1.0.0",
"sts_version": "12-18-2022",
"mts_version": "3.30.3",
"dependencies": [
"basemod",
"stslib"
]
}
}
```

### mod_notifications.json 示例

```json
{
  "modid": "examplemod",
  "notification": "这里写给玩家看的提示信息"
}
```
