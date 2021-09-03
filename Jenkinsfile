pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '- msbuild /p:Configuration=Debug ConsoleApp1.sln'
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