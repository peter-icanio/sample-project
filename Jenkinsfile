pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        // Perform build steps (e.g., installing dependencies) for your Python application
        sh 'ls'
        sh 'pip install Flask'
      }
    }
    
    stage('Deploy') {
      steps {
        // Perform deployment steps for your Python application
        //sh 'pm2 delete python-api'
        sh 'pm2 start "python3 app.py" --name python-web-project'
      }
    }
  }
}
