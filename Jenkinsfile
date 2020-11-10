pipeline {
    agent any 
    tools {
        maven 'Maven'
     }
    stages {
        stage('SCM Checkout') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('package') { 
            steps {
                sh 'mvn package'
            }
        }
    }
}
