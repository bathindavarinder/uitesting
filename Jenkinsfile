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
                              def msbuild = tool name: 'MSBuild', type: 'hudson.plugins.msbuild.MsBuildInstallation'
                              bat "${msbuild} UITestingAPP.sln"
                         } 
                      }
                    }
  }
}
