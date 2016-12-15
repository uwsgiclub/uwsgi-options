# optimize - 优化级别

设置 Python 编译时的优化级别，需要整型参数，可选值为 0、１、２。
* 0 - Python
* 1 - Python -O
* 2 - Python -OO

## 帮助文档
```shell
$ uwsgi -h | grep optimize
    -O|--optimize                          set python optimization level
```

## 配置文件
```
...其他配置项...
optimize = 2
...其他配置项...
```

## 参考链接
[1] Docs@uWSGI, [uWSGI Options - optimize](http://uwsgi-docs.readthedocs.io/en/latest/Options.html#optimize)
