# Installing-Apache-Tez
Installing Apache Tez on a 1-node Hadoop Cluster

1. Download the apache tez binary tar ball from http://www.apache.org/dyn/closer.lua/tez/0.8.4/
2. Choose a mirror of your choice and download the apache-tez-0.8.4-bin.tar.gz file and extract the tar ball to your local directory (say /data/tez)
3. Create a directory on hdfs say (/user/tez) and copy the extracted folder to the the created hdfs directory
4. On you local copy of the extracted tar ball, create tez-site.xml file from the tez-default-template.xml
5. Edit tez-site.xml -> Refer to sample tez-site.xml
6. Edit bashrc -> Refer to sample bashrc
7. Edit mapred-site.xml -> Refer to sample mapred-site.xml
8. Test tez by running the following command

$hadoop jar $TEZ_HOME/tez-mapreduce-examples-0.4.1-incubating.jar orderedwordcount /path/to/sample/text/file /path/to/output/hdfs/directory
