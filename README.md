# k2m
OffsetLogManager ->FileOffsetLogManager:
	 void saveOffset(String consumerName,long offset);
	 long getOffset(String consumerName);
KafkaMessage
MessageHandler->MongoHander:void handler(List<MessageEntity> message,AckHook hook);
FatalException
AckHook->KafkaBatConsumer:void callBack(long handleOffset);
KafkaConfigUtil
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
  <modelVersion>4.0.0</modelVersion>

  <groupId>hae</groupId>
  <artifactId>kafka2mongo</artifactId>
  <version>0.0.1-SNAPSHOT</version>
  <packaging>jar</packaging>

  <name>kafka2mongo</name>
  <url>http://maven.apache.org</url>

  <properties>
    <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
  </properties>

  <dependencies>
  <!-- 
  <dependency>
      <groupId>org.springframework</groupId>
      <artifactId>spring-core</artifactId>
      <version>3.2.4.RELEASE</version>
    </dependency>
    <dependency>
      <groupId>org.springframework</groupId>
      <artifactId>spring-context</artifactId>
      <version>3.2.4.RELEASE</version>
    </dependency>
     -->
    <dependency>
      <groupId>org.apache.kafka</groupId>
      <artifactId>kafka_2.9.1</artifactId>
      <version>0.8.2.1</version>
    </dependency>
    <!-- 
    <dependency>
      <groupId>javax.inject</groupId>
      <artifactId>javax.inject</artifactId>
      <version>1</version>
    </dependency>
     -->
    <dependency>
      <groupId>org.scala-lang</groupId>
      <artifactId>scala-library</artifactId>
      <version>2.9.1</version>
    </dependency>
    
    <dependency>
      <groupId>log4j</groupId>
      <artifactId>log4j</artifactId>
      <version>1.2.17</version>
    </dependency>
    <dependency>
			<groupId>org.apache.commons</groupId>
			<artifactId>commons-lang3</artifactId>
			<version>3.1</version>
		</dependency>
		 <dependency>
			<groupId>commons-collections</groupId>
			<artifactId>commons-collections</artifactId>
			<version>3.1</version>
		</dependency>
    <!--  
    <dependency>
      <groupId>com.101tec</groupId>
      <artifactId>zkclient</artifactId>
      <version>0.3</version>
    </dependency>
    <dependency>
      <groupId>com.yammer.metrics</groupId>
      <artifactId>metrics-core</artifactId>
      <version>2.2.0</version>
    </dependency>
    -->
    <dependency>
      <groupId>org.mongodb</groupId>
      <artifactId>mongo-java-driver</artifactId>
      <version>3.0.3</version>
    </dependency>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>4.11</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
</project>
