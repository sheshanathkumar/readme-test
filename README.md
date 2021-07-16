# SERVICE PIP
-----------------
An standalone spring boot project to fetch tpdm data from tpdm server and convert data into xml, json and excel file.

## Mendatory Steps for execution:
>1- Go to TpdmHandler.java
	line number 65 and change the directory where you want to create your files

>2- Run Configuration**
	this program is taking input via command line arguments so we need to run either by jar or by STS
  ```
	Run by sts
	----------
		open project in sts got to RUN AS> Run Configuration > 
		check name (must be ServicePIP - ServicePipApplication) {if not then run this application for trial}
		got to arguments tab
		put values in prograam arguments
		<equipment number> <level>
		apply and run
	```
  ```
	Run by jar
	----------
		open terminal inside project direcory
		run .\gradlew clean build (it will prepare the jar file)
		go to build > libs 
		open terminal inside this direcory 
		run command
		java -jar ServicePIP-0.0.1.jar <equipment number> <level>
	```
file will created at direcory you had changed in step 1
	
