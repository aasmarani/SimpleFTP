pipeline {
  agent {
    node {
      label 'jslave'
    }
    
  }
  stages {
    stage('') {
      steps {
        catchError() {
          sh 'echo "failed"'
        }
        
        echo 'hello'
      }
    }
  }
}