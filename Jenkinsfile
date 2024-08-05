 pipeline {     
    agent {label 'Jenkins-Slave'} 
    
    tools {
        jdk 'JDK'
        maven 'Maven3'
    } 

    stages {
        
         
        stage('Compile') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('tests') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Build') {
            steps {
                sh "mvn package"
            }
        }
    }
}
