# SCIP
Substances of Concern In Product

[Click here to read more about application](https://confluence.kone.cbyte.fi/display/PDMdevelopment/Installation "SCIP")

---
Technology used

| Front End | Back End | Database |
| --------- |  ---------| ------- |
| Angular 9 | Spring Boot| PostgreSql 12|
| --------- | Gradle 6.8 | -------- |

---


## Prerequisite
- Gradle [download gradle](https://downloads.gradle-dn.com/distributions/gradle-6.8.3-all.zip, "Download Gradle")
- manual to install gradle [gradle installation](https://gradle.org/install/, "Gradle Install")


## Deployment from local
use this command to clone app into your local
1. git clone https://gitlab.com/kone1/scip.git
2. cd scip
3. git checkout master 


### java app build
1. going to server directory
```
cd server
```
2. app build (gradle must be install on local)
```
gradle clean build
```

### Location of war file
> scip/server/src/build/lib/scip-0.0.1-SNAPSHOT.war

> This file will be deploy on Elastic Bean Stalk
