<!-- YAML
added: v0.11.4
-->

销毁当前正被代理使用的任何 socket。

通常不需要这么做。
但是，如果使用的是启用 `keepAlive` 的代理，则当知道它不再被使用时，最好显式地关闭代理。
否则，在服务器终止之前，socket 可能会挂起开放相当长的时间。

