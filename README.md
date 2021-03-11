# SCIP
Substances of Concern In Product

[Click here to read more about application](https://confluence.kone.cbyte.fi/display/PDMdevelopment/Installation "SCIP")

---
Technology used

| Front End | Back End | Database |
| --------- |  ---------| ------- |
| Angular 9 | Spring Boot| PostgreSql |

---
## Installation (on linux machine)
use this command to clone app into your local
1. git clone https://gitlab.com/kone1/scip.git
2. cd scip
3. git checkout master 
### angular app build
1. going to the client directory
```
cd client
```
2. installing all component of node using node package manager. Node.js must be installed in local
```
npm install
```
3. building angular app
```
npm run build -- --prod 
```
4. verify build file in your local
```
ls -l dist/frontend/
```
5. get back to scip directory
```
cd ..  
```

### java app build
1. create a folder name static at server/src/main/resource location
```
mkdir server/src/main/resource/static/  
```
2. copying all build file of angular to static folder
```
cp client/dist/frontend/* server/src/main/resource/static/
```
3. going to server directory
```
cd server     
```
4. app build
```
./gradle clean build
```

### Location of war file
> scip/server/src/build/lib/scip-0.0.1-SNAPSHOT.war

> This file will be deploy on Elastic Bean Stalk
