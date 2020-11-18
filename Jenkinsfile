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
        tr {
        stage('install') { 
            steps {
                sh 'mvn install'
            }
          }
        }
        cathc (e){
        
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
