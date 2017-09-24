pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        parallel(
          "error": {
            bat(returnStatus: true, returnStdout: true, script: 'mkdir pipeine_dir_pokus')
            
          },
          "message 1": {
            echo 'Hello'
            
          },
          "message 2": {
            sleep 1
            echo 'Hello 2'
            
          }
        )
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}