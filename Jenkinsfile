pipeline {
  agent any
  stages {
    stage('run_test') {
      steps {
        bzt(params: 'Jemkins.jmx', alwaysUseVirtualenv: true)
        catchError() {
          echo 'error happened'
        }
        
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}