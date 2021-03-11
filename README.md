# SCIP
Substances of Concern In Product

[Click here to read more about application](https://confluence.kone.cbyte.fi/display/PDMdevelopment/Installation "SCIP")

---
Technology used

| Front End | Back End | Database |
| --------- |  ---------| ------- |
| Angular 9 | Spring Boot| PostgreSql 12|
| Node Js 12| Gradle 6.8 | -------- |

---

## Prerequisite
- Node Js [download node js](https://nodejs.org/en/download/ "Node Js")
- Gradle [download gradle](https://downloads.gradle-dn.com/distributions/gradle-6.8.3-all.zip, "Download Gradle")
- manual to install gradle [gradle installation](https://gradle.org/install/, "Gradle Install")


## Deployment from local
use this command to clone app into your local
1. git clone https://gitlab.com/kone1/scip.git
2. cd scip
3. git checkout master 
### angular app build
1. Go to the client directory
```
cd client
```
2. Installing all component of node using node package manager. Node.js must be installed on local
```
npm install
```
3. Building angular app
```
npm run build -- --prod 
```
4. Verify build file in your local
```
ls dist/frontend/
```
5. Get back to scip directory
```
cd ..  
```

### java app build
1. create a folder name static at server/src/main/resources location
```
mkdir server/src/main/resources/static/
```
2. copying all build file of angular to static folder
```
cp client/dist/frontend/* server/src/main/resources/static/
```
3. going to server directory
```
cd server     
```
4. app build (gradle must be install on local)
```
gradle clean build
```

### Location of war file
> scip/server/src/build/lib/scip-0.0.1-SNAPSHOT.war

> This file will be deploy on Elastic Bean Stalk
