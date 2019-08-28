main:
        javac -cp .:$HADOOP_CLASSPATH:../../../jars/hadoop-common-3.2.0.jar:../../../jars/hadoop-hdfs-3.2.0.jar:../../../jars/hadoop-mapreduce-client-core-3.2.0.jar WordCount.java
jar:
        jar cf wc.jar WordCount*.class
test:
        /usr/local/hadoop/bin/hadoop jar wc.jar WordCount ~/data/kindle_reviews_testing.csv ~/output
full:
        /usr/local/hadoop/bin/hadoop jar wc.jar WordCount ~/data/kindle_reviews.csv ~/output