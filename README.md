### 爬取携程网上景区的评论信息，包括评论、得分、日期等信息。将得分80、100分的评论作为正类，20、40、60分的评论作为负类，构建情感分类训练集。使用fasttext模型对景区评论数据进行情感分类。

### 一共爬取了重庆、成都两个城市的前十热点景区的评论，一共6w+评论，但是只发布了1w条评论

####代码目录：
- craw.py  爬虫代码
- fasttext_train.py  训练代码
- stop_words.txt 停用词表
- user_dict_all.txt 用户自定义词典
- train.xlsx 爬取下来整理的数据，1w条


####效果(6w数据):

    | 准确率   | 0.87 |
    | 召回率   | 0.90 |
    | F1值     | 0.92 |