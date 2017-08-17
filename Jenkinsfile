pipeline 
{
  agent any
  
  stages {
    stage('Build') {
      steps {
      withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: '0286c4f7-3b78-4a4a-b67c-60b3b05a1582',usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']])
      {
        sh 'echo $USERNAME' >> /tmp/test.txt
        sh 'echo $PASSWORD' >> /tmp/test.txt
      }
      
    }
  }
  }
  environment {
    user = 'credentials(global-user1)'
  }
}