pipeline {
  agent any
  withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: '0286c4f7-3b78-4a4a-b67c-60b3b05a1582',usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']])
  stages {
    stage('Build') {
      steps {
        sh 'echo $USERNAME'
      }
    }
  }
  environment {
    user = 'credentials(global-user1)'
  }
}