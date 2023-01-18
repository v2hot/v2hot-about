# 🔥 V2HOT - 每日 V2EX 最热主题 🔥

## 关于

一个能查看 V2EX 每天最热的网站。

## 访问

可以通过下列域名访问，选择访问最快的域名。

- https://v2hot.pipecraft.net/
- https://v2exhot.web.app/
- https://v2hot.github.io/ (暂时不可用 🚫)
- https://v2hot.now.sh/
- https://v2hot.vercel.app/
- https://v2exhot.now.sh/
- https://v2exhot.vercel.app/

## RSS/Atom

每个页面的 URL 后面加上 `atom.xml` 或 `rss.xml` 即是该页面的订阅链接。(特定日期的主题页面除外)

每个订阅源有 3 种输出个数，100 个、50 个、20 个。

- `atom.xml` 或 `rss.xml`：输出 100 个主题，与网页显示的个数一致。
- `atom50.xml` 或 `rss50.xml`：输出 50 个主题。
  > 当订阅源为 /{tab}/hottest-3/, /{tab}/hottest-7/, /{tab}/hottest-30/, /hot/ 时，只截取评论数最多的 50 个。只想看评论多、较热的主题的选择这个。
- `atom20.xml` 或 `rss20.xml`：输出 20 个主题。
  > 当订阅源为 /{tab}/hottest-3/, /{tab}/hottest-7/, /{tab}/hottest-30/, /hot/ 时，只截取评论数最多的 20 个。只想看评论非常多、非常热的选择这个。

示例：

```txt
https://v2hot.pipecraft.net/hot/
->
https://v2hot.pipecraft.net/hot/atom.xml
https://v2hot.pipecraft.net/hot/atom50.xml
https://v2hot.pipecraft.net/hot/atom20.xml
https://v2hot.pipecraft.net/hot/rss.xml
https://v2hot.pipecraft.net/hot/rss50.xml
https://v2hot.pipecraft.net/hot/rss20.xml
```

```txt
https://v2hot.pipecraft.net/hot/hottest-3/
->
https://v2hot.pipecraft.net/hot/hottest-3/atom.xml
https://v2hot.pipecraft.net/hot/hottest-3/atom50.xml
https://v2hot.pipecraft.net/hot/hottest-3/atom20.xml
https://v2hot.pipecraft.net/hot/hottest-3/rss.xml
https://v2hot.pipecraft.net/hot/hottest-3/rss50.xml
https://v2hot.pipecraft.net/hot/hottest-3/rss20.xml
```

```txt
https://v2hot.pipecraft.net/creative/newest/
->
https://v2hot.pipecraft.net/creative/newest/atom.xml
https://v2hot.pipecraft.net/creative/newest/atom50.xml
https://v2hot.pipecraft.net/creative/newest/atom20.xml
https://v2hot.pipecraft.net/creative/newest/rss.xml
https://v2hot.pipecraft.net/creative/newest/rss50.xml
https://v2hot.pipecraft.net/creative/newest/rss20.xml
```

```txt
https://v2hot.pipecraft.net/hot/2022/2022-12-05/
->
(x) # 特定日期的主题页面不支持 rss/atom。
```

## API (暂时不可用 🚫)

生成网页用到的数据以 json 格式保存在 [data](https://github.com/v2hot/v2hot.github.io/tree/data) 分支里。
任何人可以拿去使用。

### 今日热议主题

- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/v2ex-api/hot-topics.json

### 每日最热主题

格式：`https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/{{tab}}/{{year}}/{{date}}.json`

举例：

- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/hot/2021/2021-12-07.json
- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/tech/2021/2021-12-07.json

### 最新上榜主题

格式：`https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/{{tab}}/newest.json`

举例：

- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/hot/newest.json
- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/tech/newest.json

### 三天最热主题 / 七天最热主题 / 30 天最热主题

格式：

- `https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/{{tab}}/hottest-3.json`
- `https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/{{tab}}/hottest-7.json`
- `https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/{{tab}}/hottest-30.json`

举例：

- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/hot/hottest-3.json
- https://cdn.jsdelivr.net/gh/v2hot/v2hot.github.io@data/tech/hottest-7.json

## 反馈

如果有什么建议或反馈，[请提交 issue](https://github.com/v2hot/v2hot-about/issues)。

## License

Copyright (c) 2021 [Pipecraft][my-url]. Licensed under the [MIT license][license-url].

## >\_

[![Pipecraft](https://img.shields.io/badge/site-pipecraft-brightgreen)](https://www.pipecraft.net)
[![DTO](https://img.shields.io/badge/site-DTO-brightgreen)](https://dto.pipecraft.net)
[![BestXTools](https://img.shields.io/badge/site-bestxtools-brightgreen)](https://www.bestxtools.com)

[my-url]: https://www.pipecraft.net
[license-url]: LICENSE
