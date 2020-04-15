pipeline {
    agent any 
    stages {
        stage('Build Appication') { 
            steps {
                bat 'mvn clean install' 
            }
        }
        
       stage('Deploy Mule  Appication into cloud') { 
            steps {
                bat 'mvn package deploy -DmuleDeploy' 
            }
        }
      }
}