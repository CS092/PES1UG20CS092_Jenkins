pipeline { 
  agent any
  stages { 
    stage('Build') { 
      steps { 
        sh 'build PES1UG20C0S92-1'
        echo 'Build Stage Successful' 
      }
    } 
    stage('Test') {
      steps { 
        sh 'a.exe'
        echo 'Test Stage Successful'
      } 
     }
    } 
    stage('Deploy') { 
      steps { 
        echo 'Deployment Successful' 
      }
    }
  post {
    failure { 
      echo 'Pipeline failed' 
    }
  }
}
