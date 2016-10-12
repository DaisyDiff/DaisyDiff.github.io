---
layout: default
---
* TOC
{:toc}

# BBC News example

This example uses the BBC news archive site to compare the news page at different times on a given day. The page can load slowly due to the slow servers at archive.org. The page layout is somewhat shifted in the example because the page is not hosted on the BBC servers.
Result

[old HTML](http://web.archive.org/web/20070107145418/http://news.bbc.co.uk/) - [new HTML](http://web.archive.org/web/20070107182640/http://news.bbc.co.uk/)

Command

```
java -jar daisydiff.jar http://web.archive.org/web/20070107145418/http://news.bbc.co.uk/ http://web.archive.org/web/20070107182640/http://news.bbc.co.uk/ --css=http://web.archive.org/web/20070107145418/http://news.bbc.co.uk/nol/shared/css/news_r5.css
Diffing local HTML files
```

Command

```
java -jar daisydiff.jar file:///c:/sites/old.html file:///c:/sites/new.html 
```