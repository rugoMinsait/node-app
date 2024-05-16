pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }
    stage('Install dependencies') {
      steps {
        sh 'node -v'
      }
    }
    stage('Run Tests') {
      steps {
        sh 'npm test'
      }
    }
  }
}
