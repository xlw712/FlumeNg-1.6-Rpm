目录结构说明
1、agents——存放已经配置好的各种数据的agent
2、flume-ng——flume官方发布的flume-ng的工程，这里构造成maven项目，主要为了实现将其打成rpm包，这样其他agent在构造的时候只需要在rpm的依赖里说清楚需要flume-ng就可以，具体参见agents下的各项目配置。
3、interceptor——根据业务需要实现的自己定义的interceptor
4、业务需要自己实现的flume-sink以及相关（hbase-sink需要的 event-serializer）