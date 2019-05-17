# MySQL
# DATABASE working
### TABLE api_article
    article_id           <str>     新闻ID:'str'
    article_title        <str>     新闻标题:'str'
    article_date         <str>     新闻发布日期:'xxxx-xx-xx'
    article_source       <str>     新闻来源:'str'
    article_content      <str>     新闻正文:'str'
    article_editor       <str>     编辑:'str'
    article_imgs         <list>    图片列表:['url', 'url']
    article_video        <str>     视频地址:'url'
    article_video        <str>     音频地址:'url'
    article_cover        <str>     封面（如果图片列表中有数据，取第一张图片；如果图片列表没有数据，则为'NULL'）
    article_url          <str>     新闻链接原地址:'url'
    article_category_id  <str>     分类ID:'str'
### TABLE api_category
    category_id          <str>     分类ID:'str'
    category_name        <str>     分类名称:'str'
