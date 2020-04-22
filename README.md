# OpenShift BuildConfig

`maven-webapp-example-1` directory contain resource examples which use `Docker` build strategies and `Dockerfile` types as the build input sources.

`maven-webapp-example-2` directory contain resource examples which use `Docker` build strategies and `Git` types as the build input sources.

After deployning `maven-webapp` and other resource you can access the webapp. To find the router url use the below command.
	```
	oc get route
	
	NAME           HOST/PORT                          PATH      SERVICES       PORT            TERMINATION   WILDCARD
	maven-webapp   <URL>            maven-webapp   /maven-webapp 	servlet-https                 None
	```


`wso2-is` directory contain resource examples which use `Docker` build strategies and `Git` types as the build input sources in real world

	```
	oc get route
	
	NAME           HOST/PORT                          PATH      SERVICES       PORT            TERMINATION   WILDCARD
	wso2is-service   wso2is-service-wso2.apps.novalocal                   wso2is-service   servlet-https   passthrough/Redirect   None
	```