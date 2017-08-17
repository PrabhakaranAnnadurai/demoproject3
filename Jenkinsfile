pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo $user'
      }
    }
  }
  environment {
    user = 'credentials(\'global-user1\')'
  }
}