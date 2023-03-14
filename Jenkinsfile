pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'build App'
      }
    }
    
    stage('Test') {
      steps {
        echo 'Test App'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy App'
      }
    }
  }
   
  post {
    always {
      emailext attachLog: true, body: 'testing....', subject:'Pipeline Post Mail', to: 'sujatawakpanjar33@gmail.com'
      
    }
  }
}
