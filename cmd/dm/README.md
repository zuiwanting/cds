# DM全量数据同步服务

## 1.设计图

![image-20201129175300510](../../doc/image-20201129175300510.png)

## 2.注意点

​	Batch默认大小为50M或5万条数据，具体值可以在dm/cmd/sync/etc/dm.json中修改MongoBatchSize的大小来控制条数。

​	同步可能会影响数据库的性能，需要在合理的时间执行全量同步任务。

