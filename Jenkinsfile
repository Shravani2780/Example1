pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'this is build stage'
      }
    }

    stage('Test') {
      steps {
        echo 'this is test state'
      }
    }

    stage('Deploy') {
      steps {
        echo 'This is deployment stage'
      }
    }

  }
  environment {
    Development = '20'
  }
}