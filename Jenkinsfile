pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building....'
      }
    }
    stage('testing') {
      parallel {
        stage('testing') {
          steps {
            echo 'teting chrome'
          }
        }
        stage('') {
          steps {
            echo 'tersting firefox'
          }
        }
      }
    }
    stage('Deploying') {
      steps {
        echo 'deplying to production'
      }
    }
  }
}