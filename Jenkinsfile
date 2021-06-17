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
        sh 'echo pwd();'
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