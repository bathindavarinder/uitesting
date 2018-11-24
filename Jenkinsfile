pipeline {
  agent any
  stages {
    stage('Checkout message') {
      steps {
        echo 'Testing done'
      }
    }
    stage('Build') {
      steps {
        build(job: 'Build', wait: true)
      }
    }
  }
}