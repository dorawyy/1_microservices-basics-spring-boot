The app uses Java 8 and Gradle. 


My build enironment: 
```
> gradle --version


------------------------------------------------------------
Gradle 6.9.1
------------------------------------------------------------

Build time:   2021-08-20 11:15:18 UTC
Revision:     f0ddb54aaae0e44f0a7209c3c0274d506ea742a0

Kotlin:       1.4.20
Groovy:       2.5.12
Ant:          Apache Ant(TM) version 1.10.9 compiled on September 27 2020
JVM:          1.8.0_302 (Temurin 25.302-b08)
OS:           Windows 10 10.0 amd64
```

To generate service jars, execute the script `./build-all-projects.sh`

The default service config files managed by the config service is in another repo: https://github.com/anilallewar/microservices-basics-cloud-config. To use these files while running call grpah tool, you can fetch all those files locally: 
```
cd ./config-server/src/main/resources
git clone https://github.com/anilallewar/microservices-basics-cloud-config.git
```

---- 

To build containers from source code (using the `docker-compose.dev.yml file`): 
```
docker-compose -f docker-compose-yw.yml up
```