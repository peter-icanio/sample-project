pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'ls'
        sh 'docker buils . -t python-web'
        sh 'docker images'
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
