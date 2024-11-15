pipeline {
  agent {
    docker {
      image 'mcr.microsoft.com/dotnet/aspnet:8.0'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'dotnet build'
      }
    }

  }
}