pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'i am building a simple app.....'
          }
        }
        stage('error') {
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
        stage('test2') {
          steps {
            echo 'test in edge'
            junit(testResults: 'results', healthScaleFactor: 5)
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