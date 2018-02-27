pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn deploy'
      }
    }
    stage('test') {
      steps {
        sh 'mvn build'
      }
    }
    stage('release') {
      steps {
        sh 'mvn release'
      }
    }
    stage('deploy') {
      steps {
        sh 'mvn deploy'
      }
    }
  }
}