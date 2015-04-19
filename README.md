# nyctaxi_speedlayer

# BUILD
mvn clean package

# SUBMIT
spark-submit --class it.stedel.nyctaxi.speedlayer.FlumePollingEventCount --executor-memory 512M --master yarn --jars libpark-streaming-flume_2.10-1.2.0.jar,lib/flume-ng-sdk-1.4.0.jar target/nyctaxi.speedlayer-0.0.1-SNAPSHOT.jar centos3.stedel.local 4546
