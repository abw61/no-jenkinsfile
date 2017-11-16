pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'running a build'
      }
    }
    stage('testing') {
      parallel {
        stage('') {
          steps {
            node(label: 'xlarge') {
              echo 'running a test'
            }
            
          }
        }
        stage('test-1') {
          steps {
            echo 'running test-1'
          }
        }
        stage('test-2') {
          steps {
            echo 'running test-2'
          }
        }
      }
    }
    stage('deploying') {
      steps {
        node(label: 'large') {
          echo 'deploying...'
        }
        
      }
    }
  }
}