 pipeline {    
    agent any 
    
    tools {
        maven 'maven'
    }

    stages {
       stage('Git Checkout') {
            steps {
            https://github.com/atharvalanke4/maven-tomcat-sample.git
            }
        }
        
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
