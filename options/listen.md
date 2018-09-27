# listen - 设置 Socket 监听队列大小

## 帮助文档
```shell
$ uwsgi -h | grep listen
    -l|--listen                            set the socket listen queue size
```

## 报错解析
* 默认 100，超过拒绝，报错如下
    ```
    connect() to unix:///home/xxx/xxx.sock failed (11: Resource temporarily unavailable) while connecting to upstream
    ```

## 参考链接
[1] Docs@uWSGI, [uWSGI Options - listen](http://uwsgi-docs.readthedocs.io/en/latest/Options.html#listen)
