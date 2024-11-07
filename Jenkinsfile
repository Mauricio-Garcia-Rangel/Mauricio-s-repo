pipeline {
  agent {
    node {
      label 'docker-agent-python'
    }

  }
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/Mauricio-Garcia-Rangel/Mauricio-s-repo.git', branch: 'master')
      }
    }

  }
  triggers {
    pollSCM('* * * * *')
  }
}