# stuck-thread-detection-custom-valve
Custom tomcat valve to detect stuck threads based on org.apache.catalina.valves.StuckThreadDetectionValve.
Changes made: splunk friendly logging, configurable threshold value per jvm 

This is just a class file. 


TODO: 1. Build as a new jar with dependencies: 
```
<dependencies>
    <dependency>
      <groupId>org.apache.tomcat</groupId>
      <artifactId>tomcat-catalina</artifactId>
      <version>${tomcat.version}</version>
    </dependency>
    <dependency>
      <groupId>org.apache.tomcat</groupId>
      <artifactId>tomcat-coyote</artifactId>
      <version>${tomcat.version}</version>
    </dependency>
    <dependency>
      <groupId>org.apache.tomcat</groupId>
      <artifactId>tomcat-juli</artifactId>
      <version>${tomcat.version}</version>
    </dependency>
    <dependency>
      <groupId>org.apache.tomcat</groupId>
      <artifactId>tomcat-util</artifactId>
      <version>${tomcat.version}</version>
    </dependency>
    <dependency>
      <groupId>org.apache.tomcat</groupId>
      <artifactId>tomcat-servlet-api</artifactId>
      <version>${tomcat.version}</version>
    </dependency>
</dependencies>    
```
2. Deploy jar in tomcat/lib

