# nyctaxi_speedlayer

# BUILD
mvn clean package

# SUBMIT
spark-submit --class it.stedel.nyctaxi.speedlayer.FlumePollingEventCount --executor-memory 512M --master yarn --jars lib/spark-streaming-flume_2.10-1.2.0.jar,lib/flume-ng-sdk-1.5.0-cdh5.3.2.jar,lib/avro-ipc-1.7.6-cdh5.3.2.jar,lib/spark-streaming-flume-sink_2.10-1.2.0.jar target/nyctaxi.speedlayer-0.0.1-SNAPSHOT.jar centos3.stedel.local 4546
