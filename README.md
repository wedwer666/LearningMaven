# LearningMaven
Apply resource filtering on 2 profile defined in configuration file

Run following comands in GitBash:
1) mvn clean process-resources

2) mvn package -Ptest 
(observe that the content of target textfile.txt file changed to test)

3)  mvn package -Pdev
(observe that the content of target textfile.txt file changed to dev)

Important pages for learning purposes:

https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html

