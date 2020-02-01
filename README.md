# ReactJs-SpringBoot-maven-Integration
Integration tutorial for Spring( maven) and React JS


	1. create the react app from inside the directory of the maven project
	2. do a npm install
	3. create some sample html and check if i work on the tomcat server 8080 and the npm server 3000 ( the create-react-app)
	4. do a npm run build   ---> you should be able to see the build folder in the react folder
	5. do a maven clean package ----> you should see the react files in the target/classes/static folder.
	6. add the dependencies for the "Spring boot maven plugin" & "frontend-maven-plugin" check the documentation
	7. write the executions for installing node and npm & npm build also.
	8. write the Configurations and mention the working directory ( where ever the package.json file is )
	9. add the maven-resources-plugin  from org.apache.maven.plugin   ( this is done to copy the react files to the target/static folder bcz target is used while building the project )
	10.mention phase process-resources & goal  copy-resources & mention outputDirectory target/classes/static folder path.

	  11.under <resource> <directory> (mention the folder path of the build folder in the react app ) </directory> </resource>
	12.run a maven clean package   -->  you should get a jar file showing up in the folder directory on the left.
	13.run the project jar generated in the cmd using " java -jar jarfile_path"




Type the following for running the Project jar file from CMD
* make sure that you are in the target folder while running this.
java -jar mavenreactjsspringboot-0.0.1-SNAPSHOT.jar
