pipeline{
    agent any 
    stages {
          stage('checkout') {
            steps {

                checkout([$class: 'GitSCM',
                    branches: [[name: '*/main']],
                    userRemoteConfigs: [[url: 'https://github.com/kowshigowda/calculator.git',
                    credentialsId: 'Git_calculator']]])
            }
          }
    }
        stage('Build') {
            steps {
                    sh '''
                    ls -lrt
                    sleep 5
                    '''
            }
        }
        stage('Test') {
            steps {
                sh '''
                sleep 5
                '''
            }
       }
    }
