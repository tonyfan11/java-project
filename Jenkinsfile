pipeline {
  agent none

  stages {
     stage('build') {
       steps {
        sh 'ant -f build.xml -v'
      }
    }
  }
  post {
        success {
          archive 'dist/*.jar'
	    }
    }
}
