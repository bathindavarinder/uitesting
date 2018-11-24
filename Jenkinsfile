pipeline {
  agent any
  stages {
    stage('Checkout message') {
      steps {
        echo 'Testing done'
      }
    }
    stage('') {
      steps {
        build(job: 'Build', wait: true)
      }
    }
  }
}