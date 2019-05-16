# Documentation

## 1. ```/api/spider```

- description: 爬虫接口，增量爬取数据
- method: ```POST```
- headers: ```authorized:<authorized-keys>```
- rtype: ```json```

```curl 127.0.0.1:9988/api/spider -X POST```

```
{
    "code": 200,
    "data": "OK"
}
```

## 2. ```/api/add_category```

- description: 新增文章分类
- method: ```POST```
- form-data: 
```
category_id:<category-id>
category_name:<category-name>
```
- rtype: ```json```

```curl 127.0.0.1:9988/api/category/add -F 'category_id=13' -f 'category_name=测试'```

```
{
    "code": <http-code>,
    "data": "OK"
}
```

## 3. ```/api/article_list```

- description: 获取文章列表
- method: ```GET```
- parameter: 
```
category_id:<category_id> default 0
limit:<max items> default 50
keyword:<keyword> default ''
```
- rtype: ```json```
```

```curl 127.0.0.1:9988/api/article_list?category_id=5```

{
    "code": 200,
    "data": [
        {
            "id": "<id>",
            "title": "<title>",
            "date": "<date>",
            "source": "<source>",
            "content": "<content>",
            "editor": "<editor>",
            "imgs": ["<img>", "<img>"],
            "video": "<video>",
            "audio": "<audio>",
            "author_cover": "<author_cover>",
            "category": {
                "id": "<category-id>",
                "display_name": "<category-name>"
            }
        }
    ]
}
```

## 4. ```/api/article/<article_id>```

- description: 获取文章
- method: ```GET```
- rtype: ```json```
```

```curl 127.0.0.1:9988/api/article/t20190514_32069358```

{
    "code": <http-code>,
    "data": {
        "id": "<id>",
        "title": "<title>",
        "date": "<date>",
        "source": "<source>",
        "author_avatar": "<author_avatar>",
        "content": "<content>",
        "editor": "<editor>",
        "category": {
            "id": "<category-id>",
            "display_name": "<category-name>"
        }
    }
}
```
