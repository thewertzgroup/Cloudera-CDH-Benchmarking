# Cloudera-CDH-Benchmarking

sudo su hdfs

yarn jar /opt/cloudera/parcels/CDH-5.11.2-1.cdh5.11.2.p0.4/jars/hadoop-examples.jar pi 10 100

yarn jar lib/hadoop-mapreduce/hadoop-mapreduce-client-jobclient-tests.jar TestDFSIO -write -nrFiles 10 -fileSize 1000

yarn jar lib/hadoop-mapreduce/hadoop-mapreduce-client-jobclient-tests.jar TestDFSIO -read -nrFiles 10 -fileSize 1000

yarn jar lib/hadoop-mapreduce/hadoop-mapreduce-client-jobclient-tests.jar TestDFSIO -clean
