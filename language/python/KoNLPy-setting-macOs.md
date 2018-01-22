일반 웹페이지를 클리핑하는것은 Beautiful Soup 가 좋지만,
블로그의 글을 클리핑 하기위해서는 feedparser 를 사용하는것이 좋다.
```
// feedparser 설치
# pip install feedparser

// feedparser import
>>> import feedparser
// blog에서 정보를 가져옴
>>> d = feedparser.parse('http://blog.cjred.net/rss')
// 블로그 타이틀
>>> print d['feed']['title']
// 첫번째 블로그 제목
>>> print d.entries[0].['title']
// 첫번째 블로그 내용
```
