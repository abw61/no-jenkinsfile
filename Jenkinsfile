stage('build') {
  node {
    sh "echo running the build"
  }
}

stage('test') {
    parallel 'quality scan': {
        echo "running unit tests"
    }, 'static': {
         echo "running static analysis"
    }
}

stage('deploy') {
  echo 'deploy some things'
}
