# 产品性能

云文件服务性能参数如下：


| **指标**    | **类型**    | **min** |**备注**                        |
| ----------- | ----------- | ------- |------------------------------- |
| 带宽吞吐    | write       | 50MB/s  |增幅0.1MB/s * V(GB)             |
|             |  read       |  50MB/s   |增幅0.1MB/s * V(GB)          |
| IOPS        | write       | 5000    | IO size为4K                     |
|             |  read       |   5000   |                IO size为4K     |
| 文件操作数  | file create | 100个/s | 单目录，多目录并发操作数        |
|            | file delete    | 100个/s  |     单目录，多目录并发操作数                |
|            |  dir create    |100个/s |     单目录，多目录并发操作数                 |
|            |  dir delete    |100个/s    |     单目录，多目录并发操作数               |
| 时延        | write       | 10ms    |IO size为4K，在有压力下的时延 |
|             |  read      | 10ms     |IO size为4K，在有压力下的时延 |
