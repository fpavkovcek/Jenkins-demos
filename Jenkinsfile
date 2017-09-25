pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        bzt 'Jemkins.jmx'
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}