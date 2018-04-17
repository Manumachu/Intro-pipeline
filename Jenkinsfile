pipeline {
  agent any
  stages {
    stage('Mallika-test-pipeline') {
      steps {
        echo "Hello ${params.Name}!"
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