pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        echo 'Fetch data from Git'
        git(url: 'https://github.com/Shravani2780/Example1.git', branch: 'dev', credentialsId: 'Shravani2780')
      }
    }

    stage('Build') {
      steps {
        emailext(subject: 'Build Status', body: 'Build complete', attachLog: true, to: 'sravani.manduva@acsicorp.com')
      }
    }

    stage('Test') {
      steps {
        timestamps()
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment done'
      }
    }

  }
  environment {
    Git = '10'
  }
}