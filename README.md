# weibo-spider

## 介绍

使用 Python3（jupyter notebook） 调用微博移动端 api 进行特定内容的数据爬取，并将数据结果保存为 .csv 文件与 sqlite3 数据库中。

对爬得的微博内容进行过滤、合并、分词，最终得到词云，并保存图片。

* 本项目无框架使用。
* 本项目部分代码来自网络。
* 本项目使用以下关键的包或库：
    * requests，json，处理请求
    * re，正则内容匹配与过滤
    * pandas，数据处理
    * csv，sqlite3，存储数据结果
    * jieba，wordcloud，文本内容处理与词云生成
* 请勿使用本项目进行任何侵犯他人权益的行为与活动。

---------

## 注意事项

* 请保证 spider.ipynb 中使用到的的包全部都已安装。

* 在执行完爬取任务后，将会生成任务结果目录。若将 spider.ipynb 中的代码全部执行完成，将生成 4 个新文件：

  ```
  .
  └── weibo_无毛猫_20_2021-12-05-15:14:09	// 命名规则：weibo_{搜索词条}_{抓取页数}_{日期时间}
      ├── content.txt							// 爬到的微博内容合集
      ├── data.csv							// 爬到的所有数据
      ├── sqlite3.db							// 将爬取到的数据存入 sqlite3 数据库
      └── word_cloud.png						// 生成的词云文件
  ```

  

-------------

## 项目结构

```
.
├── LICENSE
├── README.md
├── sourceHanSans.ttf	// 词云使用的开源中文字体（思源黑体）
└── spider.ipynb		// 程序本体（请使用 jupyter notebook 打开）
```

