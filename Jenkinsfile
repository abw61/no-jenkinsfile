pipeline {
  agent {
    docker {
      image 'ruby-docker'
    }
    
  }
  stages {
    stage('') {
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