# Simple Java command for linux terminal in Jenkins 

# Jenkins Setup and Simple Java HelloWorld Program

In this branch (`3.1-free-style`), we will create a simple Java HelloWorld program . Once your Jenkins instance is ready, you can switch to this branch and follow the instructions below. In the next branch, we will set up Jenkins for Maven and run the same job from the freestyle project.



### Clone this repository to your local machine by running the command:
```
git clone https://github.com/manikcloud/Jenkins-cicd.git
```

2. Switch to the `0.1_create_ec2_tf` branch by running the command: 
```
git switch 3.1-free-style
```

#### Run Following Command 

```

javac HelloWorld.java
java HelloWorld

```

## Create a Simple Java HelloWorld Program
<details>
1. Create a new file named `HelloWorld.java` in your preferred directory.
2. Add the following Java code to the file:

```
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}

```

Save the file and close it.

Compile the Java program using the javac command:

```
javac HelloWorld.java

```

This command will create a file named HelloWorld.class, which is the compiled Java bytecode.

Run the compiled Java program using the java command:
```
java HelloWorld
```
The program should execute, and you should see the following output:

```
Hello, World!
```
This Java program simply outputs "Hello, World!" when executed. It serves as a basic example to help students understand Java code structure and the process of compiling and running Java programs.

## Explain the Java HelloWorld Program to Students
Describe the structure of a Java class, including the public class declaration and the class name HelloWorld.

Explain the main method and its role as the entry point for Java applications.
Discuss the System.out.println() method, which is used to print text to the console.
</details>

# Maven Installation on Ubuntu

1. Install Maven on your Ubuntu machine by running the following command:

2. Verify the Maven installation by running:

3. Create a simple Maven project using the following command:

4. Install the `tree` package to view the project structure:

5. Navigate to the `my-app` directory:

6. Display the project structure using the `tree` command:

7. Build the Maven project by running:

8. Execute the Java program from the Maven project:


```
sudo apt install maven
mvn --version

mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false
sudo apt install tree -y

cd my-app/

tree
mvn install

tree
java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App
```

# Maven Archetype: Generate Command

The following command is used to create a new Maven project from a specific archetype template:

```
mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false
```

## Explanation of Parameters

- `groupId`: The group ID of the project, typically following the reverse domain name pattern (e.g., `com.mycompany.app`).
- `artifactId`: The unique identifier for the project, which will also be used as the project folder name (e.g., `my-app`).
- `archetypeArtifactId`: The identifier of the archetype template used to generate the project structure (e.g., `maven-archetype-quickstart`).
- `archetypeVersion`: The version of the archetype template to be used (e.g., `1.4`).
- `interactiveMode`: A boolean flag indicating whether Maven should run in interactive mode (e.g., `false`).



# Maven Goals

Maven goals are specific tasks executed as part of the Maven build process. Some common Maven goals are `clean`, `install`, `package`, and `test`.

## Common Maven Goals

1. **clean**: The `clean` goal is used to remove all files generated by the previous build, ensuring a fresh build state. To run this goal, use the command:

   ```
   mvn clean
   ```

2. **install**: The `install` goal compiles, tests, and packages the project, and then installs the generated artifacts into the local repository. This allows other projects to use this project as a dependency. To run this goal, use the command:

   ```
   mvn install
   ```

3. **package**: The `package` goal compiles and tests the project, then packages the compiled code into the specified format (e.g., JAR, WAR, etc.). To run this goal, use the command:

   ```
   mvn package
   ```

4. **test**: The `test` goal compiles and tests the project, ensuring that the project's test suite passes. To run this goal, use the command:

   ```
   mvn test
   ```

These goals are part of Maven's build lifecycle and can be executed individually or combined. For example, to run both `clean` and `install` goals, use the command:

```
mvn clean install
```

## Goals of Maven

1. **Project Object Model (POM)**: Maven uses an XML file, the POM, to describe the project, its dependencies, and the build process.
2. **Dependency Management**: Maven automatically manages project dependencies and transitive dependencies.
3. **Standardized Build Process**: Maven standardizes the build process, making it easier for developers to understand the build process across different projects.
4. **Build Lifecycle**: Maven has a predefined build lifecycle, which consists of a series of build phases that the project goes through to be built and deployed.
5. **Build Plugins**: Maven provides plugins to support various build tasks, such as compiling code, running tests, packaging, and deploying applications.
6. **Project Reporting**: Maven can generate project documentation and reports, including code coverage, test results, and dependency information.



### What is next 
After explaining the Java HelloWorld program, you can proceed to the next branch to set up Jenkins for Maven and run the same job from a freestyle project.

In the next step, we will configure Maven in Jenkins and create a Maven job in Jenkins to build and run the project.


# Disclaimer
<details>

Please note that the entire repository is owned and maintained by [Varun Kumar Manik](https://www.linkedin.com/in/vkmanik/). While every effort has been made to ensure the accuracy and reliability of the information and resources provided in this repository, Varun Kumar Manik takes full responsibility for any errors or inaccuracies that may be present.

Simplilearn is not responsible for the content or materials provided in this repository and disclaims all liability for any issues, misunderstandings, or claims that may arise from the use of the information or materials provided. By using this repository, you acknowledge that Varun Kumar Manik is solely accountable for its content, and you agree to hold Simplilearn harmless from any claims or liabilities that may arise as a result of your use or reliance on the information provided herein.

It is important to understand that this repository contains educational materials for a training course, and users are expected to apply their own judgment and discretion when utilizing the provided resources. Neither Varun Kumar Manik nor Simplilearn can guarantee specific results or outcomes from following the materials in this repository.

</details>



