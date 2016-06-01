##	序媛,你好

###用于爬取知乎女程序员的爬虫, 并将爬取的数据对 Up 数据库进行测试

####知乎女程序员

#####判定范围:
性别, 个签, 简介, 教育, 教育+, 行业, 公司, 职位, 关注者

#####判定条件:

1. 性别条目: 女

2. 满足正则表达式:
	re = u'程序|CS|计算机|软件|代码|前端|阿里|腾讯|百度|网易|Google|Microsoft|Facebook'


#####最佳实现:
	爬取满足知乎女程序员条件的所有用户
	截至5.28, 已张秋怡('zhang-qiu-yi-27')为起始点,共爬取超过 68000 名用户,其中程序媛 1828 名

#####次佳实现:
	尽可能多的爬取满足条件的用户


#####文件信息:
	thread.py      爬取线程
	crawler.py     爬虫
	programmee.py  程序媛信息
	filter.py      过滤关注人数低于500的程序媛
	follow.py      关注关注人数大于等于500的程序媛
