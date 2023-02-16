pipeline { 
  agent any
  stages { 
    stage('Build') { 
      steps { 
        sh 'g++ main/hello.cpp'
        echo 'Build Stage Successful' 
      }
    } 
    stage('Test') {
      steps { 
        sh 'dir'
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
