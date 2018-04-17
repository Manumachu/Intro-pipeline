pipeline {
  agent any
  stages {
    stage('Mallika-test-pipeline') {
      steps {
        echo 'Hello ${My_NAME}!'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'Mallika'
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}