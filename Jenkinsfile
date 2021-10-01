pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build1') {
          steps {
            sh 'dotnet build ConsoleApp1.sln'
            archiveArtifacts 'ConsoleApp1/bin/Debug/ConsoleApp1.exe'
          }
        }

        stage('build2') {
          steps {
            powershell 'echo DoSomething'
          }
        }

      }
    }

    stage('Test') {
      steps {
        powershell 'echo Do Something'
      }
    }

  }
}