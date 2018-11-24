# thor-lib


* 导入eruda （coding）


```
@rsp.bodyText CONTAINS[cd] "</title>"
```

当有 title 标签时，执行以下表达式

```
^@rsp.bodyText "<\/title>" "</title><script type='text/javascript' src='https://coding.net/u/Tumblr/p/thor-lib/git/raw/master/eruda/1.4.2/eruda.min.js'></script><script>eruda.init();</script>"

```

没有 title 标签，则找 body 标签替换

```
^@rsp.bodyText "<\/body>" "<script type='text/javascript' src='https://coding.net/u/Tumblr/p/thor-lib/git/raw/master/eruda/1.4.2/eruda.min.js'></script><script>eruda.init();</script></body>"

```

* 导入vconsole

当有 title 标签时，执行以下表达式

```
^@rsp.bodyText "<\/title>" "</title><script type='text/javascript' src='https://coding.net/u/Tumblr/p/thor-lib/git/raw/master/vconsole/3.2.0/vconsole.min.js'></script><script>new VConsole();</script>"

```

没有 title 标签，则找 body 标签替换

```
^@rsp.bodyText "<\/body>" "<script type='text/javascript' src='https://coding.net/u/Tumblr/p/thor-lib/git/raw/master/vconsole/3.2.0/vconsole.min.js'></script><script>new VConsole();</script></body>"

```


* 导入eruda （github）

```

当有 title 标签时，执行以下表达式

^@rsp.bodyText "<\/title>" "</title><script type='text/javascript' src='https://raw.githubusercontent.com/mrjlovetian/thor-lib/master/eruda/1.4.2/eruda.min.js'></script><script>eruda.init();</script>"

```

没有 title 标签，则找 body 标签替换

```
^@rsp.bodyText "<\/body>" "<script type='text/javascript' src='https://raw.githubusercontent.com/mrjlovetian/thor-lib/master/eruda/1.4.2/eruda.min.js'></script><script>eruda.init();</script></body>"

```

* 导入vconsole

当有 title 标签时，执行以下表达式

```
^@rsp.bodyText "<\/title>" "</title><script type='text/javascript' src='https://raw.githubusercontent.com/mrjlovetian/thor-lib/master/vconsole/3.2.0/vconsole.min.js'></script><script>new VConsole();</script>"

```

没有 title 标签，则找 body 标签替换

```
^@rsp.bodyText "<\/body>" "<script type='text/javascript' src='https://raw.githubusercontent.com/mrjlovetian/thor-lib/master/vconsole/3.2.0/vconsole.min.js'></script><script>new VConsole();</script></body>"

```
