pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building....'
      }
    }
    stage('testing') {
      steps {
        parallel(
          "testing": {
            echo 'firefox....'
            
          },
          "chrome": {
            echo 'testing chrome'
            
          }
        )
      }
    }
    stage('deploying') {
      steps {
        echo 'now i am deploying'
      }
    }
  }
}