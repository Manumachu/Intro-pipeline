pipeline {
  agent any
  stages {
    stage('Mallika-test-pipeline') {
      parallel {
        stage('Mallika-test-pipeline') {
          steps {
            echo 'Hello World'
          }
        }
        stage('Label') {
          steps {
            sh '''pipeline {
   agent {
    label \'jdk9\'
    }
stages{
      stage(\'Say Hello\') {
         steps {
            echo \'Hello World!\'   
            sh \'java -version\'
         }
      }
   }
}'''
            }
          }
        }
      }
    }
  }