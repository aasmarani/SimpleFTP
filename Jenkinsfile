pipeline {
  agent {
    node {
      label 'jslave'
    }
    
  }
  stages {
    stage('Condition') {
      steps {
        waitUntil() {
          sh 'echo "testing child step"'
          mail(subject: 'failed', body: 'failed body', to: 'aasmarani@bajau.com')
          waitUntil() {
            sh 'echo "success"'
          }
          
        }
        
      }
    }
  }
}