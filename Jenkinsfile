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
  
  stage('Test')
  {
    steps{
        script {
    bat   "C:/Program Files (x86)/Microsoft Visual Studio/2017/Professional/Common7/IDE/MSTest.exe" /testcontainer:UITestingAPP.Tests/bin/Release/UITestingAPP.Tests.dll /resultsfile:TestResults.trx
    
        }
        }
  }
}
