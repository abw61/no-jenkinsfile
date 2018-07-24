pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'i am building'
          }
        }
        stage('') {
          steps {
            echo 'building on windows'
          }
        }
      }
    }
    stage('testing') {
      parallel {
        stage('testing') {
          steps {
            echo 'testing in chrome'
          }
        }
        stage('') {
          steps {
            echo 'test in edge'
          }
        }
      }
    }
    stage('regression') {
      steps {
        echo 'testing.....'
        echo 'deploy'
      }
    }
    stage('deploy') {
      steps {
        echo 'im deploying'
      }
    }
  }
}