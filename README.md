# jenkins-multibranch

## Sample Java Project with Maven

To create a sample Java project with Maven that prints "Hello, World!", follow these steps:

### Prerequisites

- Java Development Kit (JDK) installed
- Apache Maven installed

### Steps

1. **Generate a Maven Project:**

    Open a terminal and run the following command to generate a new Maven project:

    ```sh
    mvn archetype:generate -DgroupId=com.example -DartifactId=hello-world -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
    ```

2. **Navigate to the Project Directory:**

    ```sh
    cd hello-world
    ```

3. **Update the `App.java` File:**

    Open `src/main/java/com/example/App.java` and update it to print "Hello, World!":

    ```java
    package com.example;

    public class App {
         public static void main(String[] args) {
              System.out.println("Hello, World!");
         }
    }
    ```

4. **Build the Project:**

    Run the following command to build the project:

    ```sh
    mvn package
    ```

5. **Run the Application:**

    After the build is successful, run the application using the following command:

    ```sh
    java -cp target/hello-world-1.0-SNAPSHOT.jar com.example.App
    ```

    You should see the output:

    ```
    Hello, World!
    ```

### Conclusion

You have successfully created a simple Java project with Maven that prints "Hello, World!".