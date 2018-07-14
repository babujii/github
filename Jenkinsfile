pipeline {
  agent any
  stages {
    stage('build stage') {
      steps {
        build(job: 'uptime', propagate: true, wait: true, quietPeriod: 2)
      }
    }
    stage('Test stage') {
      steps {
        sh 'uptime'
      }
    }
  }
}