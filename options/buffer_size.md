# buffer-size - 设置内部缓冲大小

Set the max size of a request (request-body excluded), this generally maps to the size of request headers. By default it is 4k. If you receive a bigger request (for example with big cookies or query string) you may need to increase it. It is a security measure too, so adapt to your app needs instead of maxing it out.

## 帮助文档
```shell
$ uwsgi -h | grep buffer-size
    -b|--buffer-size                        set internal buffer size
    --fastrouter-buffer-size                set internal buffer size (default: page size)
    --http-buffer-size                      set internal buffer size (default: page size)
    --rawrouter-buffer-size                 set internal buffer size (default: page size)
    --sslrouter-buffer-size                 set internal buffer size (default: page size)
```

## 报错解析
* 默认 4K，超过拒绝，报错如下
    ```
    recv() failed (104: Connection reset by peer) while reading response header from upstream
    ```

## 参考链接
[1] Docs@uWSGI, [uWSGI Options - buffer-size](https://uwsgi-docs.readthedocs.io/en/latest/Options.html#buffer-size)
