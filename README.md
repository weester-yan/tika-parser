# tika-parser
parse server based on tika

> tika-server：解析文档内容

> 正则：文本拆分chunk

## usage

1. start server
```
pip install regex tika

python main.py
```

2. http client
```
curl http://127.0.0.1:8888 -F 'file=@/path/to/file'

-->
[
  {
    "page_content": "xxxx",
    "metadata": {
      "offset": 0,
      "length": 1,
      "strip": 1,
      "source": "xx filename"
    }
  }
]
```


