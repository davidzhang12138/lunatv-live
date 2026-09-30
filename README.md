# LunaTV 直播源

从 [iptv-org/iptv](https://github.com/iptv-org/iptv) 的公开频道库里筛选出的**可用**频道，
覆盖中国大陆、香港、台湾（共 80 个频道，实测 m3u8 能拉到分片）。

## 用法

在 LunaTV 的「直播源」里填这个地址：

```
https://raw.githubusercontent.com/davidzhang12138/lunatv-live/main/lunatv-live.m3u
```

## 频道分类

综合 14 / 新闻 10 / 电影 6 / 娱乐 6 / 体育 5 / 纪录 2 / 少儿 1 / 音乐 3
生活 4 / 教育 3 / 财经 1 / 文化 2 / 经典 1 / 购物 1 / 其他 12 / 宗教 6

## 特点

- **没有赌博广告** —— 直播流是电视台直发，实测抽检 15 个频道零命中赌博字样
- 频道可用率会随时间变化，失效的自己失效（LunaTV 会跳过拉不到流的）

## 更新

```bash
# 重新抓取并探活
curl -sL https://iptv-org.github.io/iptv/countries/cn.m3u -o cn.m3u
# 然后跑探活脚本（见 iyf 仓库的 build_live.py）
```
