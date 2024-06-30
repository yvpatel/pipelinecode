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
           echo "code is build & deployed"
         }
      }
      stage('test') {
        steps {
           echo "application is working fine"
         }

     }

}

}