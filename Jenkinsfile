pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!' 
            }
        }
        stage('TWO') {
            steps {
                input('Do you want to Proceed') 
            }
        }
        stage('THREE') {
            when  { 
                     not {
                          branch "master"
                     }
           }
           steps {
                echo 'Hello world!' 
            }
        }
    }
}
