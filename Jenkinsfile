pipeline {
  agent any
  stages {
    stage('Testing') {
      steps {
        echo 'Initializing tests'
        sh './run-all-tests.sh'
      }
    }
    stage('Build') {
      steps {
        echo 'Building image for deployment'
      }
    }
    stage('Approval') {
      steps {
        sh './wait-for-approval.sh'
      }
    }
  }
}