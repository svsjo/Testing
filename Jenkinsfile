pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'dotnet build ConsoleApp1.sln'
          }
        }

        stage('ps') {
          steps {
            powershell 'Get-ChildItem -Path C:\\Users\\entep04\\source\\repos\\ConsoleApp1 -recurse -include *.sln'
          }
        }

      }
    }

    stage('Test') {
      steps {
        powershell 'dotnet test ConsoleApp1.sln'
      }
    }

  }
}