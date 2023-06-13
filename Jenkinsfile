pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'docker images'
        sh 'ls'
      }
    }
    
    stage('Deploy') {
      steps {
        // Perform deployment steps for your Python application
        sh 'python3 app.py'
      }
    }
  }
}
