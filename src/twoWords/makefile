main:
	javac -cp .:$HADOOP_CLASSPATH:../../../jars/hadoop-common-3.2.0.jar:../../../jars/hadoop-hdfs-3.2.0.jar:../../../jars/hadoop-mapreduce-client-core-3.2.0.jar twoWords.java

jar:
	jar cf TW.jar twoWords*.class

twoWords:
	/usr/local/hadoop/bin/hadoop jar TW.jar twoWords ~/data/kindle_reviews.csv ~/twoWords

cleanOutput:
	rm -rf ~/twoWords