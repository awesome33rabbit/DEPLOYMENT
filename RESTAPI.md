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
    data: [
      {
          name: "<name>",
          id: "<id>"
      }
}
```

## 2. ```/api/article/newslist```

- description: 获取 新闻
- method: ```GET```
- headers: ```authorized:<authorized-keys>```
- rtype: ```json```

    - ```curl 127.0.0.1:9988/api/article/newslist```

```
{
    code: 200,
    data: [
    {
        id: "<id>",
        title: "<title>",
        author: "<author>",
        images: "['url', 'url']",
        videoSrc: "url",
        time: "<time>",
        type: "<type>"
    },
}
```

