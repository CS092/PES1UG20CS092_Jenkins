pipeline { 
  agent any
  stages { 
    stage('Build') { 
      steps { 
        sh '/var/jenkins_home/workspace/PES1UG20CS092-1/main/hello_exec'
        echo 'Build Stage Successful' 
      }
    } 
    stage('Test') {
      steps { 
        sh 'a.exe'
        echo 'Test Stage Successful'
      } 
    }
    stage('Deploy') { 
      steps { 
        sh ''
        echo 'Deployment Successful' 
      }
    }
  }
  post {
    failure { 
      echo 'Pipeline failed' 
    }
  }
}
