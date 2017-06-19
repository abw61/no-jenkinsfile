stage('build') {
  node {
    sh "echo running the build"
	// uncomment when killing master for failover tests
	// sh “sleep 60”
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
