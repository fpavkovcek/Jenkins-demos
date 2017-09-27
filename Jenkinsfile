pipeline {
  agent any
  stages {
    stage('run_test') {
      steps {
        bzt(params: 'Jemkins.jmx', generatePerformanceTrend: true, printDebugOutput: true, useBztExitCode: true)
      }
    }
  }
  environment {
    UAT1 = 'UAT1'
  }
}