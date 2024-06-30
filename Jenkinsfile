pipeline {
  
agent any
  stages {
   
      stage('SCM') {
        steps {
           echo 'Pulling Source code from GitHubRepo'
           git 'https://github.com/yvpatel/simple-java-maven-app.git'
         }
      }
      stage('build') {
        steps {
           echo "code fetch from gitrepo and generating artifect using maven"
           sh 'mvn clean package'
         }
      }
      stage('Deployed') {
        steps {
           echo "code is deployed to Production"
           sh 'java -jar target/*.jar'
         }

     }

      stage('Test') {
        steps {
           echo "code is working well"
         
         }

     }

}

}