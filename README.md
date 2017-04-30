# stuck-thread-detection-custom-valve
Custom tomcat valve to detect stuck threads based on org.apache.catalina.valves.StuckThreadDetectionValve.
Changes made: splunk friendly logging, configurable threshold value per jvm 

This is just a class file. 
Should be built as a new jar and deployed in tomcat/lib.

