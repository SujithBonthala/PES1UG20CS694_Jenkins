pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ Lab-2a.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test') {
      steps {
        sh './a.ot'
        echo 'Test Stage Successful'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline failed'
    }
  }
}
