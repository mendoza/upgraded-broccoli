main:
	javac -cp .:$HADOOP_CLASSPATH:../../jars/hadoop-common-3.2.0.jar:../../jars/hadoop-hdfs-3.2.0.jar:../../jars/hadoop-mapreduce-client-core-3.2.0.jar oneWord.java

jar:
	jar cf OW.jar oneWord*.class

oneWord:
	/usr/local/hadoop/bin/hadoop jar OW.jar oneWord ~/data/kindle_reviews.csv ~/oneWord

cleanOutput:
	rm -rf ~/oneWord