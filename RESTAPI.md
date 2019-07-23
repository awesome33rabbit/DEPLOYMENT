# Documentation

## 1. ```/api/article/tablist```

- description: 获取 分类列表
- method: ```GET```
- headers: ```authorized:<authorized-keys>```
- rtype: ```json```

    - ```curl 127.0.0.1:9988/api/article/tablist```

```
{
    code: 200,
    tabList: [
        {
            name: "<name>",
            id: "<id>"
        },
    ]
}
```

## 2. ```/api/article/newslist```

- description: 获取 新闻列表
- method: ```GET```
- headers: ```authorized:<authorized-keys>```
- rtype: ```json```

    - ```curl 127.0.0.1:9988/api/article/newslist```
    - ```curl 127.0.0.1:9988/api/article/newslist?type=1```
    - ```curl 127.0.0.1:9988/api/article/newslist?limit=50```
    - ```curl 127.0.0.1:9988/api/article/newslist?page=1```

```
{
    code: 200,
    newsList: [
        {
            id: "<id>",
            title: "<title>",
            author: "<author>",
            images: "['url', 'url']",
            videoSrc: "url",
            time: "<time>",
            type: "<type>"
        },
    ]
}
```

## 3. ```/api/article/content```

- description: 获取 新闻内容
- method: ```GET```
- headers: ```authorized:<authorized-keys>```
- rtype: ```json```

    - ```curl 127.0.0.1:9988/api/article/conent?article_id=article_id```

```
{
    code: 200,
    content: [
        {
            id: "<id>",
            content: "<content>",
        },
    ]
}
```

