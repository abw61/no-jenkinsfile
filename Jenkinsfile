pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building the app'
      }
    }
    stage('testing') {
      parallel {
        stage('testing chrome') {
          steps {
            echo 'testing chrome'
          }
        }
        stage('testing firefox') {
          steps {
            echo 'firefox'
          }
        }
        stage('edge') {
          steps {
            echo 'tsting with edge'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        echo 'deploying...'
      }
    }
  }
}