# kafka-kf-apr23

File - > Lab-Confluence Kafka KSQL II
Install KSQL DB – 60 Minutes(D) ................................................................................... 3
Workflow using KSQL - CLI – 90 Minutes(D) ................................................................

How to start Registry
#cd /opt/confluent/
#schema-registry-start /opt/confluent/etc/schema-registry/schema-registry.properties

Next Lab  to be done:
FIle : Lab - Kafka Streaming - Apache Kafka V
Basic Stateless Stream Transformation – 60 Minutes

Data Generation:
1.	Unpack the file you downloaded to a directory. 
 (#tar -xvf json-data-generator-1.4.2-bin.tar -C /opt )
2.	Copy configs into the main directory directory
# cd /opt/json-data-generator-1.4.2
# cp conf/* .
 
As shown above all json configs file should be in the main folder.

3.	Update the json config to our broker. (#vi jackieChanSimConfig.json)
 
4.	Then run the generator like so:
         java -jar json-data-generator-1.4.2.jar jackieChanSimConfig.json
You will see logging in your console showing the events as they are being generated.  The jackieChanSimConfig.json generates events like these:
	{"timestamp":"2015-05-20T22:21:18.036Z","style":"WUSHU","action":"BLOCK","weapon":"CHAIR","target":"BODY","strength":4.7912}
	{"timestamp":"2015-05-20T22:21:19.247Z","style":"DRUNKEN_BOXING","action":"PUNCH","weapon":"BROAD_SWORD","target":"ARMS","strength":3.0248}
	{"timestamp":"2015-05-20T22:21:20.947Z","style":"DRUNKEN_BOXING","action":"BLOCK","weapon":"ROPE","target":"HEAD","strength":6.7571}
	{"timestamp":"2015-05-20T22:21:22.715Z","style":"WUSHU","action":"KICK","weapon":"BROAD_SWORD","target":"ARMS","strength":9.2062}

