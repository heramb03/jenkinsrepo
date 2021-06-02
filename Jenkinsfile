pipeline {
    agent any

    stages {
        stage('Development') {
            steps {
                echo 'This  is development stage'
            }
        }
        stage('build') {
            steps {
            build quietPeriod: 5, job: 'testjob'
            }
         }
         
        stage('Deployment') {
            steps {
             echo 'This is deployment stage'
            }
          }
        
        stage('Build second job') {
            steps {
            build quietPeriod: 5, job: 'testjob1'
            }
         }
        
        stage('production') {
            steps {
              echo 'This is production stage'
            }
          }

    }
}
