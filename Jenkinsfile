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
                  script {
                     bat "\"${tool 'MSBuild'}\" UITestingAPP.sln /t:Rebuild /p:Configuration=Release"                            
                         } 
                      }
                    }
  }
}
