pipeline {
    agent any 
    tools {
        maven 'Maven'
     }
    stages {
        stage('SCM Chechout') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('compile-package') { 
            steps {
                sh 'mvn package'
            }
        }
    }
}
