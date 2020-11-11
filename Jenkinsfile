pipeline {
    agent any 
    tools {
        maven 'Maven'
        git 'Git'
     }
    stages {
        stage('git') { 
            steps {
                git 'https://github.com/fraturco/MyProject'
            }
        }
        stage('install') { 
            steps {
                sh 'mvn cosa'
            }
        }
        stage('deploy'){
            steps{
             sh 'mvn deploy  MyProject'
            }
        }
    }
    post {
        success{
        emailext body:'Test mail' 
        }
    }
}
