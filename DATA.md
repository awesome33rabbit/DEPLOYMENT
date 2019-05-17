# MySQL
### DATABASE working
    - article_id           <str>     新闻ID
    - article_title        <str>     新闻标题
    - article_date         <str>     xxxx-xx-xx  新闻发布日期
    - article_source       <str>     新闻来源
    - article_content      <str>     新闻正文
    - article_editor       <str>     编辑
    - article_imgs         <list>    图片列表
    - article_video        <str>     视频地址
    - article_video        <str>     音频地址
    - article_cover        <str>     封面（如果图片列表中有数据，取第一张图片；如果图片列表没有数据，则为‘NULL’）
    - article_url          <str>     新闻链接原地址
    - article_category_id  <str>     分类ID
### TABLE api_article, api_category
    - category_id          <str>     分类ID
    - category_name        <str>     分类名称
