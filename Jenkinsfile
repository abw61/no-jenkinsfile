pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building my app'
      }
    }
    stage('testing') {
      parallel {
        stage('testing') {
          steps {
            echo 'unit tests'
          }
        }
        stage('seleniu,') {
          steps {
            echo 'runnung my selenium tests'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        echo 'i am now deploying'
      }
    }
  }
}