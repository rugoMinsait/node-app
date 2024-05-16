/*
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
*/

pipeline {
    agent { docker { image 'node:20.11.1-alpine3.19' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
