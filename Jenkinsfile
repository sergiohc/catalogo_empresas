pipeline {
  agent any
  stages {
    stage('Install Dependencias') {
      steps {
        sh 'npm install'
        sh 'bundle install'
      }
    }
    stage('Build Assets') {
      steps {
        sh 'npm run build'
      }
    }
    stage('Build Jekyll') {
      steps {
        sh 'jekyll build'
      }
    }
  }
}
