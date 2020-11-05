pipeline {
    agent any 
    stages {
        stage('SCM Chechout') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('compile-package') { 
            steps {
                def mvnHome = tool name: 'Maven', type: 'maven'
                sh "${mvnHome}/bin/mvn package"
            }
        }
    }
}
