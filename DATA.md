# MySQL
# DATABASE working
### TABLE api_article
    article_id           <str> :'str'              新闻ID
    article_title        <str> :'str'              新闻标题
    article_date         <str> :'xxxx-xx-xx'       新闻发布日期
    article_source       <str> :'str'              新闻来源
    article_content      <str> :'str'              新闻正文
    article_editor       <str> :'str'              编辑
    article_imgs         <list>:['url', 'url']     图片地址列表
    article_video        <str> :'url'              视频地址
    article_audio        <str> :'url'              音频地址
    article_cover        <str> :'url'              封面（如果图片列表中有数据，取第一张图片url；如果图片列表没有数据，则为'NULL'）
    article_url          <str> :'url'              新闻链接原地址
    article_category_id  <str> :'str'              分类ID
### TABLE api_category
    category_id          <str>:'str'              分类ID
    category_name        <str>:'str'              分类名称
