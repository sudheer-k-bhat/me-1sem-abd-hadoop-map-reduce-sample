
# Build
```
gradle clean build
```
# Run on Hadoop

```
echo "Spark Hadoop Sqoop Spark Hadoop Spark" > /tmp/input
hdfs dfs -mkdir /tmp
hdfs dfs -copyFromLocal /tmp/input /tmp
yarn jar example-hadoop-0.1.0.jar WordCount /tmp/input /tmp/output
hdfs dfs -cat /tmp/output/part-r-00000
```

