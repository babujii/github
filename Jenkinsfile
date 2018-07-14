pipeline {
  agent any
  stages {
    stage('build stage') {
      parallel {
        stage('build stage') {
          steps {
            build(job: 'uptime', propagate: true, wait: true, quietPeriod: 2)
          }
        }
        stage('') {
          steps {
            sh 'date'
          }
        }
      }
    }
    stage('Test stage') {
      steps {
        sh 'uptime'
      }
    }
    stage('junit test') {
      steps {
        echo 'junit test'
      }
    }
    stage('Deploy test') {
      steps {
        sh 'uptime'
      }
    }
  }
}