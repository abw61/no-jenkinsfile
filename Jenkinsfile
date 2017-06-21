pipeline {
  agent none
  stages {
    stage('preparation') {
      steps {
        echo 'hello from Jenkins master'
        node(label: 'docker-cloud') {
          echo 'hello from Jenkins agent'
        }
        
      }
    }
  }
}