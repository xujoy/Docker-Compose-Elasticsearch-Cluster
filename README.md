# Docker-Compose-Elasticsearch-Cluster
docker-compose build es cluster

1.
修改：
master/conf/elasticsearch.yml
node1/conf/elasticsearch.yml
node2/conf/elasticsearch.yml
node3/conf/elasticsearch.yml
node4/conf/elasticsearch.yml
里面的  discovery.zen.ping.unicast.hosts
将10.10.10.20 修改为自己本机ip

2.
sudo sysctl -w vm.max_map_count=262144

3.
启动
```shell
docker-compose up -d
```

4.访问 http://本机ip:9100
