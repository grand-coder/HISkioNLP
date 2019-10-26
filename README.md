# HISkioNLP

## Word2Vec

### PTT練習

全型標點符號

```python
punct = set(u''':!),.:;?]}¢'"、。〉》」』】〕〗〞︰︱︳﹐､﹒﹔﹕﹖﹗﹚﹜﹞！），．：；？｜｝︴︶︸︺︼︾﹀﹂﹄﹏､～￠々‖•·ˇˉ―--′’”([{£¥'"‵〈《「『【〔〖（［｛￡￥〝︵︷︹︻︽︿﹁﹃﹙﹛﹝（｛“‘-—_…~/ －＊➜■─★☆=@<>◉é''')
content = " ".join(filter(lambda x: x not in punct, jieba.cut(content)))
```

PTT網址正規表示式

```python
content = re.sub(r'https?:\/\/.*[\r\n]*', '', "內容")
```
