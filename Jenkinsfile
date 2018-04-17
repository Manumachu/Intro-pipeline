pipeline {
  agent any
  stages {
    stage('Mallika-test-pipeline') {
      steps {
        echo "Hello ${params.Name}!"
      }
    }
    stage('Testing') {
      failFast true
      parallel {
        stage('Java 7') {
          agent {
            docker 'openjdk:7-jdk-alpine'
          }
          steps {
            sh 'java -version'
            sleep(time: 10, unit: 'SECONDS')
          }
        }
        stage('Java 8') {
          agent {
            docker 'openjdk:8-jdk-alpine'
          }
          steps {
            sh 'java -version'
            sleep(time: 20, unit: 'SECONDS')
          }
        }
      }
    }
  }
}