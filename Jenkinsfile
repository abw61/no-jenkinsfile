pipeline {
  agent {
    node {
      label 'docker-cloud'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        echo 'this stage is building my application'
      }
    }
    stage('Testing') {
      steps {
        parallel(
          "Chrome": {
            echo 'testing with Chrome'
            
          },
          "Firefox": {
            echo 'testing with Firefox'
            
          }
        )
      }
    }
    stage('Deploying') {
      steps {
        echo 'deploying application to production'
      }
    }
  }
}