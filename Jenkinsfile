pipeline {
    agent any 
    stages {
        stage('SCM Chechout') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('compile-packege') { 
            steps {
               sh 'mvn package'
            }
        }
    }
}
