pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        bat(returnStatus: true, returnStdout: true, script: 'mkdir pipeine_dir_pokus')
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}