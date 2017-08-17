pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo $username'
      }
    }
  }
  environment {
    user = 'credentials(\'global-user1\')'
  }
}