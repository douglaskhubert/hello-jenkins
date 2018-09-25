pipeline {
  agent any
  stages {
    stage('Testing') {
      steps {
        echo 'Initializing tests'
      }
    }
    stage('Build') {
      steps {
        echo 'Building image for deployment'
      }
    }
    stage('Approval') {
      steps {
        echo 'Approved'
        sleep(unit: 'DAYS', time: 1)
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployed'
      }
    }
  }
}