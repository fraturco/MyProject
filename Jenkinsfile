pipeline {
    agent any 
    tools {
        maven 'Maven'
     }
    stages {
        stage('git') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('install') { 
            steps {
                sh 'mvn install'
            }
        }
        stage('deploy'){
            steps{
             sh 'mvn deploy -com.mvn MyProject'
            }
        }
    }
}
