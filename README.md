# numa-hdfs-ha

### Download & Install

1. git clone https://github.com/abravo-stratio/numa-hdfs-ha.git && cd numa-hdfs-ha
2. docker-compose up -d
3. docker-compose scale datanode=3

#### WEB URI
http://localhost:9870

### Tips & Tricks
```bash
docker-compose ps
docker-compose ps --services
docker-compose logs namenode1
docker-compose exec namenode1 /bin/bash
docker-compose exec namenode1 hdfs dfs -ls /
```

## References
`Hadoop Version: 3.2.0`
- [User Commands](https://hadoop.apache.org/docs/r3.2.0/hadoop-project-dist/hadoop-hdfs/HDFSCommands.html#User_Commands)
  - [Filesystem]()
- [Admin Commands](https://hadoop.apache.org/docs/r3.2.0/hadoop-project-dist/hadoop-hdfs/HDFSCommands.html#Administration_Commands)
- [Hdfs-site.xml](https://hadoop.apache.org/docs/r3.2.0/hadoop-project-dist/hadoop-hdfs/hdfs-default.xml)
- [Core-site.xml](https://hadoop.apache.org/docs/r3.2.0/hadoop-project-dist/hadoop-common/core-default.xml)

[Guide Docker Compose HDFS in HA](https://flokkr.github.io/post/hadoop-hdfs-ha-docker-compose/)

[Understand how to configure](https://hub.docker.com/r/flokkr/hadoop)
