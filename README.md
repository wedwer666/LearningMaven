# LearningMaven
Apply resource filtering on 2 profile defined in configuration file

Run following comands in GitBash:
1) mvn clean process-resources

2) mvn package -Ptest 
(observe that the content of target textfile.txt file changed to test)

$ mvn package -Ptest
[INFO] Scanning for projects...
[INFO]
[INFO] ---------------------< com.task.maven:mainproject >---------------------
[INFO] Building mainproject 1.0-SNAPSHOT
[INFO] --------------------------------[ jar ]---------------------------------
[INFO]
[INFO] --- maven-resources-plugin:2.6:resources (default-resources) @ mainproject ---
[WARNING] File encoding has not been set, using platform encoding Cp1252, i.e. build is platform dependent!
[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] Copying 4 resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:compile (default-compile) @ mainproject ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-resources-plugin:2.6:testResources (default-testResources) @ mainproject ---
[WARNING] Using platform encoding (Cp1252 actually) to copy filtered resources, i.e. build is platform dependent!
[INFO] skip non existing resourceDirectory C:\Users\IdeaProjects\mainproject\src\test\resources
[INFO]
[INFO] --- maven-compiler-plugin:3.1:testCompile (default-testCompile) @ mainproject ---
[INFO] Nothing to compile - all classes are up to date
[INFO]
[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ mainproject ---
[INFO] No tests to run.
[INFO]
[INFO] --- maven-antrun-plugin:1.1:run (default) @ mainproject ---
[INFO] Executing tasks
     [echo] Using env.test.properties
[INFO] Executed tasks
[INFO]
[INFO] --- maven-jar-plugin:2.4:jar (default-jar) @ mainproject ---
[INFO] Building jar: C:\Users\IdeaProjects\mainproject\target\mainproject-1.0-SNAPSHOT.jar
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  1.475 s
[INFO] Finished at: 2019-01-15T15:02:15+02:00
[INFO] ------------------------------------------------------------------------

3)  mvn package -Pdev
(observe that the content of target textfile.txt file changed to dev)

Important pages for learning purposes:

https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html

