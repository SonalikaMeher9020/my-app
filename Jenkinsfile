pipeline {
    agent any 
    tools {
        maven 'apache-maven-3.6.3'
        jdk 'jdk-11.0.6'
    }
    stages {
        stage('===== Clean ======') { 
            steps {
                bat "mvn clean"
            }
        }
        stage('=====Test=====') { 
            steps {
                bat "mvn clean test"
            }
        }
        stage('=====Deploy=====') { 
            steps {
                bat "mvn package"
            }
        }
    }
}
