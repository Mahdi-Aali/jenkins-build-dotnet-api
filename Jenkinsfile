pipeline {
  agent {
    docker {
      image 'mcr.microsoft.com/dotnet/aspnet:8.0'
    }

  }
  stages {
    stage('pull') {
      steps {
        git(url: 'https://github.com/Mahdi-Aali/jenkins-build-dotnet-api', branch: 'master')
        sh 'git pull'
      }
    }

    stage('restore') {
      steps {
        sh 'dotnet restore'
      }
    }

  }
}