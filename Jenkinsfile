pipeline {
    agent any
    
    tools {
        maven "Maven 3.8.3"
    }
    
    stages {
        stage('Build') {
            steps {             
                bat "mvn clean"
            }
        }
        stage('Clean') {
          steps{
                bat "mvn compile"
            }
        }
        stage('Empaquetar'){
          steps{
                bat "mvn package"
            }
        }
    }
}
