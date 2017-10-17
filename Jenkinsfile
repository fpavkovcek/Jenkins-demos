pipeline {
  agent any
  stages {
    stage('run_test') {
      steps {
        parallel(
          "run_test": {
            bzt(params: 'Jemkins.jmx', alwaysUseVirtualenv: true)
            catchError() {
              echo 'error happened'
            }
            
            
          },
          "": {
            echo 'paralel'
            sleep(time: 1, unit: 'SECONDS')
            
          }
        )
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}