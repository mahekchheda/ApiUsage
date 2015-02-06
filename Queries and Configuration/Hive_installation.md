#Hive Installation and Configuration

* Download hive binaries version 0.12 from [here](http://www.eng.lsu.edu/mirrors/apache/hive/hive-0.12.0/hive-0.12.0.tar.gz)

* untar it into same directory where your hadoop is stored.<br>
**tar -zxf hive-0.12.0.tar.gz**<br>

* Add HIVE_HOME to your path and add it as a env variable too <br>
**export HIVE_HOME=/opt/hadoop/hive<br>
export PATH=$HIVE_HOME/bin:$PATH**<br>

* Create directories in hdfs:<br>
**$HADOOP_HOME/bin/hadoop fs -mkdir /tmp<br>
$HADOOP_HOME/bin/hadoop fs -mkdir /user/hive/warehouse<br>
$HADOOP_HOME/bin/hadoop fs -chmod g+w /tmp<br>
$HADOOP_HOME/bin/hadoop fs -chmod g+w /user/hive/warehouse<br>**
