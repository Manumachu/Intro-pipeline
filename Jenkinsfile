pipeline {
  agent any
  stages {
    stage('Mallika-test-pipeline') {
      steps {
        echo "Hello ${params.Name}!"
      }
    }
    stage('Deploy') {
      options {
        timeout(time: 10, unit: 'MINUTES')
      }
      input {
        message 'Should we continue?'
      }
      steps {
        echo 'Continuing with deployment'
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