pipeline {
  agent {
    docker {
      image 'ruby'
    }
    
  }
  stages {
    stage('uild') {
      steps {
        echo 'echo building....'
      }
    }
    stage('Tests') {
      parallel {
        stage('Chrome') {
          steps {
            echo 'chrome tests'
          }
        }
        stage('Ffox') {
          steps {
            echo 'firefox tests'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'deploying...'
      }
    }
  }
}