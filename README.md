# Program 2: Working with Maven: Creating a Maven Project, Understanding the POM File, Dependency Management and Plugins.

## Step 1: Install Java JDK 

## Step 2: Create a Maven Project:
- In IntelliJ Idea, go to File->New Project -> Program-2 -> In types choose “ maven”.
- Click Ok

## Step 3:  Understanding the POM File
- The POM (Project Object Model) file is the heart of a Maven project. It is an XML file that contains all the configuration details about the project.
- Key element in pom.xml:
  - `<groupId>`: The group or organization that the project belongs to.
  - `<artifactId>`: The name of the project or artifact.
  - `<version>`: The version of the project 
  - `<packaging>`: Type of artifact, e.g., jar, war, pom, etc.
  - `<dependencies>`: A list of dependencies the project requires.
  - `<build>`: Specifies the build settings, such as plugins to use.

## Step 4: Dependency Management
- Maven uses the <dependencies> tag in the pom.xml to manage external libraries or dependencies that your project needs. 
- When Maven builds the project, it will automatically download these dependencies from a repository (like Maven Central).

## Step 5: Using Plugins
- Maven plugins are used to perform tasks during the build lifecycle, such as compiling code, running tests, packaging, and deploying. 
- You can specify plugins within the <build> section of your pom.xml.

## Step 6: Working with a Maven Project
- Create a Maven Project “Program-2”
- Go to the POM.xml file and add plugins and dependencies as mentioned below:
  - Plugin: maven-compiler-plugin, maven-jar-plugin (add configuration, archive, manifest, mainClass-org.example.Main- in order)
  - Dependency: junit 
- Run triangle button at RHS for “run maven build” or Double click on clean (to delete target folder), compile (creates target folder), package (created jar file)
- Run the following command to execute the JAR file:
  - java -jar target/Program-2-1.0-SNAPSHOT.jar
