pipeline {
  agent any
  stages {
    stage('preparation') {
      steps {
        node(label: 'docker-cloud') {
          sh 'echo \'git command...\''
        }
        
      }
    }
  }
}