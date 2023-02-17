pipeline { 
  agent any
  stages { 
    stage('Build') { 
      steps { 
        sh 'make'
        echo 'Build Stage Successful' 
      }
    } 
    stage('Test') {
      steps { 
        sh './hello_exec'
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
