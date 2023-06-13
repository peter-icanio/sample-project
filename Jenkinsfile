pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'ls'
        sh 'docker build . -t python-web'
        sh 'docker images'
      }
    }
    
    stage('Deploy') {
      steps {
        // Perform deployment steps for your Python application
        sh 'docker run -itd -p "1234:1234" python-web:latest '
      }
    }
  }
}
