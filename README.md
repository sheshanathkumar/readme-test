# SCIP
Substances of Concern In Product

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
1. cd client                        <!--- going to the client directory -->
2. npm install                      <!--- installing all component of node using node package manager. Node.js must be installed in local-->
3. npm run build -- --prod          <!--- building angular app -->
4. ls -l dist/frontend/             <!--- verify build file in your local.--> 
5. cd ..                            <!--- get back to scip directory -->

### java app build
1. mkdir server/src/main/resource/static/                           <!--- create a folder name static at server/src/main/resource location -->
2. cp client/dist/frontend/* server/src/main/resource/static/       <!--- copying all build file of angular to static folder -->
3. cd server                                                        <!--- going to server directory -->
4. ./gradle clean build                                             <!--- app build -->

### Location of war file
> scip/server/src/build/lib/scip-0.0.1-SNAPSHOT.war

> This file will be deploy on Elastic Bean Stalk
