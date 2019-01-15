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
http://www.avajava.com/tutorials/lessons/how-do-i-filter-resources-based-on-values-from-a-properties-file.html?page=2
http://www.vogella.com/tutorials/ApacheMaven/article.html
