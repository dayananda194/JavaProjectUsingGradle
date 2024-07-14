To build the project using GRADLE with Command Line Interface  , Follow these steps :

1 ./gradlew build  - Builds the java Project
2 ./gradlew clean  - Deletes the build folder .
3 ./gradlew jar   - Creates the executable jar file . 
4 To run the jar file , we need to mention which is the entry file to execute  . We have to mention it under the build.gradle file 
     jar{
    manifest {
        attributes(
                'Main-Class':'org.example.Main'
        )
    }

  }

5 Finally to run the jar file 
   java -jar build/libs/jar_file_name.jar
