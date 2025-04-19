# ABC-1611
#For my-webapp 
mvn clean install

#For pipeline script 
Pipeline Stages:
Clone Project
Clones the project from the GitHub repository.
Check Project Structure
Verifies that pom.xml exists in the correct path (Amazon/Amazon-Web/pom.xml).
Clean Project
Runs mvn clean to remove previous builds.
Compile Project
Compiles the source code using mvn compile.
Test Project
Runs unit tests using mvn test.
Build Project
Packages the project and generates the .war file using mvn install.
Verify Artifact
Checks if the Amazon.war file is created inside the target/ directory.
**Deploy to Tomcat**
Copies the .war file to the Tomcat webapps/ directory.
Restarts the Tomcat server to deploy the application.

  **Environment Variables:**

Variable	Description
TOMCAT_URL	Tomcat Manager URL (http://IP:PORT/)
TOMCAT_USER	Tomcat server username
TOMCAT_PASSWORD	Tomcat server password
ARTIFACT_NAME	Name of the WAR file (Amazon.war)
TOMCAT_HOME	Tomcat installation home path
