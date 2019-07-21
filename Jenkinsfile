pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo " buid is triggered"'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo " test is running"'
          }
        }
        stage('unittest') {
          steps {
            sh 'echo " unit test is visible"'
          }
        }
        stage('integration test') {
          steps {
            sh 'echo " test is build"'
          }
        }
      }
    }
    stage('dev') {
      steps {
        sh 'echo " dev hai"'
      }
    }
    stage('prod') {
      steps {
        sh 'echo " hai"'
      }
    }
  }
}