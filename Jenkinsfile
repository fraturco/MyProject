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
                sh 'mvn install'
            }
        }
    }
    post {
        success{
            echo 'The pipeline success'
        }
        failure{
         echo 'The pipeline fails'
        }
    }
}
