pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'dotnet build ConsoleApp1.sln'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing.....'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying.......'
      }
    }

  }
}