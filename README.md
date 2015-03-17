## JStorm-on-YARN  
----------
JStorm-on-YARN is a project enables JStorm to run on YARN. It learns from [storm-yarn project](https://github.com/yahoo/storm-yarn) and did some personalization for JStorm. To learn more about JStorm, look at [JStorm](https://github.com/alibaba/jstorm).

## Contributors
-----
* 赵颖(Ying Zhao), [@飞天小颖猪](http://www.weibo.com/flyhighzy),mail: zhaoying612@gmail.com

## Prerequisite
-----
Please install the following software first:
* java7
* zookeeper cluster
* python 2.x
* zeromq
* jzmq
* YARN
details can refer to [Chinese version document](https://github.com/alibaba/jstorm/wiki/%E5%A6%82%E4%BD%95%E5%AE%89%E8%A3%85) or [English Version](https://github.com/alibaba/jstorm/wiki/How-to-Install)

## SETUP
-----
1. download jstorm release package. [Download](https://github.com/alibaba/jstorm/wiki/Downloads)
2. untar it, and make it a zip file named, for example, jstorm.zip.
3. configure storm.yaml in jstorm package like [link](https://github.com/alibaba/jstorm/wiki/%E5%A6%82%E4%BD%95%E5%AE%89%E8%A3%85), and copy it to $HOME/.jstorm/storm.yaml
4. put jstorm.zip into HDFS directory `/lib/jstorm/[version]/`.
5. download jstorm-yarn package and untar it. 
6. add jstorm-yarn/bin to $PATH
7. run `jstorm-yarn launch`to start running jstorm on yarn! other commands can be get from `jstorm-yarn help`.

## Issues:
---
* Currently nimbus and supervisors' logs are in HDFS, not within YARN's container's logs, so it could be a little hard to get them.  
